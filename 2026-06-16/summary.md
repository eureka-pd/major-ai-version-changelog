# SUMMARY

오늘 새로 보고할 안정 버전은 없습니다. Claude Code, Codex, Cursor, Antigravity 모두 `.version`에 저장된 최신 기준과 공식 changelog/패키지/다운로드 메타데이터 확인 결과가 일치합니다. 중복 보고를 막기 위해 `.version`은 `last_checked`만 `2026-06-16`으로 갱신했습니다.

## Claude Code

### GUI App

- 최신 저장 기준: `2.1.177`
- npm `@anthropic-ai/claude-code`의 `latest`와 `next` 태그도 `2.1.177`입니다.
- GitHub 공개 changelog의 최신 상세 항목은 아직 `2.1.176`입니다.
- `2.1.177`에 대한 새 공개 상세 설명은 아직 확인되지 않아 반복 보고하지 않았습니다.

### CLI App

- 최신 저장 기준: `2.1.177`
- CLI도 npm 최신 기준과 같습니다.
- 오늘은 session title, footer link badge, Bedrock credential caching, model allowlist enforcement, hook path matching, tmux clipboard, Remote Control, background session 관련 공개 상세가 추가로 바뀌지 않았습니다.

## Codex

### GUI App

- 최신 저장 기준: Codex app `26.609` (2026-06-11)
- 공식 changelog의 최신 앱 항목도 `26.609`입니다.
- 이미 기록한 rate-limit reset banking, referral invitation, Business workspace credit, browser/CDP debugging, `/init`, macOS Dock icon, Computer Use, onboarding, thread UI polish 항목이 최신입니다.

### CLI App

- 최신 저장 기준: Codex CLI `0.139.0` (2026-06-09)
- npm `@openai/codex`의 `latest` 태그도 `0.139.0`입니다.
- npm에는 `0.140.0-alpha.21` alpha 태그가 보이지만, 안정 버전이 아니므로 이번 보고 대상에서 제외했습니다.

### Mobile

- 최신 저장 기준: ChatGPT for iOS `1.2026.153` (2026-06-09)
- 공식 changelog의 최신 모바일 항목도 이 기준과 같습니다.
- 오늘 모바일 쪽 신규 안정 버전 변경은 없습니다.

## Cursor

### GUI App

- 최신 저장 기준: Cursor `3.7`, changelog date `2026-06-10`
- Cursor changelog 상단은 2026년 6월 10일 Bugbot 성능 개선 항목입니다.
- 이 항목은 이미 저장된 changelog date와 같으므로 새 버전으로 중복 보고하지 않았습니다.
- 2026년 6월 5일의 Cursor `3.7` 항목도 계속 최신 제품 버전 기준입니다.

### CLI App

- CLI 전용 새 안정 버전 번호는 확인되지 않았습니다.
- Cursor changelog는 `/review` 기반 Bugbot 실행에 대해 CLI 지원이 곧 추가될 예정이라고만 안내합니다.

## Antigravity

### GUI App

- 최신 저장 기준: Antigravity 2.0 `2.1.4` (2026-06-11)
- 공개 사이트 번들의 다운로드 메타데이터도 `2.1.4-6481382726303744`를 가리킵니다.
- changelog 데이터의 최신 Antigravity 2.0 항목도 `2.1.4`이며, quota screen redesign, PDF attachment support, `/btw`, conversation search, breadcrumbs, nested subagents 관련 항목이 최신입니다.

### IDE App

- 최신 저장 기준: Antigravity IDE `2.0.4` (2026-06-02)
- 공개 사이트 번들의 IDE 다운로드 메타데이터도 `2.0.4-6381998290370560`입니다.
- 최신 IDE changelog 항목은 enterprise account authentication blank screen fix입니다.

### CLI App

- CLI는 Antigravity 2.0 제품군 기준으로 유지합니다.
- CLI 설치 스크립트는 공개되어 있지만, 별도 새 패치 버전 번호는 확인되지 않았습니다.

## Sources

- [Claude Code CHANGELOG](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [npm @anthropic-ai/claude-code](https://www.npmjs.com/package/@anthropic-ai/claude-code)
- [OpenAI Codex changelog](https://developers.openai.com/codex/changelog)
- [npm @openai/codex](https://www.npmjs.com/package/@openai/codex)
- [Cursor changelog](https://cursor.com/ko/changelog)
- [Google Antigravity changelog](https://antigravity.google/changelog)
- [Google Antigravity download metadata](https://antigravity.google/download)
