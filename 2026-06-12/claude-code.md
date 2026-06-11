# Claude Code

- 확인 결과: Claude Code에는 새 버전이 있습니다.
- 이전 저장 기준: `2.1.170` (2026-06-09)
- 최신 확인 기준: `2.1.173` (npm publish: 2026-06-11)
- 중복 보고 방지 상태: `.version`의 Claude Code GUI/CLI 기준을 `2.1.173`으로 저장했습니다.
- 출처: [Claude Code CHANGELOG](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md), [npm @anthropic-ai/claude-code](https://www.npmjs.com/package/@anthropic-ai/claude-code)

## GUI App

### `2.1.173`

- Fable 5 모델 이름에 `[1m]` 같은 1M context 표시가 붙어 있을 때 이름을 잘못 처리하던 문제가 수정되었습니다.
- Windows에서 sandbox가 켜진 상태로 시작할 때, 실제 문제 없이 "sandbox dependencies missing" 경고가 뜨던 문제가 수정되었습니다.

### `2.1.172`

- sub-agent가 다시 자기 sub-agent를 만들 수 있습니다. 최대 5단계까지 중첩할 수 있어, 큰 작업을 더 잘게 나눠 맡기는 구조가 가능해졌습니다.
- `/plugin` marketplace 탐색 화면에 검색창이 추가되었습니다.
- 1M context 권한/크레딧, background agent, remote session, model picker, Bedrock model 선택, plugin marketplace UI 같은 여러 안정성 문제가 수정되었습니다.
- 긴 대화에서 불필요한 메시지 정규화와 tool-use 상태 변환을 줄여 성능이 개선되었습니다.
- idle 상태의 CPU 사용량과 UI re-render가 줄었습니다.

## CLI App

- npm 기준 최신 패키지도 `2.1.173`입니다.
- CLI 사용자가 체감할 핵심 변화는 sub-agent 중첩, Bedrock region 자동 인식, background/remote session 안정화, 긴 대화 성능 개선입니다.
- Windows, Bedrock, remote session, 권한 allowlist, wildcard permission rule 관련 오류 수정이 많아 운영 환경에서 덜 멈추고 덜 헷갈리게 됩니다.
