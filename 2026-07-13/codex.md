# Codex

오늘 새로 반영할 안정 기준은 ChatGPT for iOS `1.2026.181`입니다. 이 항목은 2026-07-06 공개되었지만 기존 `.version`의 `1.2026.167`에 반영되지 않아 이번 실행에서 바로잡았습니다. Codex CLI 안정 버전은 `0.144.1` 그대로입니다.

## GUI App

- 숫자로 공개된 최신 Codex 앱 버전 저장 기준은 계속 `26.616`입니다.
- 2026-07-09 ChatGPT desktop app 통합 이후 새 GUI release 항목은 확인되지 않았습니다.

## CLI App

- 안정 버전 최신 기준은 계속 `0.144.1`이며 npm `latest`도 같습니다.
- 사전 공개 테스트 빌드는 `0.145.0-alpha.4`까지 올라갔습니다. 안정 버전과 섞지 않도록 `.version`에 prerelease로 따로 기록했습니다.
- `alpha.4`는 실험 단계이므로 일반 사용자의 업데이트 기준에는 포함하지 않습니다.

## Mobile

- 최신 저장 기준을 ChatGPT for iOS `1.2026.181`로 올렸습니다.
- 대화 안에서 Codex task를 생성, 검색, 열기, fork, 관리할 수 있습니다.
- staged, unstaged, branch, last-turn 변경사항을 나눠 보고 branch끼리 비교할 수 있습니다.
- 선택한 transcript를 composer에 넣고, 전송 전에 이미지와 파일 첨부를 미리 볼 수 있습니다.
- SSH 연결, task loading과 reconnect 복구, autocomplete, plugin 표시, workspace diff가 개선되었습니다.
- thread list가 멈추거나 prompt mode가 교착되는 문제, 오래된 이미지와 microphone·keyboard 관련 오류가 수정되었습니다.

## Sources

- [OpenAI Codex changelog](https://developers.openai.com/codex/changelog)
- [npm @openai/codex](https://www.npmjs.com/package/@openai/codex)
- [Codex CLI prerelease](https://github.com/openai/codex/releases/tag/rust-v0.145.0-alpha.4)
