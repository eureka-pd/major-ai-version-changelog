# SUMMARY

오늘 새로 반영할 안정 버전은 Claude Code `2.1.191`과 Codex CLI `0.142.2`입니다. Cursor와 Antigravity는 저장된 최신 기준과 같아서 중복 보고하지 않았습니다.

## Claude Code

### GUI App

- 최신 저장 기준을 `2.1.191`로 올렸습니다.
- `/clear` 이전 시점으로 대화를 되돌려 이어갈 수 있는 `/rewind` 지원이 추가되었습니다.
- 스트리밍 응답을 읽는 중 화면이 맨 아래로 튀는 문제와, tasks panel에서 멈춘 background agent가 다시 살아나는 문제가 수정되었습니다.
- 조직 정책으로 `/voice`가 비활성화된 경우 이제 단순 오류가 아니라 정책 제한임을 더 명확히 안내합니다.
- agent panel 스크롤, welcome splash 화면 overflow, Ghostty fullscreen Cmd+click URL 열기 같은 터미널 UI 문제가 수정되었습니다.
- 스트리밍 텍스트 업데이트를 100ms 단위로 묶어 CPU 사용량을 약 37% 줄였고, 긴 세션에서 terminal output cache로 메모리가 커지는 문제도 줄였습니다.

### CLI App

- npm `@anthropic-ai/claude-code`의 `latest` 기본 설치 버전도 `2.1.191`입니다. `next`도 같은 버전을 가리킵니다.
- comma-separated hook matcher 예: `"Bash,PowerShell"`가 조용히 동작하지 않던 문제가 수정되었습니다.
- `/permissions`의 Recently-denied 탭에서 거부 항목을 승인해도 닫을 때 사라지던 문제가 수정되었습니다.
- MDM 또는 file policy로 설정한 `forceRemoteSettingsRefresh`가 실제로 적용되고, stale proxy cache를 피하도록 설정 fetch에 `Cache-Control: no-cache`가 붙습니다.
- sandbox network permission dialog에서 한 번 허용한 host는 같은 세션 동안 다시 묻지 않도록 개선되었습니다.
- MCP server capability discovery, MCP OAuth discovery/token request가 일시적 네트워크 오류에서 짧게 재시도하도록 개선되었습니다.
- MCP HTTP 404 오류는 이제 URL과 MCP config 확인 안내를 같이 보여줍니다.

## Codex

### GUI App

- 최신 앱 버전 저장 기준: `26.616`
- OpenAI Codex changelog의 최신 GUI 앱 항목도 `26.616` 기준입니다.
- Record & Replay, automation run history bulk action, local/remote thread handoff, SSH connection deep link, Browser Use 이동 안정성 개선 항목은 기존 최신 기준으로 유지됩니다.

### CLI App

- 최신 저장 기준을 `0.142.2`로 올렸습니다.
- npm `@openai/codex`의 `latest` 안정 태그가 `0.142.0`에서 `0.142.2`로 올라갔습니다.
- platform별 stable 태그도 `0.142.2-linux-x64`, `0.142.2-darwin-arm64`, `0.142.2-win32-x64`처럼 `0.142.2` 계열로 맞춰져 있습니다.
- `alpha`는 `0.143.0-alpha.22`까지 올라왔지만 prerelease 채널이므로 안정 버전 보고에는 포함하지 않았습니다.
- 공개 Codex changelog에는 이번 CLI 패치의 상세 항목이 별도 노출되지 않아, 이번 보고는 npm stable version 기준 갱신으로 기록합니다.

### Mobile

- 최신 저장 기준: ChatGPT for iOS `1.2026.167`
- OpenAI Codex changelog의 최신 모바일 항목도 2026-06-22 `1.2026.167`입니다.

## Cursor

### GUI App

- 최신 저장 기준: Cursor `3.9`
- 최신 changelog 항목도 2026-06-22 `3.9`입니다.
- `Cursor Customize`에서 플러그인, skills, MCP, subagents, rules, commands, hooks를 한 화면에서 관리하는 변경은 기존 최신 기준으로 유지됩니다.
- Marketplace leaderboard, plugin canvas, GitLab/BitBucket/Azure DevOps 플러그인 repository 가져오기 지원도 기존 최신 기준입니다.

### CLI App

- CLI 전용 새 안정 버전 번호는 확인되지 않았습니다.
- 별도 CLI baseline 변경이 없어 `.version`의 CLI 값은 계속 `null`로 유지합니다.

## Antigravity

### GUI App

- 최신 저장 기준: Antigravity 2.0 `2.1.4`
- 공식 releases 검색 결과에서도 Antigravity 2.0 최신 버전은 `2.1.4`로 확인됩니다.
- quota screen redesign, PDF attachment support, `/btw`, conversation search, breadcrumbs, nested subagents, MCP server stability 관련 항목이 최신 기준으로 유지됩니다.

### IDE App

- 최신 저장 기준: Antigravity IDE `2.0.4`
- 공식 release 표면에서 `.version` 이후 새 IDE 버전은 확인되지 않았습니다.

### CLI App

- CLI는 Antigravity 2.0 제품군 기준으로 유지합니다.
- 별도 새 CLI 패치 버전 번호는 확인되지 않았습니다.

## Sources

- [Claude Code CHANGELOG](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [Claude Code raw CHANGELOG](https://raw.githubusercontent.com/anthropics/claude-code/main/CHANGELOG.md)
- [npm @anthropic-ai/claude-code](https://www.npmjs.com/package/@anthropic-ai/claude-code)
- [OpenAI Codex changelog](https://developers.openai.com/codex/changelog)
- [npm @openai/codex](https://www.npmjs.com/package/@openai/codex)
- [Cursor changelog](https://cursor.com/ko/changelog)
- [Google Antigravity changelog](https://antigravity.google/changelog)
- [Google Antigravity releases](https://antigravity.google/releases)
