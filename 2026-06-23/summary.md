# SUMMARY

오늘 새로 반영할 안정 버전은 없습니다. Claude Code, Codex, Cursor, Antigravity 모두 저장된 최신 기준과 같아서 중복 보고하지 않았습니다.

## Claude Code

### GUI App

- 최신 저장 기준: `2.1.185`
- 공식 changelog 최신 항목도 `2.1.185`입니다.
- API 응답 대기 안내 문구가 더 정확해지고, 표시 시점이 10초 침묵 후에서 20초 침묵 후로 조정된 항목이 최신 기준으로 유지됩니다.
- 이 변경은 실제 장애처럼 보일 수 있는 “응답 없음” 표현을 줄이고, 재시도 대기 상태를 더 분명히 보여 주는 UX 수정입니다.

### CLI App

- npm `@anthropic-ai/claude-code` latest는 `2.1.185`입니다.
- npm `next`에는 `2.1.186`이 있지만, 안정 기준인 `latest`는 저장 기준과 같습니다.
- CLI 관점에서도 새로 보고할 안정 변경사항은 없습니다.

## Codex

### GUI App

- 최신 앱 버전 저장 기준: `26.616`
- OpenAI Codex changelog의 최신 앱 항목도 `26.616`입니다.
- Record & Replay, automation run history bulk action, local/remote thread handoff, SSH connection deep link, Browser Use 이동 안정성 개선 항목이 최신 기준으로 유지됩니다.

### CLI App

- 최신 저장 기준: `0.141.0`
- npm `@openai/codex` latest 안정 태그도 `0.141.0`입니다.
- npm에는 `0.142.0-alpha.11` alpha 태그가 있지만 안정 버전 기준 보고 대상은 아닙니다.
- remote executor Noise relay, cross-platform remote execution 보존, plugin discovery 개선, TUI input prompt auto-resolve 항목은 이미 반영된 최신 안정 기준입니다.

### Mobile

- 최신 저장 기준: ChatGPT for iOS `1.2026.160`
- 새 모바일 버전 번호는 확인되지 않았습니다.

## Cursor

### GUI App

- 최신 저장 기준: Cursor `3.8`, changelog date `2026-06-18`
- 공식 changelog 최신 항목도 Cursor `3.8`입니다.
- `/automate` skill, Slack emoji trigger, GitHub automation trigger, computer use tool, automation 저장/PR 생성/memory file 관리 개선은 이미 반영된 최신 항목입니다.

### CLI App

- CLI 전용 새 안정 버전 번호는 확인되지 않았습니다.
- 최신 Cursor changelog 항목은 automation과 cloud Agent 중심의 제품 변경입니다.
- SDK 관련 항목은 실행 추적용 `requestId`, 로컬 실행 `wait()` 안정성, Python SDK `list_runs` 개선, `cursor-sdk` `0.1.6` 릴리스가 최신 기준으로 유지됩니다.

## Antigravity

### GUI App

- 최신 저장 기준: Antigravity 2.0 `2.1.4` (2026-06-11)
- 공식 changelog bundle의 최신 항목도 `2.1.4`입니다.
- quota screen redesign, PDF attachment support, `/btw`, conversation search, breadcrumbs, nested subagents, MCP server stability 관련 항목이 최신 기준으로 유지됩니다.

### IDE App

- 최신 저장 기준: Antigravity IDE `2.0.4` (2026-06-02)
- 공식 download/release bundle 기준의 IDE 최신 버전도 `2.0.4`입니다.

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
- [Google Antigravity releases](https://antigravity.google/releases)
