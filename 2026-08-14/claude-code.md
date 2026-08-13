# Claude Code 변경사항

## GUI App

- 버전: `2.1.231` (이전: `2.1.228`)
- `2.1.229`에서 Remote Control 재개 안내, 자체 호스팅 서버 훅, Vertex·Bedrock 연결 유지 기능을 추가했습니다.
- 스트리밍 출력 중복·누락, 도구 호출 오류, 좁은 터미널과 Windows 경로 문제 등 작업 중단을 일으키던 문제를 수정했습니다.
- `2.1.231`에서는 Slack처럼 사전 등록한 OAuth 클라이언트가 MCP 로그인 중 리디렉션 URI 불일치로 실패하던 문제를 고쳤습니다.
- 공식 변경 로그는 GUI와 CLI의 별도 빌드가 아닌 공통 Claude Code 릴리스로 게시합니다.

## CLI App

- 버전: `2.1.231` (이전: `2.1.228`)
- 플러그인 마켓플레이스에 명령 기반 소스를 추가하고, 에이전트의 오프라인·클라우드 상태를 구분해 표시합니다.
- OAuth, GitHub 리뷰 게시, IDE 응답 멈춤, Remote Control 대기 표시를 개선해 명령줄 작업의 안정성을 높였습니다.
- `2.1.231`의 MCP OAuth 로그인 수정은 GUI와 CLI에 공통으로 적용되는 릴리스 항목입니다.

## Sources

- [Claude Code changelog](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
