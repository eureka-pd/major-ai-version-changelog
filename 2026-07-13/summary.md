# SUMMARY

오늘 새로 반영할 기준은 Claude Code `2.1.207`과 ChatGPT for iOS `1.2026.181`입니다. Codex CLI prerelease는 stable과 분리해 `0.145.0-alpha.4`로 기록했습니다. Cursor와 Antigravity는 저장된 최신 기준과 같습니다.

## Claude Code

### GUI App

- 최신 저장 기준을 `2.1.207`로 올렸습니다.
- background agent와 worktree session의 재연결·복구가 더 안정적으로 바뀌었습니다.
- Remote Control 상태 복원과 agent teams mailbox 오류 처리가 개선되었습니다.

### CLI App

- npm 기본 `latest`와 `next`는 `2.1.207`이며 별도 `stable` 태그는 `2.1.197`입니다.
- Bedrock, Vertex AI, Foundry에서 Auto mode를 바로 사용할 수 있습니다.
- Bedrock, Vertex, AWS 기반 Claude Platform의 기본 모델이 Claude Opus 4.8로 바뀌었습니다.
- 긴 출력의 터미널 멈춤·입력 지연·화면 점프가 개선되었습니다.
- plugin shell injection 방어, 사용자 launcher 보호, AWS 인증과 background session 안정성 수정이 포함되었습니다.

## Codex

### GUI App

- 최신 숫자 저장 기준은 계속 Codex 앱 `26.616`입니다.
- 2026-07-09 ChatGPT desktop app 통합 이후 새 GUI release는 확인되지 않았습니다.

### CLI App

- 안정 버전 최신 기준은 계속 `0.144.1`입니다.
- 사전 공개 테스트 빌드는 `0.145.0-alpha.4`까지 올라갔으며 stable 기준과 분리해 기록했습니다.

### Mobile

- 최신 저장 기준을 ChatGPT for iOS `1.2026.181`로 올렸습니다.
- 대화에서 Codex task를 생성·검색·열기·fork·관리할 수 있습니다.
- 변경사항 필터와 branch 비교, transcript 재사용, 첨부 미리보기가 추가되었습니다.
- SSH 연결, loading·reconnect, autocomplete, plugin 표시와 workspace diff가 개선되었습니다.

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
- 설치 manifest의 binary `1.1.1`은 별도 버전 체계이며 공개 changelog의 새 CLI release는 없습니다.

## Sources

- [Claude Code CHANGELOG](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [Claude Code raw CHANGELOG](https://raw.githubusercontent.com/anthropics/claude-code/main/CHANGELOG.md)
- [npm @anthropic-ai/claude-code](https://www.npmjs.com/package/@anthropic-ai/claude-code)
- [OpenAI Codex changelog](https://developers.openai.com/codex/changelog)
- [npm @openai/codex](https://www.npmjs.com/package/@openai/codex)
- [Codex CLI prerelease](https://github.com/openai/codex/releases/tag/rust-v0.145.0-alpha.4)
- [Cursor changelog](https://cursor.com/ko/changelog)
- [Google Antigravity changelog](https://antigravity.google/changelog)
- [Google Antigravity releases](https://antigravity.google/releases)
