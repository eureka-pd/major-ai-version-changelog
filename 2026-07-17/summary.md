# SUMMARY

오늘 새로 반영한 안정 기준은 Claude Code `2.1.211`, Codex CLI `0.144.5`, Antigravity CLI binary `1.1.3`입니다. Codex prerelease는 별도로 `0.145.0-alpha.18`까지 올렸고, Cursor는 `3.11`을 유지합니다.

## Claude Code

### GUI App

- 최신 저장 기준을 `2.1.210`에서 `2.1.211`으로 올렸습니다.
- 권한 미리보기의 보이지 않는 문자와 방향 제어 문자를 무력화해 승인 내용을 속여 보이게 만들기 어렵도록 했습니다.
- 잠자기 뒤 동시 로그아웃, plugin MCP 재연결, Chrome 시작·업로드, background session 재개 문제를 고쳤습니다.
- 설정·통계·diff 화면의 지연을 줄이고 terminal 렌더링 성능을 개선했습니다.

### CLI App

- npm `latest`와 `next`는 모두 `2.1.211`입니다.
- `stream-json`에 subagent 텍스트와 thinking을 포함하는 옵션을 추가했습니다.
- hook의 사용자 확인 결정을 auto mode가 건너뛰지 않도록 하고, subagent 모델 지정이 resume 뒤에도 유지되게 했습니다.
- background agent의 실제 상태를 기다려 보고하고, worktree 권한을 저장소 전체에서 유지합니다.
- 여러 cloud provider에서 발생한 prompt caching 과금 회귀를 고쳤습니다.

## Codex

### GUI App

- 최신 숫자 저장 기준은 계속 Codex 앱 `26.616`입니다.
- 새 GUI release는 확인되지 않았습니다.

### CLI App

- 안정 버전 최신 기준을 `0.144.4`에서 `0.144.5`로 올렸습니다.
- 강제 `rm` 형태를 포함한 위험 명령 감지를 보강하고 거부 이유를 더 분명하게 보여줍니다.
- 사전 공개 테스트 빌드는 `0.145.0-alpha.13`에서 `0.145.0-alpha.18`로 올라갔습니다.

### Mobile

- 최신 저장 기준은 계속 ChatGPT for iOS `1.2026.188`입니다.
- 새 mobile release는 확인되지 않았습니다.

## Cursor

### GUI App

- 최신 저장 기준은 계속 Cursor `3.11`입니다.
- 새 GUI release는 확인되지 않았습니다.

### CLI App

- CLI 전용 새 안정 버전 번호는 확인되지 않았습니다.
- `.version`의 CLI 값은 계속 `null`입니다.

## Antigravity

### GUI App

- 최신 저장 기준은 계속 Antigravity 2.0 `2.3.0`입니다.
- 새 GUI release는 확인되지 않았습니다.

### IDE App

- 최신 저장 기준은 계속 Antigravity IDE `2.1.1`입니다.
- 새 IDE release는 확인되지 않았습니다.

### CLI App

- 제품군 기준은 계속 `2.0`입니다.
- 설치 manifest의 별도 binary version을 `1.1.2`에서 `1.1.3`으로 올렸습니다.
- 공개 changelog에 CLI 전용 변경 설명이 없어 버전만 기록합니다.

## Sources

- [Claude Code CHANGELOG](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [Claude Code raw CHANGELOG](https://raw.githubusercontent.com/anthropics/claude-code/main/CHANGELOG.md)
- [npm @anthropic-ai/claude-code](https://www.npmjs.com/package/@anthropic-ai/claude-code)
- [OpenAI Codex changelog](https://developers.openai.com/codex/changelog)
- [npm @openai/codex](https://www.npmjs.com/package/@openai/codex)
- [Cursor changelog](https://cursor.com/ko/changelog)
- [Google Antigravity changelog](https://antigravity.google/changelog)
- [Google Antigravity releases](https://antigravity.google/releases)
- [Antigravity Hub release API](https://antigravity-hub-auto-updater-974169037036.us-central1.run.app/releases)
- [Antigravity IDE release API](https://antigravity-ide-auto-updater-974169037036.us-central1.run.app/releases)
- [Antigravity CLI manifest](https://antigravity-cli-auto-updater-974169037036.us-central1.run.app/manifests/darwin_arm64.json)
