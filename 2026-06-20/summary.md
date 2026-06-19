# SUMMARY

오늘 새로 반영한 항목은 Claude Code `2.1.183`, Codex app `26.616`, Cursor `3.8`입니다. Codex CLI는 안정 버전 `0.141.0` 그대로이고, Antigravity는 저장된 최신 기준과 일치합니다.

## Claude Code

### GUI App

- 최신 저장 기준: `2.1.183`
- 이전 저장 기준: `2.1.181`
- auto mode에서 사용자가 로컬 작업 삭제를 요청하지 않았을 때 `git reset --hard`, `git checkout -- .`, `git clean -fd`, `git stash drop` 같은 명령을 막습니다.
- 모델이 deprecated 되었거나 새 모델로 자동 치환될 때 경고를 보여줍니다.
- `/config --help`가 추가되어 `/config key=value`로 바꿀 수 있는 shorthand key를 확인할 수 있습니다.
- `/config` 토글과 startup setup issues 안내가 정리됐습니다.
- subagent WebSearch, skill autocomplete, thinking-only response 처리 문제가 수정됐습니다.

### CLI App

- 최신 저장 기준: `2.1.183`
- print mode(`-p`)에서도 deprecated model 또는 자동 모델 변경 경고가 stderr로 표시됩니다.
- `attribution.sessionUrl` 설정으로 web 또는 Remote Control session에서 commit/PR에 claude.ai session link를 넣지 않도록 할 수 있습니다.
- subagent spawn, Windows Terminal fullscreen TUI, tmux teammate pane, scheduled task/webhook trigger 처리 문제가 수정됐습니다.

## Codex

### GUI App

- 최신 앱 버전 저장 기준: `26.616`
- 이전 앱 버전 저장 기준: `26.609`
- macOS Record & Replay가 추가되어 사용자가 직접 보여준 작업 흐름을 재사용 가능한 skill로 바꿀 수 있습니다.
- automation run history에 bulk action이 추가되어 여러 run을 한 번에 읽음 처리하거나 archive할 수 있습니다.
- SSH connection deep link와 Browser Use session 이동 안정성이 개선됐습니다.

### CLI App

- 최신 저장 기준: `0.141.0`
- npm `@openai/codex`의 latest 안정 태그도 `0.141.0`입니다.
- `0.142.0-alpha.4`까지 prerelease가 보이지만 안정 버전이 아니므로 이번 보고 기준에는 포함하지 않았습니다.

### Mobile

- 최신 저장 기준: ChatGPT for iOS `1.2026.160`
- 새 모바일 버전 번호는 확인되지 않았습니다.

## Cursor

### GUI App

- 최신 저장 기준: Cursor `3.8`, changelog date `2026-06-18`
- 이전 저장 기준: Cursor `3.7`, changelog date `2026-06-18`
- `/automate` skill로 local agent session에서 자연어로 자동화를 만들 수 있습니다.
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
- 공식 release endpoint의 최신 항목도 `2.1.4`입니다.
- quota screen redesign, PDF attachment support, `/btw`, conversation search, breadcrumbs, nested subagents 관련 항목이 최신 기준으로 유지됩니다.

### IDE App

- 최신 저장 기준: Antigravity IDE `2.0.4` (2026-06-02)
- 공식 release endpoint의 IDE 최신 항목도 `2.0.4`입니다.

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
