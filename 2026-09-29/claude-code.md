# Claude Code 변경사항

## GUI App

- 버전: `2.1.284` (이전: `2.1.283`)
- **2.1.284**: 기본 Sonnet을 Claude Sonnet 5.5(`claude-sonnet-5-5`)로 올렸습니다(1M 컨텍스트, $2/$10 per Mtok·캐시 읽기 $0.20/Mtok). auto mode에서 작업 디렉터리 밖 읽기에 "Yes, but ask again next time"을 추가했고, Claude apps gateway 사용 한도를 `/usage`·상태줄에 달러로 표시합니다. `/mcp reconnect all`, effort 슬라이더 키바인딩(`effortSlider:*`·`toggleUltracode`), Ultracode를 `/effort`의 독립 토글로 분리했으며, 권한 모드를 정하지 않으면 대화형 세션이 auto mode로 시작합니다. 손상된 응답 스트림·과부하 재시도·compaction 후 Prompt too long·MCP 재개 대기·플러그인·vim·VS Code·Cloud·Claude Tag·Code Review 등 다수 수정·개선이 포함됩니다.

## CLI App

- 버전: `2.1.284`
- GUI와 동일합니다.

## Sources

- [Claude Code changelog](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
