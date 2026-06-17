# SUMMARY

오늘 새로 반영한 항목은 Claude Code와 Codex Mobile입니다. Claude Code는 npm 안정 기준이 `2.1.181`까지 올라갔고, 공개 changelog 상세 설명은 `2.1.179`까지 확인됩니다. Codex Mobile은 ChatGPT for iOS `1.2026.160`이 새 기준입니다. Cursor와 Antigravity는 저장된 최신 기준과 일치합니다.

## Claude Code

### GUI App

- 최신 저장 기준: `2.1.181`
- 공개 changelog 상세 기준: `2.1.179`
- 응답 스트리밍 중 연결이 끊겨도 부분 응답을 보존하도록 수정됐습니다.
- welcome 화면에서 여러 홍보 배너가 겹쳐 쌓이던 문제가 고쳐졌습니다.
- subagent 화면에서 Ctrl+O를 눌렀을 때 해당 subagent의 transcript가 제대로 보이지 않던 문제가 수정됐습니다.
- subagent/footer 패널에서 prompt 입력칸을 클릭했을 때 focus가 돌아오지 않던 문제도 고쳐졌습니다.

### CLI App

- 최신 저장 기준: `2.1.181`
- 공개 changelog 상세 기준: `2.1.179`
- WSL2의 Windows Terminal과 VS Code에서 mouse-wheel scrolling이 깨지던 회귀가 수정됐습니다.
- Linux에서 큰 디렉터리 트리를 대상으로 sandbox read glob을 걸면 Bash tool 설명이 지나치게 커지던 문제가 고쳐졌습니다.
- feedback survey가 한 자리 숫자 답변을 곧바로 세션 평점으로 잡아버리던 문제가 수정됐습니다.
- remote session의 background task 상태 표시와 plugin loading 성능이 개선됐습니다.

## Codex

### GUI App

- 최신 앱 버전 저장 기준: `26.609`
- 새 GUI 앱 버전 번호는 확인되지 않았습니다.
- 2026-06-16 지역 제공 범위 공지는 이미 저장 기준에 반영된 상태입니다.

### CLI App

- 최신 저장 기준: `0.140.0`
- npm `@openai/codex`의 `latest` 태그도 `0.140.0`입니다.
- `0.141.0-alpha.5` 계열 alpha 빌드는 pre-release라 안정 버전 보고 대상에는 넣지 않았습니다.

### Mobile

- 최신 저장 기준: ChatGPT for iOS `1.2026.160`
- workspace file browser와 workspace folder directory picker가 추가됐습니다.
- diff review에서 전체 diff를 펼치거나 접는 controls가 생겼습니다.
- MCP approval은 현재 chat에서만 허용할지, 여러 chat에 걸쳐 허용할지 선택할 수 있습니다.
- Codex message와 plan에서 LaTeX rendering이 지원됩니다.
- thread 상태 표시, pairing/onboarding, task recovery, reconnect 흐름이 더 안정적으로 개선됐습니다.

## Cursor

### GUI App

- 최신 저장 기준: Cursor `3.7`, changelog date `2026-06-10`
- Cursor changelog 상단은 2026년 6월 10일 Bugbot 성능 개선 항목입니다.
- 이 항목은 이미 `.version`의 기준일과 같으므로 중복 보고하지 않았습니다.
- 2026년 6월 5일의 Cursor `3.7` 디자인 모드 개선 항목도 계속 제품 버전 기준으로 남아 있습니다.

### CLI App

- CLI 전용 새 안정 버전 번호는 확인되지 않았습니다.
- 현재 changelog는 `/review` 기반 Bugbot 실행이 Cursor 3.7+와 `cursor.com/agents`에서 가능하고, CLI 지원은 곧 추가될 예정이라고 안내합니다.

## Antigravity

### GUI App

- 최신 저장 기준: Antigravity 2.0 `2.1.4` (2026-06-11)
- 공개 사이트 번들의 다운로드 링크도 `2.1.4`를 가리킵니다.
- quota screen redesign, PDF attachment support, `/btw`, conversation search, breadcrumbs, nested subagents 관련 항목이 최신 기준으로 유지됩니다.

### IDE App

- 최신 저장 기준: Antigravity IDE `2.0.4` (2026-06-02)
- 공개 사이트 번들의 IDE 다운로드 링크도 `2.0.4`를 가리킵니다.
- 최신 IDE 기준은 enterprise account authentication blank screen fix 항목 그대로입니다.

### CLI App

- CLI는 Antigravity 2.0 제품군 기준으로 유지합니다.
- 별도 새 CLI 패치 버전 번호는 확인되지 않았습니다.

## Sources

- [Claude Code CHANGELOG](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [npm @anthropic-ai/claude-code](https://www.npmjs.com/package/@anthropic-ai/claude-code)
- [OpenAI Codex changelog](https://developers.openai.com/codex/changelog)
- [npm @openai/codex](https://www.npmjs.com/package/@openai/codex)
- [Cursor changelog](https://cursor.com/ko/changelog)
- [Google Antigravity changelog](https://antigravity.google/changelog)
- [Google Antigravity download](https://antigravity.google/download)
