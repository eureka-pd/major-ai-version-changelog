# Codex

오늘 Codex는 모바일 앱 기준만 새로 반영했습니다. Codex app `26.609`와 Codex CLI `0.140.0`은 기존 저장 기준과 같습니다.

## GUI App

- 최신 앱 버전 저장 기준: `26.609`
- 새 GUI 앱 버전 번호는 확인되지 않았습니다.
- 공식 changelog 상단의 2026-06-16 지역 제공 범위 공지는 이미 저장 기준에 반영된 상태입니다.
- EEA, UK, Switzerland의 Computer Use, Chrome extension, Memories, Chronicle 제공 범위도 기존 기준과 같습니다.

## CLI App

- 최신 저장 기준: `0.140.0`
- npm `@openai/codex`의 `latest` 태그도 `0.140.0`입니다.
- `0.141.0-alpha.5` 계열 alpha 빌드가 보이지만 pre-release라 안정 버전 보고 대상에는 넣지 않았습니다.

## Mobile

- 최신 저장 기준: ChatGPT for iOS `1.2026.160`
- 공식 changelog 기준 2026-06-15에 `1.2026.160`이 올라왔습니다.
- workspace file browser가 추가되어 파일을 미리 보고 workspace path를 prompt에 연결할 수 있습니다.
- 새 thread를 시작할 때 workspace folder를 고르는 directory picker가 추가됐습니다.
- diff review에서 전체 diff를 한 번에 펼치거나 접는 controls가 생겼습니다.
- MCP approval은 현재 chat에서만 허용할지, 여러 chat에 걸쳐 허용할지 선택할 수 있습니다.
- Codex message와 plan에서 LaTeX rendering이 지원됩니다.
- running thread, queued prompt, side chat, subagent 상태 표시와 pairing/onboarding 흐름이 더 안정적으로 개선됐습니다.

## Sources

- [OpenAI Codex changelog](https://developers.openai.com/codex/changelog)
- [npm @openai/codex](https://www.npmjs.com/package/@openai/codex)
