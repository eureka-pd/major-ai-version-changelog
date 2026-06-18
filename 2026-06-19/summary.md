# SUMMARY

오늘 새로 반영한 항목은 Codex CLI `0.141.0`과 Cursor의 2026-06-18 automation 개선입니다. Claude Code는 공개 changelog 상세 기준을 `2.1.181`로 맞췄고, Antigravity는 저장된 최신 기준과 일치합니다.

## Claude Code

### GUI App

- 최신 저장 기준: `2.1.181`
- 공개 changelog 상세 기준: `2.1.181`
- `/config key=value`로 prompt에서 설정을 바로 바꿀 수 있습니다.
- 긴 문단 streaming과 subagent panel 표시가 개선됐습니다.
- MCP OAuth browser page가 정리되고 성공 시 자동으로 닫힙니다.
- UI focus, AskUserQuestion, copy/paste, `/stats`, transcript cleanup 관련 문제가 수정됐습니다.

### CLI App

- 최신 저장 기준: `2.1.181`
- macOS sandbox의 Apple Events opt-in 설정과 `CLAUDE_CLIENT_PRESENCE_FILE` 환경변수가 추가됐습니다.
- bundled Bun runtime이 `1.4`로 올라갔습니다.
- thinking 중 API 연결이 끊겼을 때 자동 재시도합니다.
- provider, symlink, AWS credential, Linux clipboard, Windows/OneDrive 환경 관련 오류가 수정됐습니다.

## Codex

### GUI App

- 최신 앱 버전 저장 기준: `26.609`
- 새 GUI 앱 버전 번호는 확인되지 않았습니다.
- 2026-06-16 지역 제공 범위 공지는 기존 기준과 같습니다.

### CLI App

- 최신 저장 기준: `0.141.0`
- remote executor 통신에 인증된 end-to-end encrypted Noise relay channel이 적용됐습니다.
- 원격 실행에서 executor 쪽 working directory, shell, filesystem permission path를 더 정확히 보존합니다.
- 선택한 executor plugin의 stdio MCP server 활성화와 plugin discovery가 개선됐습니다.
- app-server, realtime client, TUI prompt auto-resolve 기능이 확장됐습니다.
- Windows sandbox, hook trust, plugin routing, SQLite WAL reset, enterprise proxy TLS 문제가 수정됐습니다.

### Mobile

- 최신 저장 기준: ChatGPT for iOS `1.2026.160`
- 새 모바일 버전 번호는 확인되지 않았습니다.

## Cursor

### GUI App

- 최신 저장 기준: Cursor `3.7`, changelog date `2026-06-18`
- `/automate` skill로 local agent session에서 자동화를 만들 수 있습니다.
- Slack emoji reaction과 GitHub event를 automation trigger로 사용할 수 있습니다.
- 실패한 GitHub Actions 처리와 PR 리뷰 댓글 자동 수정을 위한 marketplace template이 추가됐습니다.
- cloud Agent automation은 computer use tool을 기본으로 사용할 수 있습니다.
- automation 저장, PR 생성 기본값, memory file 관리가 개선됐습니다.

### CLI App

- CLI 전용 새 안정 버전 번호는 확인되지 않았습니다.
- 이번 항목은 Cursor automation과 cloud Agent 중심의 제품 변경입니다.

## Antigravity

### GUI App

- 최신 저장 기준: Antigravity 2.0 `2.1.4` (2026-06-11)
- 공식 사이트 bundle의 최신 항목도 `2.1.4`입니다.
- quota screen redesign, PDF attachment support, `/btw`, conversation search, breadcrumbs, nested subagents 관련 항목이 최신 기준으로 유지됩니다.

### IDE App

- 최신 저장 기준: Antigravity IDE `2.0.4` (2026-06-02)
- 공식 사이트 bundle의 IDE 최신 항목도 `2.0.4`입니다.

### CLI App

- CLI는 Antigravity 2.0 제품군 기준으로 유지합니다.
- 별도 새 CLI 패치 버전 번호는 확인되지 않았습니다.

## Sources

- [Claude Code CHANGELOG](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [npm @anthropic-ai/claude-code](https://www.npmjs.com/package/@anthropic-ai/claude-code)
- [OpenAI Codex changelog](https://developers.openai.com/codex/changelog)
- [OpenAI Codex GitHub releases](https://github.com/openai/codex/releases)
- [npm @openai/codex](https://www.npmjs.com/package/@openai/codex)
- [Cursor changelog](https://cursor.com/ko/changelog)
- [Google Antigravity changelog](https://antigravity.google/changelog)
- [Google Antigravity releases](https://antigravity.google/releases)
