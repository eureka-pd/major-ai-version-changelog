# SUMMARY

오늘 새로 반영한 안정 기준은 Claude Code `2.1.214`, Codex CLI `0.144.6`, Antigravity CLI 설치 binary `1.1.4`입니다. Codex prerelease는 `0.145.0-alpha.23`까지 올랐습니다. Cursor 버전은 `3.11`을 유지하지만 7월 17일 Slack 개선 공지를 새로 기록했습니다.

## Claude Code

### GUI App

- 최신 저장 기준을 `2.1.212`에서 `2.1.214`로 올렸습니다.
- 오래 걸리는 도구 호출에 진행 신호를 추가하고 background session 재접속·삭제 안정성을 개선했습니다.
- 설정 파일, memory frontmatter, feature flag 캐시가 잘못됐을 때 더 안전하게 처리합니다.

### CLI App

- npm `latest`와 `next`는 모두 `2.1.214`입니다. 별도의 `2.1.213` changelog 항목은 없습니다.
- 폴더 허용 규칙, Windows PowerShell, Bash 리다이렉션과 긴 명령 등 권한 판정의 빈틈을 보강했습니다.
- Docker·Podman 원격 daemon 옵션은 권한을 묻도록 바뀌었습니다.
- Windows 프록시·PowerShell 처리, plugin·MCP·OpenTelemetry, background 작업 종료 안정성을 개선했습니다.

## Codex

### GUI App

- 최신 숫자 저장 기준은 계속 Codex 앱 `26.616`입니다.
- 새 GUI release는 확인되지 않았습니다.

### CLI App

- 안정 버전 최신 기준을 `0.144.5`에서 `0.144.6`으로 올렸습니다.
- GPT-5.6 Sol, Terra, Luna의 기본 지침을 갱신하고 context window 정보를 272,000 tokens로 바로잡았습니다.
- 사전 공개 테스트 빌드는 `0.145.0-alpha.22`에서 `0.145.0-alpha.23`으로 올라갔습니다.

### Mobile

- 최신 저장 기준은 계속 ChatGPT for iOS `1.2026.188`입니다.
- 새 mobile release는 확인되지 않았습니다.

## Cursor

### GUI App

- 최신 버전 번호는 계속 Cursor `3.11`입니다.
- Slack에서 작업 전 계획과 진행 상태를 보여 주고, 여러 repo 환경을 선택하거나 중간에 전환할 수 있게 됐습니다.
- 다른 채널과 thread의 내용을 context로 읽고 관련 위치에 업데이트를 보낼 수 있습니다.
- 표, PR, artifact를 포함한 Slack 응답 표시도 더 간결해졌습니다.

### CLI App

- CLI 전용 새 안정 버전 번호는 확인되지 않았습니다.
- `.version`의 CLI 값은 계속 `null`입니다.

## Antigravity

### GUI App

- 최신 저장 기준은 계속 Antigravity 2.0 `2.3.1`입니다.
- 새 GUI release는 확인되지 않았습니다.

### IDE App

- 최신 저장 기준은 계속 Antigravity IDE `2.1.1`입니다.
- 새 IDE release는 확인되지 않았습니다.

### CLI App

- 제품군 기준은 계속 `2.0`입니다.
- 공식 macOS ARM manifest의 설치 binary가 `1.1.3`에서 `1.1.4`로 올라갔습니다.
- 별도 변경 설명은 공개되지 않아 binary 갱신 사실만 기록합니다.

## Sources

- [Claude Code CHANGELOG](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [Claude Code raw CHANGELOG](https://raw.githubusercontent.com/anthropics/claude-code/main/CHANGELOG.md)
- [npm @anthropic-ai/claude-code](https://www.npmjs.com/package/@anthropic-ai/claude-code)
- [OpenAI Codex changelog](https://developers.openai.com/codex/changelog)
- [Codex CLI 0.144.6 release](https://github.com/openai/codex/releases/tag/rust-v0.144.6)
- [npm @openai/codex](https://www.npmjs.com/package/@openai/codex)
- [Cursor changelog](https://cursor.com/ko/changelog)
- [Slack의 Cursor 개선 사항](https://cursor.com/ko/changelog/slack-improvements)
- [Google Antigravity changelog](https://antigravity.google/changelog)
- [Google Antigravity releases](https://antigravity.google/releases)
- [Antigravity Hub release API](https://antigravity-hub-auto-updater-974169037036.us-central1.run.app/releases)
- [Antigravity IDE release API](https://antigravity-ide-auto-updater-974169037036.us-central1.run.app/releases)
- [Antigravity CLI manifest](https://antigravity-cli-auto-updater-974169037036.us-central1.run.app/manifests/darwin_arm64.json)
