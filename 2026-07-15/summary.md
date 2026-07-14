# SUMMARY

오늘 새로 반영한 기준은 Claude Code `2.1.209`, Codex CLI `0.144.4`, ChatGPT for iOS `1.2026.188`, Antigravity CLI binary `1.1.2`입니다. Codex prerelease는 stable과 분리해 `0.145.0-alpha.11`로 기록했습니다. Cursor와 나머지 GUI/IDE 기준은 그대로입니다.

## Claude Code

### GUI App

- 최신 저장 기준을 `2.1.207`에서 `2.1.209`로 올렸습니다.
- 화면 낭독기용 plain-text 모드와 fullscreen 메뉴의 마우스 조작이 추가되었습니다.
- fast mode 복원, background agent 메시지 보존과 재접속이 안정화되었습니다.
- `2.1.209`는 background session에서 `/model` 같은 dialog가 막히던 회귀를 수정했습니다.

### CLI App

- npm `latest`와 `next`는 모두 `2.1.209`입니다.
- vim insert mode remap과 기업용 process wrapper를 지원합니다.
- 큰 JSON/stream-json 출력 누락, 긴 session의 메모리 누수, 대형 markdown 표 렌더링 문제를 줄였습니다.
- Edit, Read, Grep, Glob의 여러 경계 사례도 수정했습니다.

## Codex

### GUI App

- 최신 숫자 저장 기준은 계속 Codex 앱 `26.616`입니다.
- 2026-07-09 ChatGPT desktop app 통합 이후 새 GUI release는 확인되지 않았습니다.

### CLI App

- 안정 버전 최신 기준을 `0.144.3`에서 `0.144.4`로 올렸습니다.
- `0.144.4`는 사용자에게 보이는 변경이 없는 patch release입니다.
- 사전 공개 테스트 빌드는 `0.145.0-alpha.11`이며 stable 기준과 분리해 기록했습니다.

### Mobile

- 최신 저장 기준을 ChatGPT for iOS `1.2026.181`에서 `1.2026.188`로 올렸습니다.
- Codex task에서 inline visualization을 표시할 수 있게 되었습니다.
- task 생성과 링크, tool 진행 표시, 파일 열기 안내, 긴 prompt composer가 개선되었습니다.
- task별 fast mode 복원과 approval preset 적용 오류를 고쳤습니다.

## Cursor

### GUI App

- 최신 저장 기준은 계속 Cursor `3.11`입니다.
- 새 GUI release는 확인되지 않았습니다.

### CLI App

- CLI 전용 새 안정 버전 번호는 확인되지 않았습니다.
- `.version`의 CLI 값은 계속 `null`입니다.

## Antigravity

### GUI App

- 최신 저장 기준은 계속 Antigravity 2.0 `2.2.1`입니다.
- Hub release API에서도 새 GUI release는 확인되지 않았습니다.

### IDE App

- 최신 저장 기준은 계속 Antigravity IDE `2.1.1`입니다.
- IDE release API에서도 새 release는 확인되지 않았습니다.

### CLI App

- 제품군 기준은 계속 `2.0`입니다.
- 설치 manifest의 별도 binary version은 `1.1.1`에서 `1.1.2`로 올라갔습니다.
- 공개 changelog에는 binary `1.1.2`의 세부 변경 설명이 없습니다.

## Sources

- [Claude Code CHANGELOG](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [Claude Code raw CHANGELOG](https://raw.githubusercontent.com/anthropics/claude-code/main/CHANGELOG.md)
- [npm @anthropic-ai/claude-code](https://www.npmjs.com/package/@anthropic-ai/claude-code)
- [OpenAI Codex changelog](https://developers.openai.com/codex/changelog)
- [Codex CLI 0.144.4](https://github.com/openai/codex/releases/tag/rust-v0.144.4)
- [Codex CLI prerelease 0.145.0-alpha.11](https://github.com/openai/codex/releases/tag/rust-v0.145.0-alpha.11)
- [npm @openai/codex](https://www.npmjs.com/package/@openai/codex)
- [Cursor changelog](https://cursor.com/ko/changelog)
- [Google Antigravity changelog](https://antigravity.google/changelog)
- [Google Antigravity releases](https://antigravity.google/releases)
- [Antigravity CLI manifest](https://antigravity-cli-auto-updater-974169037036.us-central1.run.app/manifests/darwin_arm64.json)
