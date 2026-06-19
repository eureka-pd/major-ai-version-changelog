# Codex

오늘 Codex는 앱 버전이 `26.616`으로 올라간 항목을 새로 반영했습니다. CLI 안정 버전은 `0.141.0` 그대로이고, npm에는 `0.142.0-alpha.*`가 보이지만 안정 릴리스가 아니므로 중복 방지 장부에는 올리지 않았습니다.

## GUI App

- 최신 앱 버전 저장 기준: `26.616`
- 이전 앱 버전 저장 기준: `26.609`
- macOS에서 Record & Replay가 추가됐습니다. 사용자가 직접 보여준 작업 흐름을 재사용 가능한 skill로 바꾸는 기능입니다.
- Record & Replay 초기 제공 지역은 EEA, UK, Switzerland를 제외하며, Computer Use도 켜져 있어야 합니다.
- automation run history에 bulk action이 추가되어 여러 run을 한 번에 읽음 처리하거나 archive할 수 있습니다.
- SSH connection 관리를 위한 deep link가 추가됐습니다.
- Browser Use는 draft browser session이 server로 이동해도 visible-tab routing과 annotation이 더 잘 유지되도록 개선됐습니다.
- 추가 성능 개선과 버그 수정이 포함됐습니다.

## CLI App

- 최신 저장 기준: `0.141.0`
- npm `@openai/codex`의 latest 안정 태그도 `0.141.0`입니다.
- `0.142.0-alpha.4`까지 prerelease가 올라와 있지만, 안정 버전이 아니므로 이번 보고 기준에는 포함하지 않았습니다.
- 직전 보고에서 이미 반영한 remote executor Noise relay, cross-platform remote execution 보존, plugin discovery 개선 항목은 저장 기준과 같습니다.

## Mobile

- 최신 저장 기준: ChatGPT for iOS `1.2026.160`
- 새 모바일 버전 번호는 확인되지 않았습니다.

## Sources

- [OpenAI Codex changelog](https://developers.openai.com/codex/changelog)
- [npm @openai/codex](https://www.npmjs.com/package/@openai/codex)
