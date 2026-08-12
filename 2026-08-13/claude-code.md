# Claude Code 변경사항

## GUI App

- 버전: `2.1.228` (이전: `2.1.227`)
- 화면이 드물게 갱신을 멈추는 문제와 `/tui`에서 모델 선택이 되돌아가는 문제를 수정했습니다.
- 대화 간 메시지 전달과 Remote Control 연결 문제를 고쳐 더 안정적으로 이어서 작업할 수 있게 했습니다.
- 공식 변경 로그는 이 릴리스를 GUI와 CLI의 별도 빌드로 구분하지 않습니다.

## CLI App

- 버전: `2.1.228` (이전: `2.1.227`)
- Windows에서 Git 저장소를 찾지 못하는 문제와 self-hosted runner 관련 문제를 수정했습니다.
- claude.ai 동기화 스킬이 로컬 명령이나 MCP 프롬프트를 가리지 못하도록 보호 기능을 강화했습니다.
- 위 변경사항은 공식 로그에 공통 Claude Code 릴리스로 게시되었습니다.

## Sources

- [Claude Code changelog](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
