# Codex

오늘 새로 반영할 기준은 Codex CLI `0.144.4`와 ChatGPT for iOS `1.2026.188`입니다. CLI patch는 사용자 기능 변화가 없고, mobile은 task 화면과 조작 안정성이 개선되었습니다.

## GUI App

- 숫자로 공개된 최신 Codex 앱 버전 저장 기준은 계속 `26.616`입니다.
- 2026-07-09 ChatGPT desktop app 통합 이후 새 GUI release 항목은 확인되지 않았습니다.

## CLI App

- 안정 버전 최신 기준을 `0.144.3`에서 `0.144.4`로 올렸습니다.
- `0.144.4`는 사용자에게 보이는 기능 변경이 없는 patch release입니다.
- 사전 공개 테스트 빌드는 `0.145.0-alpha.11`까지 올라갔습니다. 안정 버전과 섞이지 않도록 `.version`에 따로 기록했습니다.

## Mobile

- 최신 저장 기준을 ChatGPT for iOS `1.2026.181`에서 `1.2026.188`로 올렸습니다.
- Codex task 안에서 inline visualization을 표시할 수 있게 되었습니다.
- 대화에서 task를 만들고 관리하는 흐름, 새 task 링크, tool 진행 표시, 파일 열기 안내가 더 안정적으로 바뀌었습니다.
- 긴 prompt와 큰 글자 크기에서 composer가 잘리지 않도록 개선했고, task별 fast mode 복원과 approval preset 적용 오류를 고쳤습니다.

## Sources

- [OpenAI Codex changelog](https://developers.openai.com/codex/changelog)
- [Codex CLI 0.144.4](https://github.com/openai/codex/releases/tag/rust-v0.144.4)
- [Codex CLI prerelease 0.145.0-alpha.11](https://github.com/openai/codex/releases/tag/rust-v0.145.0-alpha.11)
- [npm @openai/codex](https://www.npmjs.com/package/@openai/codex)
