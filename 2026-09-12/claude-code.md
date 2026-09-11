# Claude Code 변경사항

## GUI App

- 버전: `2.1.268` (이전: `2.1.267`)
- Claude apps gateway에 `pricing:`을 두면 로그인된 Claude Code가 관리 설정으로 같은 요금을 받아 `/cost`·텔레메트리가 사용량 미터와 맞습니다.
- `access_control.allow_cidrs`가 비어 있으면 gateway 기동 경고를 내고, 공개 주소에서 첫 요청이 오면 한 번 더 경고합니다. `gatewayInternalNetworks`로 조직 공인 IPv4 대역에서 gateway `/login`을 허용할 수 있습니다.
- `claude self-hosted-runner --remove-session-state`(기본 끔)로 세션 종료 시 `_sessions/` 아래 세션 디렉터리를 지울 수 있고, `claude auth status --json`에 `configDirectory`가 들어갑니다.
- `claude plugin install`·`uninstall`·`update`·`enable`·`disable`에 `--json`을 넣었고, `plugin list --json` 행에 `errorDetails`·`noteDetails`를 붙였습니다. 게시된 아티팩트에 페이지에 맞는 브라우저 탭 아이콘을 넣습니다.
- 2.1.265 이후 서드파티 Anthropic 호환 엔드포인트(`ANTHROPIC_BASE_URL`)에서 Artifact 도구 스키마 정규식 때문에 매 턴 HTTP 400이 나던 문제를 고쳤습니다.
- WebFetch가 끝나지 않는 응답에 300초 기한을 두고(`CLAUDE_CODE_WEBFETCH_DEADLINE_MS`로 변경, 0은 끔), 신뢰하지 않은 폴더의 동명 에이전트 파일을 리스폰 팀원이 가져가던 문제를 고쳤습니다.
- 오래 유휴인 세션의 busy loop·리캡 중 빠른 focus 보고로 CPU가 치솟던 문제, MCP 도구 호출 뒤 “빈 메시지” 응답, 심링크 경로의 deny/ask 규칙·Bash 복합 줄 분석 실패를 고쳤습니다.
- 플러그인·마켓플레이스·`/mcp`·MCP 로그인 오류에 git URL·`${VAR}`로 풀린 비밀이 보이던 문제를 막고, `excludeDynamicSections` SDK 세션의 프롬프트 캐시·extended thinking 깨짐을 고쳤습니다.
- 오래된 모델 접근 거절 캐시로 권한 있는 사용자에게 제한이라고 안내하거나, 다른 프로세스가 캐시를 갱신해 기본 모델로 조용히 바뀌던 문제를 고쳤습니다.
- Fable 1M 컨텍스트 429를 크레딧 동의로 오인하던 문제, WIF 프로필 `jti reused` 401, MCP OAuth 콜백 포트 부족, `/compact` 요약의 `$` 손상·resume 순서, SDK 제안·`/rename`이 compaction 이전 대화를 보내던 문제를 고쳤습니다.
- `@`·`/` 제안, `claude agents` 뒤로가기·worktree 삭제, 에이전트 패널 줄바꿈, Slack MCP allowlist, Chrome “https” 호스트, 긴 스피너 줄바꿈, `/bug`·`/feedback` 커서, Remote Control 이름, plugin validate·monitors/SKILL 스킵, localhost WebFetch 안내를 고치거나 개선했습니다.
- PermissionRequest 훅의 `--print` 미발화, headless policy-helper 경고, `/resume` fork 이름, 로그아웃 시 Enterprise 오안내, SessionEnd 훅 타임아웃, `/autofix-pr`·클라우드 명령의 GitHub·정책 안내, Bash 샌드박스 설명 과장을 고쳤습니다.
- 전체화면 줄 추가/삭제 반응, `--continue`/`--resume` 즉시 표시, 도구 많은 턴의 불필요 재그리기, `.claude/workflows/` 기동, auto mode 거절 메시지, Chrome 긴 페이지 읽기, MEMORY.md 잘림 경고, 아티팩트 권한 질문, 푸터·1M 크레딧 안내, `/plugin` 즉시 적용을 개선했습니다.
- Bedrock·Vertex·Foundry 시스템 프롬프트·도구 목록을 1st-party와 맞추고, Task/Todo 도구 노출 모델 범위를 좁히며(`CLAUDE_CODE_ENABLE_TODO_TOOLS=1`로 확장), Artifact·WebFetch 규칙 분리, MCP 인증 안내 중복을 줄였습니다.
- [VSCode] `CLAUDE_CONFIG_DIR`·로그인 직후 빈 필·Auto 모드 소실·세션 이름·푸터 필 대기·이중 기동·sidebar preferredLocation·Windows WSL/진단·커스텀 스타일 경로를 고쳤고, 항상 허용 저장 위치 화살표·마지막 메시지 포커스·플러그인 즉시 적용·일부 아티팩트 “다시 묻지 않기” 제거를 넣었습니다.
- [웹] 6시간 넘는 세션의 persisted 폴더 유실(최대 하루 유지), effort 상한 org의 “Invalid effort level”, 커넥터 없는 루틴 생성 안내를 고치거나 개선했습니다.
- [Claude Tag] 관리 설정 로딩 실패 Retry, Slack 채널→조직 설정 링크, Enterprise Grid 채널 이동 후 설정 유실, 차단 사유 설명, 읽기 전용 조회 병렬화, 비교 포맷, `@Claude !restart` 모순 안내, org 불일치 안내, 꺾쇠 URL 링크, 게스트 @mention, 조용할 때까지 세션 갱신 대기, 채널 설정 카드 중복 거부, 공개 채널 메모리를 채널별로 나눴습니다.
- [Code Review] open findings는 스레드 resolve로만 닫힘 안내, 검증 에이전트 실패 시 교체, draft 전환 뒤 대기 리뷰 게시, 루트 동명 파일만 고친 PR에서 하위 CLAUDE.md 무시를 고쳤습니다.

## CLI App

- 버전: `2.1.268` (이전: `2.1.267`)
- GUI와 동일 릴리스입니다. gateway 요금·CIDR 경고, self-hosted runner 세션 정리, 플러그인 `--json`, 서드파티 엔드포인트 400, WebFetch 기한, 심링크 권한, 비밀 유출 방지, 프롬프트 캐시·VS Code·Claude Tag·Code Review 수정을 포함합니다.

## Sources

- [Claude Code changelog](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
