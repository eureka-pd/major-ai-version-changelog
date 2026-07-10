# Codex

오늘 새로 반영할 기준은 Codex CLI `0.144.1`과 2026-07-09 ChatGPT desktop app 통합 소식입니다. CLI는 저장된 `0.142.3`에서 두 개의 안정 기능 릴리스를 거쳐 `0.144.1`로 올라갔습니다.

## GUI App

- 숫자로 공개된 최신 Codex 앱 버전 저장 기준은 계속 `26.616`입니다.
- Codex가 macOS와 Windows의 ChatGPT desktop app 안에 통합되었습니다. 기존 Codex app 사용자는 프로젝트와 설정을 유지한 채 업데이트할 수 있습니다.
- Markdown과 code를 앱에서 직접 편집하고 선택 영역에 annotation을 붙여 수정 요청을 보낼 수 있습니다.
- sidebar에서 GitHub PR diff와 reviewer feedback을 함께 보고 Codex에게 수정 작업을 맡길 수 있습니다.
- 하나의 project에서 여러 repository를 함께 다룰 수 있습니다.
- Computer Use 속도, 작업 진행 표시, plugin 설정 위치, mobile 연결과 SSH video rendering이 개선되었습니다.

## CLI App

- 최신 저장 기준을 `0.144.1`로 올렸습니다. npm `@openai/codex`의 `latest`도 같은 안정 버전입니다.
- `0.143.0`에서는 remote plugin 기본 활성화, system proxy/PAC/WPAD 지원, manual remote-control pairing code, Bedrock GPT-5.6 model 지원, MCP tool search 기본 사용이 추가되었습니다.
- `0.144.0`에서는 사용량 reset credit 정보, 쓰기 작업만 승인받는 `writes` app approval mode, MCP interactive authentication, 외부 host가 제공하는 Codex 인증 흐름이 추가되었습니다.
- Windows sandbox, Intel Mac Code Mode, terminal control sequence, connector 인증 갱신, WebSocket proxy 처리와 대형 repository의 `/review` branch picker가 개선되었습니다.
- `0.144.1`은 standalone installer가 GitHub release metadata 형식 변화에도 동작하도록 하고, macOS code-mode host 설치와 fallback runtime을 보강한 패치입니다.
- `alpha`는 `0.145.0-alpha.2`까지 올라왔지만 prerelease 채널이므로 안정 버전 기준에는 포함하지 않았습니다.

## Mobile

- 최신 숫자 저장 기준은 ChatGPT for iOS `1.2026.167`입니다.
- 이번 확인에서 별도의 새 mobile version 번호는 공개 changelog에 없었습니다.

## Sources

- [OpenAI Codex changelog](https://developers.openai.com/codex/changelog)
- [npm @openai/codex](https://www.npmjs.com/package/@openai/codex)
