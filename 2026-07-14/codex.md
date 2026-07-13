# Codex

오늘 새로 반영할 안정 기준은 Codex CLI `0.144.3`입니다. `0.144.2`의 실제 버그 수정과 코드 변경 없이 버전만 올린 `0.144.3`이 같은 날 공개되었습니다.

## GUI App

- 숫자로 공개된 최신 Codex 앱 버전 저장 기준은 계속 `26.616`입니다.
- 2026-07-09 ChatGPT desktop app 통합 이후 새 GUI release 항목은 확인되지 않았습니다.

## CLI App

- 안정 버전 최신 기준을 `0.144.1`에서 `0.144.3`으로 올렸습니다.
- `0.144.2`는 Guardian 자동 검토의 prompting 회귀를 되돌려, 이전의 자동 검토 정책과 요청 형식, 도구 동작을 복구했습니다.
- `0.144.3`은 `0.144.2` 이후 새로 병합된 코드가 없는 version-only release입니다. 사용자 기능이나 추가 수정은 없습니다.
- 사전 공개 테스트 빌드는 `0.145.0-alpha.7`까지 올라갔습니다. 안정 버전과 섞이지 않도록 `.version`에 따로 기록했습니다.

## Mobile

- 최신 저장 기준은 계속 ChatGPT for iOS `1.2026.181`입니다.
- 저장된 기준 이후 새 mobile release 항목은 확인되지 않았습니다.

## Sources

- [OpenAI Codex changelog](https://developers.openai.com/codex/changelog)
- [Codex CLI 0.144.2](https://github.com/openai/codex/releases/tag/rust-v0.144.2)
- [Codex CLI 0.144.3](https://github.com/openai/codex/releases/tag/rust-v0.144.3)
- [Codex CLI prerelease 0.145.0-alpha.7](https://github.com/openai/codex/releases/tag/rust-v0.145.0-alpha.7)
- [npm @openai/codex](https://www.npmjs.com/package/@openai/codex)
