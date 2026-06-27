# SUMMARY

오늘 새로 반영할 기준은 Claude Code `2.1.195`와 Codex CLI `0.142.3`입니다. Cursor와 Antigravity는 저장된 최신 기준과 같아서 중복 보고하지 않았습니다.

## Claude Code

### GUI App

- 최신 저장 기준을 `2.1.195`로 올렸습니다.
- fullscreen mode에서 mouse click, drag, hover만 끄고 wheel scroll은 유지할 수 있는 `CLAUDE_CODE_DISABLE_MOUSE_CLICKS` 설정이 추가되었습니다.
- macOS voice dictation이 기본 입력 장치 변경 후 긴 세션에서 무음을 잡던 문제가 수정되었습니다.
- Japanese, Chinese, Thai처럼 공백 없이 쓰는 언어에서 voice dictation auto-submit이 동작하지 않던 문제가 수정되었습니다.
- crashed background task를 다시 열 때 최대 5초 동안 blank screen이 보이던 문제가 수정되었습니다.
- background agent daemon의 control socket 시작 실패가 restart를 막던 문제가 수정되었습니다.
- `claude agents` 완료 목록이 작은 터미널에서도 더 많은 세션을 보여주도록 개선되었습니다.
- Remote session 시작 중 provisioning checklist를 보여주도록 개선되었습니다.

### CLI App

- npm `@anthropic-ai/claude-code`의 기본 `latest` 설치 버전은 `2.1.195`입니다.
- `next` 태그도 `2.1.195`를 가리킵니다.
- npm의 별도 `stable` 태그는 아직 `2.1.181`에 머물러 있지만, 이 저장소의 기준은 기존처럼 기본 설치 경로인 `latest`를 따릅니다.
- hyphen이 들어간 hook matcher가 의도치 않게 substring match 되던 문제가 수정되어 이제 정확히 일치해야 합니다. 예를 들어 hyphenated MCP 서버 전체를 잡으려면 `mcp__brave-search__.*`처럼 써야 합니다.
- project `.claude/settings.json`만으로 활성화된 external plugin이 일부 loader path에서 설치 동의를 반복 요구하던 문제가 수정되었습니다.
- `/plugin` Enable/Disable이 plugin manifest 이름과 marketplace 이름이 다를 때 동작하지 않던 문제가 수정되었습니다.
- newer Claude Code가 쓴 background job이 `claude agents`에서 사라지거나 데이터를 잃던 문제가 수정되었습니다.
- Linux voice mode는 SoX가 설치되어 있지만 capture device가 없을 때와 SoX 자체가 없을 때를 구분해서 안내합니다.

## Codex

### GUI App

- 최신 앱 버전 저장 기준은 계속 `26.616`입니다.
- 공개 Codex changelog의 최신 일반 항목은 2026-06-25 Codex Remote 일반 제공과 DigitalOcean plugin 안내입니다.
- Codex Remote는 ChatGPT 모바일 앱에서 연결된 Mac 또는 Windows host의 작업을 시작, 이어가기, 검토, 승인할 수 있게 안내합니다.
- Remote Control pairing은 iOS/Android device와 host 사이의 인증된 1:1 QR pairing으로 설명되어 있습니다.
- DigitalOcean plugin은 Droplet 생성, SSH 구성, Codex App remote workspace 연결을 돕는 흐름입니다.

### CLI App

- 최신 저장 기준을 `0.142.3`으로 올렸습니다.
- npm `@openai/codex`의 `latest` 안정 태그가 `0.142.3`입니다.
- 공개 Codex changelog에는 이번 CLI 패치의 상세 변경 문구가 별도로 노출되지 않았습니다.
- platform별 패키지도 `0.142.3-linux-x64`, `0.142.3-darwin-arm64`, `0.142.3-win32-x64`처럼 같은 안정 버전으로 맞춰져 있습니다.
- `alpha`는 `0.143.0-alpha.27`까지 올라왔지만 prerelease 채널이므로 안정 버전 보고에는 포함하지 않았습니다.

### Mobile

- 최신 저장 기준은 ChatGPT for iOS `1.2026.167`입니다.
- 공개 Codex changelog의 최신 모바일 항목도 2026-06-22 `1.2026.167`입니다.

## Cursor

### GUI App

- 최신 저장 기준은 계속 Cursor `3.9`입니다.
- 최신 changelog 항목도 2026-06-22 `3.9`입니다.
- `Cursor Customize`에서 plugin, skill, MCP, subagent, rule, command, hook을 한 화면에서 관리하는 변경은 기존 최신 기준으로 유지됩니다.
- Marketplace leaderboard, plugin canvas, GitLab/BitBucket/Azure DevOps plugin repository 가져오기 지원도 기존 최신 기준입니다.

### CLI App

- CLI 전용 새 안정 버전 번호는 확인되지 않았습니다.
- 별도 CLI baseline 변경이 없어 `.version`의 CLI 값은 계속 `null`로 유지합니다.

## Antigravity

### GUI App

- 최신 저장 기준은 계속 Antigravity 2.0 `2.2.1`입니다.
- 최신 공개 항목은 2026-06-25 `Antigravity Guide, audio support, search improvements, and performance fixes`입니다.
- `Antigravity Guide` skill, audio file rendering, substring file search, `Conversation Width`, OAuth token keyring 저장, permission dialog 설명 개선은 기존 최신 기준입니다.
- 이번 실행에서 `2.2.2` 같은 새 GUI 버전은 확인되지 않았습니다.

### IDE App

- 최신 저장 기준은 계속 Antigravity IDE `2.1.1`입니다.
- 최신 공개 항목은 2026-06-22 quota screen, agent permission/security, MCP stability 개선입니다.
- `mcp_config.json`의 `url` 필드 지원, strict mode sensitive path에 `.vscode`와 `.cache` 추가도 기존 최신 기준입니다.
- 이번 실행에서 `2.1.2` 같은 새 IDE 버전은 확인되지 않았습니다.

### CLI App

- Antigravity 2.0 제품군 기준의 CLI baseline은 유지합니다.
- 공식 changelog에서 별도 새 CLI 패치 버전 번호는 확인되지 않았습니다.

## Sources

- [Claude Code CHANGELOG](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [Claude Code raw CHANGELOG](https://raw.githubusercontent.com/anthropics/claude-code/main/CHANGELOG.md)
- [npm @anthropic-ai/claude-code](https://www.npmjs.com/package/@anthropic-ai/claude-code)
- [OpenAI Codex changelog](https://developers.openai.com/codex/changelog)
- [npm @openai/codex](https://www.npmjs.com/package/@openai/codex)
- [Cursor changelog](https://cursor.com/ko/changelog)
- [Google Antigravity changelog](https://antigravity.google/changelog)
- [Google Antigravity releases](https://antigravity.google/releases)
