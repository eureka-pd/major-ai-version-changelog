# Claude Code

- 확인 결과: Claude Code에는 새 버전이 있습니다.
- 이전 저장 기준: `2.1.173` (2026-06-11)
- 최신 확인 기준: `2.1.175` (npm publish: 2026-06-12)
- 중복 보고 방지 상태: `.version`의 Claude Code GUI/CLI 기준을 `2.1.175`로 저장했습니다.
- 출처: [Claude Code CHANGELOG](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md), [npm @anthropic-ai/claude-code](https://www.npmjs.com/package/@anthropic-ai/claude-code)

## GUI App

### `2.1.175`

- 조직이나 관리자가 허용 모델 목록을 강하게 적용할 수 있는 `enforceAvailableModels` 설정이 추가되었습니다.
- 이 설정을 켜면 기본 모델도 허용 목록 안에서만 선택됩니다. 기본값이 허용되지 않은 모델을 가리키면 첫 번째 허용 모델로 자동 전환됩니다.
- 사용자 설정이나 프로젝트 설정이 관리자가 정한 `availableModels` 범위를 넓힐 수 없게 됩니다. 기업 환경에서는 모델 거버넌스가 더 예측 가능해집니다.

### `2.1.174`

- fullscreen mode에서 mouse wheel scroll acceleration을 끄는 `wheelScrollAccelerationEnabled` 설정이 추가되었습니다.
- `/model` picker가 Default가 실제로 가리키는 모델 family를 숨기던 문제가 수정되었습니다.
- `ANTHROPIC_DEFAULT_SONNET_MODEL`로 다른 Sonnet을 고정했을 때 `/model` picker가 고정된 모델이 아니라 hardcoded label을 보여주던 문제가 수정되었습니다.
- enterprise usage-based billing 계정에서 Fable 5 사용량 credit banner가 잘못 표시되던 문제가 수정되었습니다.
- Bedrock GovCloud `us-gov-*` region에서 inference profile prefix를 잘못 계산해 400 error가 나던 문제가 수정되었습니다.
- background session이 다른 session의 `ANTHROPIC_*` provider 환경 변수를 물려받던 문제가 수정되었습니다.
- macOS와 Linux에서 shell command를 중단한 직후 Claude Code를 종료할 때 1-2초 멈추던 문제가 줄었습니다.
- git commit co-author attribution, `/advisor` 모델 선택, skill hot-reload, Workflow `agent()` subagent attribution, VSCode `/usage` breakdown, pre-warmed background worker 인증 오류가 함께 개선되었습니다.

## CLI App

- npm 기준 최신 패키지는 `2.1.175`입니다.
- CLI 사용자는 관리형 모델 allowlist, fullscreen scroll 동작, background session 환경 변수 격리, Bedrock GovCloud, model picker 안정화의 영향을 받습니다.
- 운영 조직에서는 허용 모델 정책이 더 강하게 적용되고, 개인 사용자는 모델 선택 UI와 background 작업 안정성이 좋아집니다.
