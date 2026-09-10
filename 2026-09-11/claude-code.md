# Claude Code 변경사항

## GUI App

- 버전: `2.1.267` (이전: `2.1.266`)
- `maxEffortLevel` 설정으로 제공자별(Bedrock·Vertex·Foundry 포함) effort 상한을 두고, 사용자는 그보다 낮은 값만 고를 수 있습니다.
- `--system-prompt-snapshot off`로 매 요청마다 시스템 프롬프트를 새로 그릴 수 있어, 프롬프트 문구를 반복 시험하기 쉽습니다.
- 관리 설정이 샌드박스를 강제하는 조직에서 Cowork 클라우드 예약 작업이 기동에 실패하던 문제, 모바일에서 `/context` 등 로컬 명령 출력이 비던 문제를 고쳤습니다.
- 에이전트 뷰 안에서 tmux·ssh 재연결 뒤 shift+enter·option+backspace, 전체화면에서 스크롤 시 흐린 마지막 프롬프트 헤더, Workflow `agent()` 큰 output schema의 auto mode 거부를 고쳤습니다.
- 마켓플레이스 경로 백슬래시 우회, 호스트 앱의 만료된 AWS·GCP 자격 증명 재인증 안내, `-p --resume` 뒤 가짜 Continue 턴, 5MB 넘는 트랜스크립트 resume 시 병렬 도구·훅 유실을 고쳤습니다.
- 읽기 불가한 managed `allowedHttpHookUrls`·`httpHookAllowedEnvVars`·`allowedChannelPlugins`가 전부 허용되던 문제를 아무것도 허용하지 않도록 바꿨고, gateway 강제 `/login`에서 Esc가 닫히게 고쳤습니다.
- 아티팩트 업로드가 중간에 끊기면 미완료일 때 한 번 재시도하고, `effort:` 프론트매터 무시(Opus 4.7·4.8·Fable 5), UTF-8이 아닌 페이지 파일의 불친절한 오류를 고쳤습니다.
- `claude agents` `@` 메뉴가 세션 중 새 저장소를 못 보던 문제, Remote Control 권한 모드 잔상, `claude remote-control` 자격 만료 시 전체 세션 드롭, 사용량 한도 경고 깜빡임을 고쳤습니다.
- MCP·플러그인 도구가 바뀌거나 사라질 때 도구 목록을 다시 써서 이전 thinking·프롬프트 캐시가 깨지던 여러 경로를 고쳤고, ToolSearch 없는 세션의 중도 추가 도구는 지연 정의로 받습니다.
- `/model` 전환·resume·claude.ai 커넥터 재연결·`-p` 대화의 대화형 resume에서 프롬프트 캐시 미스와 extended thinking 유실을 줄였습니다.
- `/diff` 패널 깜빡임, Bash·샌드박스 안내 문구, 많은 Bash 호출 세션의 `--resume` 첫 렌더, 입력 반응성, `--system-prompt`·서브에이전트 캐시 안정성, Artifact publish 거절 메시지를 개선했습니다.
- Self-hosted runner의 `--use-anthropic-git-proxy` 보고 방식과 Gateway `forward_user_identity`의 429 페일오버 동작을 바꿨습니다.
- [VSCode] 순환 parent 링크 트랜스크립트의 100% CPU, WSL2 스크린샷 붙여넣기, diff 다크 테마 고정, RTL 입력 순서, CRLF diff accept, 공백 경로 @-mention, Remote-SSH 세션 목록, 과도한 ripgrep을 고쳤습니다.
- [웹] GitHub Enterprise 토큰 만료 후 연결 끊김 표시, GitHub App 없는 org의 `gh`/API 호출이 연결된 계정을 쓰게 고쳤습니다.
- [Claude Tag] 커스텀 커넥터 링크, 크레딧 소진 안내, 채널 최상위 메시지 수정·삭제 라우팅, Tool access Connect 실패를 고쳤습니다.

## CLI App

- 버전: `2.1.267` (이전: `2.1.266`)
- GUI와 동일 릴리스입니다. effort 상한, 시스템 프롬프트 스냅샷 옵션, 프롬프트 캐시·Remote Control·MCP·VS Code·Claude Tag 수정을 포함합니다.

## Sources

- [Claude Code changelog](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
