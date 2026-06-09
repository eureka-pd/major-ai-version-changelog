# Claude Code

- 확인 결과: `.version` 기준으로 새 버전이 있습니다.
- 이전 저장 기준: `2.1.168`
- 최신 확인 기준: `2.1.170`
- 중복 보고 방지 상태: `2.1.170`으로 저장해 다음 실행에서 같은 내용을 다시 보고하지 않도록 했습니다.
- 출처: [Claude Code CHANGELOG](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md), [npm @anthropic-ai/claude-code](https://www.npmjs.com/package/@anthropic-ai/claude-code)

## GUI App

### `2.1.170`

- 새 모델 접근 안내가 추가되었습니다. changelog는 `2.1.170`으로 업데이트하면 Claude Fable 5를 사용할 수 있다고 설명합니다.
- VS Code 통합 터미널이나 Claude Code 환경 변수를 물려받은 shell에서 시작했을 때 세션 transcript가 저장되지 않고 `--resume` 목록에도 안 보이던 문제가 수정되었습니다.
- 사용자가 체감하는 핵심은 새 모델 사용 가능성과 세션 복구 안정성입니다.

### `2.1.169`

- 문제 해결용 `--safe-mode`와 `CLAUDE_CODE_SAFE_MODE`가 추가되었습니다. 설정, 플러그인, 스킬, hook, MCP 서버를 끈 상태로 실행해 원인을 좁힐 수 있습니다.
- `/cd` 명령이 추가되어 세션 중 작업 폴더를 바꿀 수 있습니다.
- bundled skills와 built-in slash command를 숨기는 설정이 추가되었습니다.
- 방향키, 관리형 MCP 정책, macOS UI 멈춤, Windows `claude -p`, Remote Control 재연결, background agent, plugin cache, 권한 prompt 등 여러 안정성 문제가 고쳐졌습니다.
- 전체적으로 새 기능보다 운영 안정성과 진단 도구를 크게 보강한 릴리스입니다.

## CLI App

- Claude Code CLI도 같은 `2.1.170` 기준으로 추적합니다.
- `2.1.169`의 `--safe-mode`, `/cd`, background agent 안정화, `claude agents --json` 개선은 CLI 사용 흐름에 직접 영향을 줍니다.
- `2.1.170`의 transcript 저장 수정은 터미널에서 시작한 세션을 나중에 이어서 작업할 때 중요합니다.
