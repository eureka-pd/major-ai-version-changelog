# Claude Code

오늘 Claude Code의 새 안정 버전 `2.1.186`이 확인되었습니다. `.version`에 저장된 `2.1.185` 이후 새로 보고할 변경입니다.

## GUI App

- 최신 저장 기준을 `2.1.186`으로 올렸습니다.
- MCP 로그인/로그아웃을 `/mcp` 메뉴 밖에서도 처리할 수 있게 되었고, `/workflows` 상세 화면에는 상태 필터가 추가되었습니다.
- `/plugin` Installed 탭에 Skills 섹션이 생겨 설치된 플러그인 안의 skill 구성을 더 쉽게 볼 수 있습니다.
- 배경 작업, subagent 화면, Chrome tab-group 격리, 권한 프롬프트, strikethrough 렌더링처럼 장시간 작업 중 눈에 띄던 UI/상태 표시 문제가 다수 수정되었습니다.

## CLI App

- npm `@anthropic-ai/claude-code` latest도 `2.1.186`입니다.
- `claude mcp login`과 `claude mcp logout`이 추가되어 SSH 환경에서도 브라우저 없이 MCP 인증 흐름을 진행할 수 있습니다.
- `!` bash 명령이 실행 결과에 대해 Claude가 바로 응답하도록 바뀌었습니다. 기존처럼 컨텍스트에만 넣고 싶으면 `respondToBashCommands: false`를 설정해야 합니다.
- `claude mcp get/remove`는 서버 이름 오타에 더 가까운 후보를 제안하고, 긴 서버 목록은 잘라 보여 줍니다.
- agent team에서 tmux/pane backend로 띄운 teammate가 leader의 `--effort` 값을 이어받도록 수정되었습니다.

## Sources

- [Claude Code CHANGELOG](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [npm @anthropic-ai/claude-code](https://www.npmjs.com/package/@anthropic-ai/claude-code)
