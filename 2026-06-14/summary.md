# SUMMARY

오늘 새로 보고할 변화는 Claude Code 하나입니다. npm 패키지는 `2.1.177`까지 올라왔고, 요청된 GitHub changelog 페이지에는 `2.1.176` 상세 변경 내용까지 공개되어 있습니다. Codex, Cursor, Antigravity는 저장된 최신 기준과 같아서 반복 보고하지 않았습니다.

## Claude Code

### GUI App

- 최신 기준: npm package `2.1.177` (2026-06-13)
- changelog 공개 기준: `2.1.176`
- `2.1.177`은 npm에는 올라왔지만 GitHub changelog 상세 항목은 아직 확인되지 않았습니다.
- `2.1.176`에서는 session title이 대화 언어에 맞춰 생성되고, footer link badge regex 설정이 추가되었습니다.
- Bedrock credential caching, 모델 allowlist enforcement, Fable 5 auto mode, hook path 조건, Linux sandbox, tmux/SSH clipboard, Remote Control, `/cd`, background session, Windows daemon, cloud session 인증 문제가 개선되었습니다.
- 핵심은 모델 정책 우회 가능성을 줄이고, remote/background 작업과 터미널 환경에서 생기던 상태 불일치를 줄인 것입니다.

### CLI App

- 최신 기준: `2.1.177`
- CLI 사용자는 `availableModels` enforcement, Bedrock credential caching, hook path matching, tmux clipboard, `/cd`, background session, Remote Control 관련 수정의 영향을 받습니다.
- 운영 조직에서는 허용 모델 정책이 더 정확히 적용되고, 원격/백그라운드 세션이 덜 헷갈리게 됩니다.

## Codex

### GUI App

- 최신 기준: Codex app `26.609` (2026-06-11), ChatGPT for iOS `1.2026.153` (2026-06-09)
- 저장된 기준과 같아서 새로 보고하지 않았습니다.

### CLI App

- 최신 기준: Codex CLI `0.139.0` (2026-06-09)
- npm 기준도 `0.139.0`입니다.
- `0.140.0` 계열은 alpha 빌드만 확인되어 정식 버전으로 반복 보고하지 않았습니다.

## Cursor

### GUI App

- 최신 기준: `3.7`, changelog 날짜 `2026-06-10`
- 최신 Bugbot 개선 항목은 이미 저장된 기준이라 반복 보고하지 않았습니다.

### CLI App

- CLI 전용 새 버전 번호는 확인되지 않았습니다.

## Antigravity

### GUI App

- 최신 기준: Antigravity 2.0 `2.1.4` (2026-06-11), Antigravity IDE `2.0.4`
- 저장된 기준과 같아서 새로 보고하지 않았습니다.

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
