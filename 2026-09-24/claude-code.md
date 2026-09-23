# Claude Code 변경사항

## GUI App

- 버전: `2.1.281` (이전: `2.1.280`)
- Claude apps gateway에 Bedrock `assume_role`(STS로 다른 계정 IAM 역할 가정)·`guardrail`·`telemetry.resource_attributes`를 추가했습니다. 최신 Claude Desktop 키용 `desktop` 정책 블록도 지원합니다.
- `settings.json`에 `"attribution": false`를 두면 커밋·PR 기여 표시를 숨깁니다. MCP URL 모드 elicitation, `claude plugin validate`의 MCP 검사, `/insights`의 auto mode 권장, 전체 화면 Installed 목록 스크롤바를 추가했습니다.
- 재시도·재개·프롬프트 캐시·MCP 연결·권한·플러그인·VSCode·클라우드·Claude Tag·Code Review 등 다수 수정·개선이 포함됩니다.

## CLI App

- 버전: `2.1.281` (이전: `2.1.280`)
- GUI와 동일 릴리스입니다. 게이트웨이·세션 재개·MCP·권한·플러그인 관련 수정이 포함됩니다.

## Sources

- [Claude Code changelog](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
