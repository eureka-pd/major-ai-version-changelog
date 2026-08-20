# Claude Code 변경사항

## GUI App

- 버전: `2.1.237` (이전: `2.1.235`)
- 결과부터 보여주는 내장 Concise 출력 스타일을 `/config`의 Output style에서 고를 수 있습니다.
- 같은 기기의 다른 세션이 다음으로 유휴해질 때 한 번만 알려 달라는 `notify_when_idle`을 교차 세션 `SendMessage`에 추가했습니다.
- VS Code 트랜스크립트 스크린 리더를 지원하고, 전체화면 렌더러가 한 번 실패해도 클래식 렌더러로 넘어가게 고쳤습니다.

## CLI App

- 버전: `2.1.237` (이전: `2.1.235`)
- `ANTHROPIC_DEFAULT_MODEL`로 새 세션 기본 모델을 정하고, LLM 게이트웨이·커스텀 base URL 세션의 프롬프트 캐시를 고쳤습니다.
- macOS 샌드박스에서 `**/.env` 같은 읽기 거부 와일드카드가 허용 영역 안에서도 우선하며, 이름을 바꿔도 우회되지 않습니다.
- 슬래시 명령 오타는 퍼지 실행 대신 오류를 내고, Remote Control은 CLI가 끝나면 수 초 안에 오프라인으로 표시합니다. 공식 로그는 GUI와 CLI의 별도 빌드가 아닌 공통 릴리스로 게시합니다.

## Sources

- [Claude Code changelog](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
