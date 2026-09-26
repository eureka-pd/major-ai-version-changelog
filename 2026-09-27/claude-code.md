# Claude Code 변경사항

## GUI App

- 버전: `2.1.283` (이전: `2.1.282`)
- **2.1.283**: LLM 게이트웨이가 한 사용자 프롬프트의 요청을 묶을 수 있도록 `x-claude-code-prompt-id` 힌트 헤더를 추가했습니다(`CLAUDE_CODE_GATEWAY_HINT_HEADERS=1`). 관리 설정에 `availableModelsMatch: "exact"`와 `deniedModels`를 넣어 모델 허용·차단을 더 엄격히 제어할 수 있습니다. `/doctor prompt-audit`(및 `/checkup prompt-audit`)로 CLAUDE.md·스킬·에이전트·명령의 구형 프롬프트 패턴을 점검합니다. MCP·WebFetch·WebSearch 출력을 `tool.output` OpenTelemetry 이벤트에 넣을 수 있고, fullscreen에서 다른 세션의 잘린 메시지를 클릭해 펼칠 수 있습니다. 게이트웨이에 Bedrock Mantle upstream·로드 테스트 모드를 추가했고, MCP 진행 알림·플러그인 검증·vim·VS Code·Cloud·Claude Tag·Code Review 등 다수 수정과 UI 개선이 포함됩니다.

## CLI App

- 버전: `2.1.283`
- GUI와 동일합니다.

## Sources

- [Claude Code changelog](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
