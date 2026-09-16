# Claude Code 변경사항

## GUI App

- 버전: `2.1.273` (이전: `2.1.272`)
- LLM 게이트웨이용 요청 헤더(`x-claude-code-request-class` 등, `CLAUDE_CODE_GATEWAY_HINT_HEADERS=1`), MCP 연결 끊김 알림, Remote Control/Claude 앱에서 포크한 세션을 로컬 백그라운드로 실행하는 기능을 넣었습니다.
- Bash 권한·샌드박스·`blockReadsOutsideWorkingDirectories`, 조직 Skills 끔 후 동기화 스킬 회수, MDM/`managed-settings.json` MCP 제한 무시, Bedrock·Vertex·Foundry·게이트웨이 401/403 안내, `/login`·`/upgrade` 후 프롬프트 캐시 깨짐, Artifact 업로드 승인 중단, stub `.git/info/exclude` 재생성, 셸 모드 앞머리 `!`, macOS 스크린샷 Read, 서브에이전트 결과 미전달, 컨텍스트 미터 이중 집계, `/tui` 재시작, 스케줄 작업 세션 혼선, stream-json 백그라운드 서브에이전트 출력 유실을 고쳤습니다.
- 긴 세션 반응성(훅·서브에이전트 진행), Artifact 오류·DB 필드 삭제·재전송, `/autofix-pr`·`/web-setup`·SSL/프록시·클라우드 세션·MCP 재인증 안내를 개선했습니다.
- Bedrock/Vertex/Foundry auto mode는 당분간 로컬 classifier 기본, `OTEL_LOG_TOOL_DETAILS`에 실제 이름 포함, Claude 계정 로그인 시 claude.ai 플러그인 접근 요청, `/bug`·`/feedback` 보고 범위를 좁혔습니다.
- [VSCode] 피드백 비활성 조직의 Report 폼, Windows 종료 코드 4294967295 배너를 고쳤고 UNC/`--add-dir` 네트워크 경로 권한 검사를 개선했습니다.
- [웹] 커넥터 재추가 후 루틴 접근, 셀프호스트 환경 생성 실패, Share cloud sessions 위치(Data and privacy), 루틴 편집 확인·레이아웃, 신규 사용자 데스크톱 다운로드 강제 화면 제거를 반영했습니다.
- [Claude Tag] Grid/워크스페이스·스케줄·스레드 재시작·토큰 갱신·AWS 리전리스 엔드포인트·OAuth Bearer·채널 매니저·자동 관련 채널 감시·Memory 목록을 고치거나 개선했습니다.
- [Code Review] base 머지 후 가벼운 follow-up, REVIEW.md 파싱, 제안 수정·이차 위치 문장, `/ultrareview --post` 재시도, 대문자 owner/repo의 빈 푸시 재검토를 고쳤습니다.
- `2.1.268`의 분석 불가 Bash 줄에 대한 Read/Edit deny 적용을 되돌렸습니다(`time -p make build` 등이 다시 승인 프롬프트를 받음).

## CLI App

- 버전: `2.1.273` (이전: `2.1.272`)
- GUI와 동일 릴리스입니다. 게이트웨이 힌트 헤더, MCP 끊김 알림, Remote Control 포크, 권한·Artifact·Tag·Code Review·VS Code·웹 수정이 포함됩니다.

## Sources

- [Claude Code changelog](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
