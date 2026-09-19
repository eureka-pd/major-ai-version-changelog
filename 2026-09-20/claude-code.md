# Claude Code 변경사항

## GUI App

- 버전: `2.1.278` (이전: `2.1.277`)
- Claude API·Enterprise와 Bedrock·Vertex·Foundry·게이트웨이에서 auto mode가 서버 측 분류기를 기본으로 쓰도록 바뀌었습니다. 분류기 오버헤드 과금이 없고, Bedrock·Vertex·Foundry·게이트웨이에서는 `CLAUDE_CODE_AUTO_MODE_SERVER=0`으로 끌 수 있으며, 과금 폴백 시 경고합니다. 안내: https://code.claude.com/docs/en/auto-mode-classifier-billing
- `/status`에 이 세션의 auto mode 분류기가 서버에서 도는지 보여주는 `Auto mode server` 행을 추가했습니다.

## CLI App

- 버전: `2.1.278` (이전: `2.1.277`)
- GUI와 동일 릴리스입니다. 서버 측 auto mode 분류기 기본화와 `/status` 행이 포함됩니다.

## Sources

- [Claude Code changelog](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
