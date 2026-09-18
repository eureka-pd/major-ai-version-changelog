# Claude Code 변경사항

## GUI App

- 버전: `2.1.277` (이전: `2.1.274`)
- `2.1.275`–`2.1.277`을 반영했습니다. AGENTS.md(프로젝트에 CLAUDE.md가 없을 때)·게이트웨이 egress 경계(`CLAUDE_GATEWAY_PROXY_IS_EGRESS_BOUNDARY`)·업스트림 `headers:` 맵, 게이트웨이 로그인 시 계정 확인, 큐 일괄 전송(ctrl+enter), claude.ai 스킬·플러그인 동기화, `/plugin install --marketplace`를 넣었습니다.
- `ANTHROPIC_BASE_URL` 프록시에서 `advisor_20260301` 400이 나던 `2.1.275` 회귀(`2.1.276`), `claude -p`/SDK 내부 오류 후 행, 빈 text block으로 전 요청 실패, 구버전 CLI와 동시 실행 시 로그아웃, 잘못된 `customApiKeyResponses`/`theme`/`claudeAiMcpEverConnected`로 기동·`/mcp` 크래시, Grep/Glob 리소스 고갈 시 무일치 오보, Write가 디렉터리에 쓰려 할 때 silent decline, Edit의 `\uXXXX`·거대 non-ASCII 편집, null-byte 경로, `--bg`의 LSP stdin 종료로 세션 종료를 고쳤습니다.
- TaskOutput 도구를 제거하고 Read로 백그라운드 출력을 읽게 했으며, 서브에이전트 결과에 헤더·들여쓰기 표식, Bedrock/Vertex/Foundry의 sandbox·workflow 문구, Fable을 Anthropic API `/model`에 항상 표시하도록 바꿨습니다.
- [VSCode] 패널 Sign out·에이전트 맵의 백그라운드 셸/`/tasks`·Copy response/`/copy`·자동 아카이브 알림·Unarchive all, Vertex/Bedrock/Foundry/API 키의 비용·토큰을 Account & usage에 표시하고, General config·effort·Auto·`/fast` 기본값 유실을 고쳤습니다.
- [웹] Team/Enterprise 환경 선택기 Personal/Organization 구분·개인 환경 조직 공유, org 환경 읽기 전용 요약, Custom network에 도메인 필수, admin 라벨을 "Cloud sessions"로 바꿨습니다.
- [Claude Tag] Enterprise Grid 채널 루틴의 공개 채널 읽기, credential preset Learn more·Pylon EU 호스트, Google Cloud 키 폼·네트워크 이벤트 로그를 고쳤습니다.

## CLI App

- 버전: `2.1.277` (이전: `2.1.274`)
- GUI와 동일 릴리스입니다. AGENTS.md·게이트웨이 헤더/egress·`2.1.276` 프록시 회귀 수정·TaskOutput 제거·VS Code·웹·Tag 수정이 포함됩니다.

## Sources

- [Claude Code changelog](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
