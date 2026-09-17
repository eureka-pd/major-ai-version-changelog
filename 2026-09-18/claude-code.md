# Claude Code 변경사항

## GUI App

- 버전: `2.1.274` (이전: `2.1.273`)
- 메모리 임계 경고, `CLAUDE_CODE_MCP_STARTUP_WAIT_MS`, OTel `effort`·`managed_settings_resolved`·`enduser.sub`, 게이트웨이 Postgres `store.connect_timeout_seconds`·복제본 과부하 경고, 전체화면에서 접힌 teammate/agent 메시지 클릭 확장을 넣었습니다.
- `unexpected tool_use_id` 400 무한 재시도(손상 트랜스크립트 자가 치유·`/rewind`), legacy HTTP+SSE MCP의 4xx 폴백, Streamable HTTP MCP 5분 고정 타임아웃, `listChanged` 없이 list-changed 알림 시 프롬프트·리소스 미갱신, MCP 403 insufficient_scope를 만료 로그인으로 오인하던 문제를 고쳤습니다.
- `/goal`이 reactive compaction 뒤 "Prompt is too long"으로 종료되던 문제·resume 시 goal 유실, `claude agents` 자동 업데이트 후 플래그 유실, 대규모 LSP 진단으로 턴 지연, Bedrock/Vertex/Foundry에서 `model: "opus"` 서브에이전트가 세션 모델을 버리던 문제, 셀프호스트 러너 401 후 재시도·토큰 재발급을 고쳤습니다.
- VS Code/터미널의 로컬 경로 `file://` 링크, 트랜스크립트 번호 목록 재번호 매김, AskUserQuestion 미리보기 노트·하이라이트 옵션, resume된 백그라운드 에이전트의 중단된 툴 배치, `CLAUDE_CODE_RESUME_INTERRUPTED_TURN`의 미완료 백그라운드 보고, 클라우드 첫 턴의 아직 연결 중인 SDK MCP 도구 누락을 고쳤습니다.
- 훅 세션 Stop 프롬프트 전체 재전송, Wayland+Cursor/VS Code에서 빈 에디터 창, 게이트웨이 Postgres 끊김·SIGTERM 드레인(`CLAUDE_GATEWAY_DRAIN_TIMEOUT_MS`), 원격 managed 정책 시 `installed_plugins.json` 매 기동 재작성, headless/SDK의 백그라운드 완료마다 별도 모델 호출, 플러그인 reload 후 Bash 프로필 재소스, `$schema` hooks 경고, MCP 설정 `${VAR}` 비밀 노출을 고쳤습니다.
- Bash 특수 변수 루프/할당·worktree 세션의 중첩 셸 확장을 권한 검사에서 다루고, 멀티바이트 Edit 미리보기 위치, 메모리 압박 시 30분 idle로 백그라운드 명령이 죽던 문제(임계일 때만), Desktop 재기동 후 서브에이전트→메인 메시지 유실, zip 플러그인 중복 reload, 서브에이전트 progress 요약이 장문으로 덮이던 문제를 고쳤습니다.
- stream-json 기동 시 tool-search 지연 MCP 대기 단축, Monitor 최종 출력·종료를 한 알림으로, Artifact 미로그인·구버전 publish·서브모듈 worktree 제거 검사를 개선했습니다.
- Bedrock/Vertex/Foundry·telemetry-off는 기본 v2 MCP 클라이언트·MCP 2026-07-28(옵트아웃: `MCP_SDK_GENERATION=v1` 등), `/code-review`는 튜닝 없는 모델에 leaner inline 프롬프트, `"type":"sdk"` MCP 항목은 스킵 경고, 로컬 artifact 외부 새 버전은 턴을 시작하지 않음, 플러그인/marketplace 클론은 Git LFS 포인터만, 셀프호스트는 읽기 거부 repo를 스킵, `/status` 등 문구를 "cloud session"으로 바꿨습니다.
- [VSCode] 창 reload 후 중단 단계 이어하기·Memory/Instructions Customize 메뉴·`claudeCode.lockEditorGroups`, `/btw` 타 세션 이력, gitignore 조회 프리즈, reload 후 툴 중 메시지 유실, 키보드로 Manage Plugins/MCP 행, `CLAUDE_CONFIG_DIR` 변경 후 로그인 상태, 긴 diff 잘림, settings.json 동시 쓰기, New Tab 포커스·잠긴 그룹 레이아웃, 세션 검색 이름 흔들림, plan review 스크롤, High Contrast 코드 가독성, 스크린 리더 "You"/"Claude" 안내, 기본 gitignore를 `$XDG_CONFIG_HOME/git/ignore`로 바꿨습니다.
- [웹] diff "Compare against" 브랜치 선택, GitHub 토큰 갱신 순간 "service unavailable", 루틴 이중 실행·일시정지 재활성, 자격 갱신 직후 서명 커밋 실패, 루틴 GitHub 트리거 토스트 원인, unread 플리커, GitHub 연결 없을 때 루틴 최대 72시간 재시도, 구독 일시정지 on-hold 안내를 고치거나 바꿨습니다.
- [Claude Tag] Add channel/workspace Guests 설정, 다른 Slack 앱 @멘션·새 채널 직후 @Claude, 늦은 후속을 silent edit로 접지 않음, 단일 채널 Slack 검색, safety-filter 무음 컨텍스트 리셋·백그라운드 취소 방지, mailto 표시, Enterprise Grid org-wide 공유 채널 watch, Environment picker 이름, 진행 체크리스트(2,000자·15분), "Channel only" guest canvas 반복 고지를 제거했습니다.
- [Code Review] 재리뷰 시 낮은 severity 메모 때문에 해결된 스레드가 열린 채 남던 문제, 일시 오류로 "Code review encountered an error", 소견을 짧은 plain sentence로, org limit skip 카드에 관리 페이지 링크를 넣었습니다.

## CLI App

- 버전: `2.1.274` (이전: `2.1.273`)
- GUI와 동일 릴리스입니다. 메모리 경고, MCP 기동 대기·타임아웃·list-changed, tool_use_id 자가 치유, `/goal`·agents 플래그·셀프호스트 러너, VS Code·웹·Tag·Code Review 수정이 포함됩니다.

## Sources

- [Claude Code changelog](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
