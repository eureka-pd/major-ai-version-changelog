# SUMMARY

오늘 새로 보고할 변화는 세 가지입니다. Claude Code가 `2.1.175`로 올라갔고, Codex app이 `26.609`로 올라갔으며, Antigravity 2.0이 `2.1.4`로 올라갔습니다. Cursor는 저장된 최신 기준과 일치했습니다.

## Claude Code

### GUI App

- 최신 기준: `2.1.175` (2026-06-12)
- 관리자가 허용한 모델 목록을 Default 모델까지 강하게 제한하는 `enforceAvailableModels` 설정이 추가되었습니다.
- `2.1.174`에서는 fullscreen mouse wheel acceleration 설정, `/model` picker 표시, Fable 5 billing banner, Bedrock GovCloud, background session provider 환경 변수 격리, skill hot-reload, VSCode `/usage` breakdown 등이 개선되었습니다.
- 핵심은 조직의 모델 정책이 더 정확히 적용되고, 모델 선택과 background 작업이 덜 헷갈리게 된 것입니다.

### CLI App

- 최신 기준: `2.1.175`
- npm 패키지도 `2.1.175`로 확인되었습니다.
- CLI 사용자는 관리형 모델 allowlist, fullscreen scroll 동작, background session 환경 변수 격리, Bedrock GovCloud, model picker 안정화의 영향을 받습니다.

## Codex

### GUI App

- 최신 기준: Codex app `26.609` (2026-06-11), ChatGPT for iOS `1.2026.153` (2026-06-09)
- Plus/Pro 사용자를 위한 rate-limit reset banking과 referral invitation이 추가되었습니다.
- Browser use용 Developer mode가 추가되어 performance, network, console, runtime error, page state를 더 깊게 디버깅할 수 있습니다.
- app composer에서 `/init`으로 project instructions를 만들 수 있고, macOS Dock icon customization, Enterprise Computer Use 확장, Windows per-app access control, Unread chats section이 추가되었습니다.
- Browser use 성능, plugin management, usage-limit 안내, scheduled automation approval mode, background agent, PR/commit message 생성, Codex Mobile QR pairing 등 여러 안정성 항목이 개선되었습니다.

### CLI App

- 최신 기준: Codex CLI `0.139.0` (2026-06-09)
- npm 기준도 `0.139.0`입니다.
- `0.140.0` 계열은 alpha 빌드만 확인되어 정식 버전으로 반복 보고하지 않았습니다.

## Cursor

### GUI App

- 최신 기준: `3.7`, changelog 날짜 `2026-06-10`
- 새 제품 버전 번호나 새 changelog 날짜는 확인되지 않았습니다.
- 2026-06-10 Bugbot 개선 항목은 이미 저장된 기준이라 반복 보고하지 않았습니다.

### CLI App

- CLI 전용 새 버전 번호는 확인되지 않았습니다.
- `/review` 관련 CLI 지원은 아직 "곧 추가" 상태입니다.

## Antigravity

### GUI App

- 최신 기준: Antigravity 2.0 `2.1.4` (2026-06-11), Antigravity IDE `2.0.4`
- Quota screen이 개편되어 사용한 credit과 남은 credit을 더 명확히 볼 수 있습니다.
- `/btw`로 현재 대화 context를 가진 임시 agent에게 옆질문을 보낼 수 있습니다.
- 대화 검색, PDF attachment, file viewer breadcrumbs, nested subagent 표시, Project 생성/정렬 UX가 개선되었습니다.
- LaTeX, MCP server 안정성, Chrome DevTools MCP server 문제 해결, `mcp_config.json` schema 호환성, sensitive path 인식도 개선되었습니다.

### CLI App

- CLI는 `2.0` 제품군 기준으로 유지합니다.
- CLI만의 별도 패치 번호는 오늘 확인되지 않았습니다.

## Sources

- [Claude Code CHANGELOG](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [npm @anthropic-ai/claude-code](https://www.npmjs.com/package/@anthropic-ai/claude-code)
- [OpenAI Codex changelog](https://developers.openai.com/codex/changelog)
- [npm @openai/codex](https://www.npmjs.com/package/@openai/codex)
- [Cursor changelog](https://cursor.com/ko/changelog)
- [Google Antigravity changelog](https://antigravity.google/changelog)
- [Google Antigravity releases](https://antigravity.google/releases)
