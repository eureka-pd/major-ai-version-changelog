# Claude Code 변경사항

## GUI App

- 버전: `2.1.238` (이전: `2.1.237`)
- `keybindingFlavor`를 `"readline"`으로 두면 프롬프트에서 Ctrl+W가 Bash처럼 이전 공백까지 지웁니다. 기본 `"classic"`은 그대로입니다.
- 긴 대화에서 서브에이전트 도구 결과가 최근 표시 창을 벗어나면 해제되어 메모리 증가를 막고, 출력 스타일이 세션 중간에 기본 말투로 돌아가던 문제를 고쳤습니다.
- 전체화면에서 Ctrl+L·Cmd+K는 화면만 다시 그리며, 두 번 눌러 `/clear`하던 단축키는 제거되었습니다.

## CLI App

- 버전: `2.1.238` (이전: `2.1.237`)
- URL 마켓플레이스와 카탈로그 항목에 `headersHelper`를 추가해 카탈로그·같은 출처 아카이브 요청용 HTTP 헤더(단기 토큰 등)를 만들 수 있습니다. 설치·업데이트 시에만 실행되며 `-y` 또는 `[y/N]` 확인이 필요합니다.
- `claude self-hosted-runner`에 SIGTERM 후 세션을 유지하는 `--defer-shutdown-max-min`과 매 연결마다 `Proxy-Authorization`을 발급하는 `--proxy-authorization-command`/`--proxy-authorization-file`을 추가했습니다.
- Remote Control은 짧은 네트워크 끊김·403·로그인 갱신 지연을 더 잘 버티고, 크래시 후 재사용·모델 표시·메시지 유실을 고쳤습니다. MCP `headersHelper`는 해당 폴더 신뢰 대화가 필요하며 자격 증명 환경 변수를 상속하지 않습니다. 공식 로그는 GUI와 CLI의 별도 빌드가 아닌 공통 릴리스로 게시합니다.

## Sources

- [Claude Code changelog](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
