# SUMMARY

오늘 새로 반영할 안정 버전은 Claude Code `2.1.190`과 Cursor `3.9`입니다. Codex와 Antigravity는 저장된 최신 기준과 같아서 중복 보고하지 않았습니다.

## Claude Code

### GUI App

- 최신 저장 기준을 `2.1.190`으로 올렸습니다.
- `2.1.190`은 별도 상세 항목 없이 버그 수정과 안정성 개선 릴리스로 공개되어 있습니다.
- `2.1.187`에서는 조직에서 제한한 모델을 model picker, `--model`, `/model`, `ANTHROPIC_MODEL`에서 더 명확히 막고 안내하도록 바뀌었습니다.
- fullscreen mode의 선택 메뉴에서 마우스 클릭을 지원하고, Ghostty의 Cmd+click URL 열기, `/btw` 이전 답변 이동, `/plugin` 정리 노출 같은 사용성 수정이 들어갔습니다.
- background jobs, channel 연결, subagent depth, leaked worktree registration, VS Code extension resume 같은 장시간 작업 안정성 문제가 다수 수정되었습니다.

### CLI App

- npm `@anthropic-ai/claude-code` latest도 `2.1.190`입니다. `next` 태그 `2.1.191`은 다음 채널이라 안정 버전 보고에는 포함하지 않았습니다.
- `sandbox.credentials` 설정이 추가되어 sandboxed command가 credential 파일이나 secret 환경변수를 읽지 못하게 막을 수 있습니다.
- `--resume`이 원래 `-p` 실행에서 모델 턴을 만들지 않았을 때 실패하던 문제를 고쳤습니다.
- `--json-schema`와 workflow `agent({schema})` 구조화 출력이 성공 후 무한 재호출되거나 후속 턴에서 불안정하던 문제가 수정되었습니다.
- remote MCP tool call이 5분 동안 응답 없이 멈추면 이제 계속 기다리지 않고 오류로 중단합니다.

## Codex

### GUI App

- 최신 앱 버전 저장 기준: `26.616`
- OpenAI Codex changelog의 최신 GUI 앱 항목도 `26.616` 기준입니다.
- Record & Replay, automation run history bulk action, local/remote thread handoff, SSH connection deep link, Browser Use 이동 안정성 개선 항목은 기존 최신 기준으로 유지됩니다.

### CLI App

- 최신 저장 기준: `0.142.0`
- npm `@openai/codex` latest 안정 태그도 `0.142.0`입니다.
- `alpha`는 `0.143.0-alpha.14`까지 올라왔지만 prerelease 채널이므로 이번 안정 버전 보고에는 포함하지 않았습니다.
- 공개 Codex changelog 기준 최신 CLI 안정 항목은 이미 전일 보고한 `0.142.0` 기준입니다.

### Mobile

- 최신 저장 기준: ChatGPT for iOS `1.2026.167`
- OpenAI Codex changelog의 최신 모바일 항목도 2026-06-22 `1.2026.167`입니다.

## Cursor

### GUI App

- 최신 저장 기준을 Cursor `3.9`, changelog date `2026-06-22`로 올렸습니다.
- 이번 릴리스의 핵심은 `Cursor Customize`입니다. 플러그인, skills, MCP, subagents, rules, commands, hooks를 한 화면에서 관리할 수 있게 되었습니다.
- 사용자, 팀, workspace 단위로 customization을 추가하고 관리할 수 있고, 자체 custom MCP도 쓸 수 있습니다.
- Marketplace leaderboard가 추가되어 팀에서 많이 쓰는 플러그인, skills, MCP를 더 쉽게 찾을 수 있습니다.
- plugin canvas가 추가되어 팀이 재사용할 수 있는 공유 설정 템플릿을 플러그인에서 제공할 수 있습니다.
- 팀 마켓플레이스는 GitLab, BitBucket, Azure DevOps의 플러그인 repository 가져오기를 지원합니다.

### CLI App

- CLI 전용 새 안정 버전 번호는 확인되지 않았습니다.
- 이번 Cursor `3.9` 항목은 Customize와 팀 마켓플레이스 중심의 GUI/제품 변경입니다.
- 별도 CLI baseline 변경이 없어 `.version`의 CLI 값은 계속 `null`로 유지합니다.

## Antigravity

### GUI App

- 최신 저장 기준: Antigravity 2.0 `2.1.4`
- 공식 changelog/release 표면은 raw HTML에 버전 본문을 직접 노출하지 않았지만, 공식 JS bundle의 download metadata에서 최신 GUI 다운로드가 계속 `2.1.4`로 확인되었습니다.
- quota screen redesign, PDF attachment support, `/btw`, conversation search, breadcrumbs, nested subagents, MCP server stability 관련 항목이 최신 기준으로 유지됩니다.

### IDE App

- 최신 저장 기준: Antigravity IDE `2.0.4`
- 공식 bundle metadata 기준 IDE 최신 버전도 기존 저장 기준과 같습니다.

### CLI App

- CLI는 Antigravity 2.0 제품군 기준으로 유지합니다.
- 별도 새 CLI 패치 버전 번호는 확인되지 않았습니다.

## Sources

- [Claude Code CHANGELOG](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [Claude Code raw CHANGELOG](https://raw.githubusercontent.com/anthropics/claude-code/main/CHANGELOG.md)
- [npm @anthropic-ai/claude-code](https://www.npmjs.com/package/@anthropic-ai/claude-code)
- [OpenAI Codex changelog](https://developers.openai.com/codex/changelog)
- [Cursor changelog](https://cursor.com/ko/changelog)
- [Google Antigravity changelog](https://antigravity.google/changelog)
- [Google Antigravity releases](https://antigravity.google/releases)
