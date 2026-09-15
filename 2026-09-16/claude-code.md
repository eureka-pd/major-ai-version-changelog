# Claude Code 변경사항

## GUI App

- 버전: `2.1.272` (이전: `2.1.270`)
- `2.1.271`에서 Remote 세션(클라우드·셀프호스트) 빠른 모드(`/fast`·호스트 설정), 전체화면 `/config` 마우스(휠·클릭·호버), `claude self-hosted-runner --drain-marker-file`, 샌드박스 auto mode의 명령별 `allowed_domains`, 에이전트 `omitClaudeMd`, `claude plugin install|update --accept-command`, `modelPricing`/`pricing` multiplier(1–10), Bedrock·Vertex·Foundry·gateway 사용자를 데스크톱 앱·`/desktop`으로 안내하는 tip을 넣었습니다.
- org·계정·API 키 전환 뒤 캐시된 조직 정책 재사용, 정책 로드 후 도구·명령 목록 미갱신, 읽기 불가 `managed-mcp.json`이 exclusive MCP를 놓치던 문제, `ANTHROPIC_UNIX_SOCKET` 프록시가 org 정책을 거절하던 문제, 워커 재시작 후 서브에이전트 스키마 검증 실패, `/fast off`·skip-org-check·retry-watchdog 빠른 모드 경로를 고쳤습니다.
- Bash 권한 검사(`fmt`/`column`·와일드카드·변수 선언·이중 `cd`/`cd`+`git`), Linux `.git/config.lock` 잔존, macOS 파일 감시 폴링 폴백, MCP-only resume의 `defer_loading`, gateway `text/plain` 응답, MCP `list_changed` CPU 폭주, MCP OAuth 클라이언트 등록, tool search 단축 이름, Ctrl+O·Remote `/mcp`, Chrome ToolSearch 안내를 고쳤습니다.
- 교차 세션 메시지 미전달 흔적, compaction 후 백그라운드 명령 이중 기동, `/model` 캐시 경고, `/reload-skills` 불일치, 짧은 터미널의 `/resume`·`/continue` 목록, resume 파일-읽기 추적·1M 컨텍스트·artifacts 유실, 가상 드라이브(inode 0) 커스텀 로딩, 64MiB 초과 호스트 설정 유실·`--host-config-snapshot`, 로그아웃 후 스킬 정리, `/add-dir`·`!` 입력·`/hooks`·렌더·키 입력을 고쳤습니다.
- 터미널 렌더·기동, 훅·스피너 상태, 사용량 한도 시 dynamic workflow 일시정지, Remote Control 빈 세션, Chrome 연결 불가 안내, `claude mcp serve` 30초 progress, Foundry/AWS `alwaysLoad` MCP, Markdown artifact·Artifact 오류·감시(최대 10), PDF @-mention, `/mobile` QR, auto mode의 인라인 `!`·서브에이전트 hand-back·Monitor 기한, IDE selection pill, Pro 기본 workflow 크기, gateway/Bedrock/Vertex/Foundry의 잔여 claude.ai 로그인 갱신 중단, `claude-api` skill을 개선·변경했습니다.
- [VSCode] Attach Open File 설정, Hooks·Permission 저장·표시, SUBST/네트워크 드라이브 세션 이력, Active 필터, 새 채팅 되돌림, `CLAUDE_CONFIG_DIR` 반영, Windows 콘솔 깜빡임, 캐시 시계·auto-compact 툴팁, Hooks 저장 실패 팝업, 토글 색을 고치거나 바꿨습니다.
- [웹] 프로세스 종료 후 약 10분 무응답(메시지 전송 시 즉시 재시작), Routines 레이아웃(Yours/Templates), Cloud environments Custom network·기본 환경 표시를 넣거나 바꿨습니다.
- [Claude Tag] 스레드 활동으로 시간당 컨텍스트 리셋 방지, PR watch 재시작 후 CI·리뷰 알림 복구, 첫 메시지 삭제로 작업 종료, 다른 봇 대상 지시 무시, 바쁜 채널 카드 문구, Environment picker 라벨을 고치거나 개선했습니다.
- [Code Review] 대기 중 커밋 누락, 동일 소견 중복 게시, 해결된 보안 소견 재게시, 끝난 `/ultrareview` 재개를 고쳤습니다.
- Windows: temp 경로 260자에서 PowerShell이 빈 Exit code 1로 실패하던 문제를 고쳤습니다.
- `2.1.272`는 버그 수정·안정성 개선만 있습니다.

## CLI App

- 버전: `2.1.272` (이전: `2.1.270`)
- GUI와 동일 릴리스입니다. Remote 빠른 모드, 샌드박스 `allowed_domains`, `omitClaudeMd`, plugin `--accept-command`, 조직 정책·Bash·MCP·Remote·VS Code·웹·Claude Tag·Code Review 수정을 `2.1.271`에 담고, `2.1.272`는 안정성 패치입니다.

## Sources

- [Claude Code changelog](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
