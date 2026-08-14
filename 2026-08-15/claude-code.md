# Claude Code 변경사항

## GUI App

- 버전: `2.1.232` (이전: `2.1.231`)
- 다른 Claude 세션을 `@이름`으로 언급해 바로 메시지를 보낼 수 있고, 하위 에이전트 포크가 기본으로 켜졌습니다.
- 원격 제어 세션의 재연결·대화 복원과 음성 모드 연결 실패 안내를 개선했습니다.
- Windows와 PowerShell의 권한 우회 가능성을 막고, 중첩 Git 저장소마다 별도 신뢰 확인을 요구하도록 보안을 강화했습니다.

## CLI App

- 버전: `2.1.232` (이전: `2.1.231`)
- 이름만으로 실행 중인 세션에 메시지를 보내고, 대화·프롬프트 캐시를 이어받는 포크 에이전트를 기본으로 사용할 수 있습니다.
- MCP 서버 연결 실패 시 30초 동안 멈추는 현상과 클라우드 게이트웨이 로그인 오류 안내를 개선했습니다.
- 공식 변경 로그는 GUI와 CLI의 별도 빌드가 아닌 공통 Claude Code 릴리스로 게시합니다.

## Sources

- [Claude Code changelog](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
