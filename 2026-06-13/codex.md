# Codex

- 확인 결과: Codex에는 새로 보고할 앱 버전이 있습니다.
- 이전 저장 기준: Codex app `26.608`, Codex CLI `0.139.0`, ChatGPT for iOS `1.2026.153`
- 최신 확인 기준: Codex app `26.609`, Codex CLI `0.139.0`, ChatGPT for iOS `1.2026.153`
- 중복 보고 방지 상태: Codex app component를 `26.609`로 저장했습니다.
- 출처: [OpenAI Codex changelog](https://developers.openai.com/codex/changelog), [npm @openai/codex](https://www.npmjs.com/package/@openai/codex)

## GUI App

### Codex app `26.609` (2026-06-11)

- Plus와 Pro 사용자를 위한 rate-limit reset banking이 추가되었습니다. launch 시점에 무료 reset 1개가 제공되고, referral invitation으로 promotion 기간 중 추가 reset을 얻을 수 있습니다.
- Business workspace에서는 coworker 초대를 통해 shared workspace credit을 얻을 수 있는 별도 referral program이 추가되었습니다.
- Chrome과 Codex in-app browser에서 Browser use용 Developer mode가 추가되었습니다. Codex가 Chrome DevTools Protocol을 통해 performance profiling, network traffic, console output, runtime error, page state를 더 깊게 볼 수 있습니다.
- app composer에 `/init` command가 추가되었습니다. CLI의 project instruction 초기화 흐름을 앱에서도 바로 만들 수 있습니다.
- macOS Dock icon을 light/dark Codex variant로 바꿀 수 있습니다.
- Enterprise 사용자는 EEA, UK, Switzerland 밖에서 Computer Use를 사용할 수 있게 되었습니다.
- Windows에서는 Computer Use의 per-app access control 설정을 지원합니다.
- command menu에 Unread chats section이 생겨 읽지 않은 최근 chat으로 더 빨리 이동할 수 있습니다.
- Browser use가 CDP와 DOM snapshot 최적화로 최대 2배 빨라졌습니다.
- activity summary, plugin management, usage-limit error, approval feedback shortcut, Browser download handling, scheduled automation approval mode, background agent tab 복원, commit/PR message 생성, Codex Mobile QR pairing, remote-control MFA, updater prompt 등 여러 UI/안정성 문제가 개선되었습니다.

## CLI App

- Codex CLI 최신 정식 기준은 계속 `0.139.0`입니다.
- npm `latest`도 `0.139.0`입니다.
- `0.140.0` 계열은 npm에 alpha 빌드만 확인되어 정식 버전 보고 대상에서는 제외했습니다.
