# Claude Code

## GUI App

- Claude Code 공통 최신 기준이 `2.1.218`에서 `2.1.219`로 올라갔습니다.
- GUI 전용으로 따로 구분된 추가 release는 확인되지 않았습니다.

## CLI App

- 기본 Opus 모델이 100만 토큰 문맥을 지원하는 Claude Opus 5로 바뀌었습니다.
- 샌드박스 명령은 허용 목록 밖의 네트워크 연결을 막도록 설정할 수 있습니다.
- 작업 중 새 프로젝트 폴더를 추가했을 때 알림 hook을 실행하고, 하위 에이전트가 더 깊게 다른 에이전트를 시작할 수 있습니다.
- MCP 연결 오류에는 HTTP 상태와 원인이 표시되며, 설정값의 앞뒤 공백도 경고합니다.
- 출력 유실, Windows Git Bash 경로, 화면 읽기, Vim 모드, 원격 제어 상태 등의 오류가 수정됐습니다.

## Sources

- [Claude Code CHANGELOG](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [Claude Code raw CHANGELOG](https://raw.githubusercontent.com/anthropics/claude-code/main/CHANGELOG.md)
