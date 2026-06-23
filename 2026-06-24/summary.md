# SUMMARY

오늘 새로 반영할 안정 버전은 Claude Code `2.1.186`, Codex CLI `0.142.0`, Codex Mobile `1.2026.167`입니다. Cursor와 Antigravity는 저장된 최신 기준과 같아서 중복 보고하지 않았습니다.

## Claude Code

### GUI App

- 최신 저장 기준을 `2.1.186`으로 올렸습니다.
- MCP 로그인/로그아웃을 `/mcp` 메뉴 밖에서도 처리할 수 있게 되었고, `/workflows` 상세 화면에는 상태 필터가 추가되었습니다.
- `/plugin` Installed 탭에 Skills 섹션이 생겨 설치된 플러그인 안의 skill 구성을 더 쉽게 볼 수 있습니다.
- 배경 작업, subagent 화면, Chrome tab-group 격리, 권한 프롬프트, strikethrough 렌더링처럼 장시간 작업 중 눈에 띄던 UI/상태 표시 문제가 다수 수정되었습니다.

### CLI App

- npm `@anthropic-ai/claude-code` latest도 `2.1.186`입니다.
- `claude mcp login`과 `claude mcp logout`이 추가되어 SSH 환경에서도 브라우저 없이 MCP 인증 흐름을 진행할 수 있습니다.
- `!` bash 명령이 실행 결과에 대해 Claude가 바로 응답하도록 바뀌었습니다. 기존처럼 컨텍스트에만 넣고 싶으면 `respondToBashCommands: false`를 설정해야 합니다.
- `claude mcp get/remove`는 서버 이름 오타에 더 가까운 후보를 제안하고, 긴 서버 목록은 잘라 보여 줍니다.
- agent team에서 tmux/pane backend로 띄운 teammate가 leader의 `--effort` 값을 이어받도록 수정되었습니다.

## Codex

### GUI App

- 최신 앱 버전 저장 기준: `26.616`
- OpenAI Codex changelog의 최신 GUI 앱 항목도 `26.616` 기준입니다.
- Record & Replay, automation run history bulk action, local/remote thread handoff, SSH connection deep link, Browser Use 이동 안정성 개선 항목은 기존 최신 기준으로 유지됩니다.

### CLI App

- 최신 저장 기준을 `0.141.0`에서 `0.142.0`으로 올렸습니다.
- npm `@openai/codex` latest 안정 태그가 `0.142.0`으로 올라왔고, `alpha`는 `0.143.0-alpha.9`입니다.
- 공개 Codex changelog에는 2026-06-22 `0.142.0` 항목이 올라와 있습니다.
- 이번 CLI 변경은 주로 remote execution, plugin/skill 처리, app-server/exec-server 경계, path/cwd 처리, realtime routing, Windows sandbox, MCP sandbox metadata 같은 내부 실행 안정성 개선이 중심입니다.

### Mobile

- 최신 저장 기준을 ChatGPT for iOS `1.2026.160`에서 `1.2026.167`로 올렸습니다.
- 2026-06-22 항목이며, 모바일 앱 기준으로 새 버전 번호가 확인되어 중복 보고 방지용 `.version`에도 반영했습니다.

## Cursor

### GUI App

- 최신 저장 기준: Cursor `3.8`, changelog date `2026-06-18`
- 공식 changelog 최신 항목도 Cursor `3.8`입니다.
- `/automate` skill, Slack emoji trigger, GitHub automation trigger, computer use tool, automation 저장/PR 생성/memory file 관리 개선은 이미 반영된 최신 항목입니다.

### CLI App

- CLI 전용 새 안정 버전 번호는 확인되지 않았습니다.
- 최신 Cursor changelog 항목은 automation과 cloud Agent 중심의 제품 변경입니다.
- 별도 CLI baseline 변경이 없어 `.version`의 CLI 값은 계속 `null`로 유지합니다.

## Antigravity

### GUI App

- 최신 저장 기준: Antigravity 2.0 `2.1.4`
- 공식 changelog 검색 결과와 release/download 표면에서 확인되는 최신 안정 버전도 `2.1.4`입니다.
- quota screen redesign, PDF attachment support, `/btw`, conversation search, breadcrumbs, nested subagents, MCP server stability 관련 항목이 최신 기준으로 유지됩니다.

### IDE App

- 최신 저장 기준: Antigravity IDE `2.0.4`
- 공식 release/download 표면 기준의 IDE 최신 버전도 기존 저장 기준과 같습니다.

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
