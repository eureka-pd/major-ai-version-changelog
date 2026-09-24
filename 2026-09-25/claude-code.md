# Claude Code 변경사항

## GUI App

- 버전: `2.1.282` (이전: `2.1.281`)
- 넓은 터미널에서 본문만 폭을 제한하는 `maxProseWidth` 설정을 추가했습니다. 표·코드 블록은 전체 폭을 유지합니다.
- 프로젝트 설정에서 무시되거나 텔레메트리를 끈 변수를 시작 알림·`/status`·`claude doctor`에 표시합니다.
- 관리형 `managed-mcp.json`과 함께 `claude --chrome`을 허용하는 `allowClaudeInChromeWithManagedMcp`를 추가했습니다.
- Claude apps gateway에 `store.readiness_grace_seconds`를 넣어 Postgres 짧은 장애(페일오버 등) 동안 `/readyz`가 준비 상태를 유지할 수 있습니다.
- 전체 화면 `/feedback` 초안 목록에 마우스 오버 시 스크롤바를 추가했습니다.
- 웹 검색 복호화 불가·재개 시 메시지 변형·확장 thinking 유실·`redacted_thinking` 오류·compaction 거부·Fable 크레딧 프롬프트·로그인 갱신 경합·권한·플러그인·vim·VSCode·클라우드·Claude Tag 등 다수 수정을 포함합니다.

## CLI App

- 버전: `2.1.282` (이전: `2.1.281`)
- GUI와 동일 릴리스입니다. 본문 폭·텔레메트리 표시·Chrome+managed MCP·게이트웨이 readiness·재개·thinking·권한 관련 수정이 포함됩니다.

## Sources

- [Claude Code changelog](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
