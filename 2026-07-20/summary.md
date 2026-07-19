# SUMMARY

오늘 새로 반영한 안정 기준은 Claude Code `2.1.215`입니다. Codex 안정판은 `0.144.6`을 유지하고 prerelease만 `0.145.0-alpha.24`로 올라갔습니다. Cursor와 Antigravity의 버전 기준은 그대로입니다.

## Claude Code

### GUI App

- 최신 저장 기준을 `2.1.214`에서 `2.1.215`로 올렸습니다.
- Claude가 `/verify`와 `/code-review` skill을 스스로 실행하지 않도록 바뀌었습니다.
- 검증이나 코드 리뷰가 필요하면 사용자가 해당 명령을 직접 실행해야 합니다.

### CLI App

- npm `latest`와 `next`는 모두 `2.1.215`입니다.
- 자동 검증·리뷰 실행을 없애 사용자가 실행 시점을 직접 정하게 했습니다.

## Codex

### GUI App

- 최신 숫자 저장 기준은 계속 Codex 앱 `26.616`입니다.
- 새 GUI release는 확인되지 않았습니다.

### CLI App

- 안정 버전 최신 기준은 계속 `0.144.6`입니다.
- 사전 공개 테스트 빌드는 `0.145.0-alpha.23`에서 `0.145.0-alpha.24`로 올라갔습니다.
- alpha 빌드의 별도 변경 설명은 공개되지 않았습니다.

### Mobile

- 최신 저장 기준은 계속 ChatGPT for iOS `1.2026.188`입니다.
- 새 mobile release는 확인되지 않았습니다.

## Cursor

### GUI App

- 최신 버전 번호는 계속 Cursor `3.11`입니다.
- 7월 17일 Slack 개선 공지 이후 새 changelog는 확인되지 않았습니다.

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
- 공식 macOS ARM 설치 binary도 `1.1.4`를 유지합니다.
- 새 CLI release는 확인되지 않았습니다.

## Sources

- [Claude Code CHANGELOG](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [Claude Code raw CHANGELOG](https://raw.githubusercontent.com/anthropics/claude-code/main/CHANGELOG.md)
- [npm @anthropic-ai/claude-code](https://www.npmjs.com/package/@anthropic-ai/claude-code)
- [OpenAI Codex changelog](https://developers.openai.com/codex/changelog)
- [Codex CLI 0.145.0-alpha.24 release](https://github.com/openai/codex/releases/tag/rust-v0.145.0-alpha.24)
- [npm @openai/codex](https://www.npmjs.com/package/@openai/codex)
- [Cursor changelog](https://cursor.com/ko/changelog)
- [Google Antigravity changelog](https://antigravity.google/changelog)
- [Google Antigravity releases](https://antigravity.google/releases)
- [Antigravity Hub release API](https://antigravity-hub-auto-updater-974169037036.us-central1.run.app/releases)
- [Antigravity IDE release API](https://antigravity-ide-auto-updater-974169037036.us-central1.run.app/releases)
- [Antigravity CLI manifest](https://antigravity-cli-auto-updater-974169037036.us-central1.run.app/manifests/darwin_arm64.json)
