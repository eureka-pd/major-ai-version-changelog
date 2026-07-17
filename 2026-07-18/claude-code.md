# Claude Code

오늘 새로 반영할 Claude Code 버전은 `2.1.212`입니다. 여러 작업을 동시에 돌릴 때 세션을 더 쉽게 관리하도록 바뀌었고, 무한 검색·과도한 subagent 실행을 막는 안전장치와 권한·worktree 보안 수정이 추가됐습니다.

## GUI App

- 최신 저장 기준을 `2.1.211`에서 `2.1.212`로 올렸습니다.
- `/fork`는 현재 대화를 별도 background session으로 복사해 원래 작업을 계속할 수 있게 바뀌었습니다. 기존처럼 현재 세션 안에서 subagent를 만들려면 `/subtask`를 사용합니다.
- agent 화면에서 `/resume`을 입력하면 과거 세션을 고르는 목록이 열리고, 목록에서 삭제했던 세션도 background session으로 다시 시작할 수 있습니다.
- 2분 넘게 걸리는 MCP 호출은 자동으로 background로 이동해 화면을 계속 사용할 수 있습니다.
- background session에 다시 붙을 때 빈 화면 대신 기존 대화를 먼저 보여주며, 입력 대기 상태를 `Needs input`으로 더 정확히 표시합니다.
- 좁은 화면의 diff 표시, 긴 경로가 있는 승인 창, terminal 크기 변경 뒤 화면 배치가 깨지던 문제를 고쳤습니다.

## CLI App

- npm `latest`와 `next`는 모두 `2.1.212`입니다.
- `claude auto-mode reset` 명령을 추가해 auto mode 설정을 기본값으로 되돌릴 수 있습니다.
- 한 세션의 WebSearch와 subagent 생성 횟수에 각각 기본 200회 제한을 두어 잘못된 반복 실행을 막습니다.
- plan mode가 `touch`, `rm` 같은 파일 변경 명령을 승인 없이 실행하던 문제를 고쳤습니다.
- 저장소의 `.claude/worktrees` 심볼릭 링크를 따라 저장소 밖에 파일을 만들 수 있던 문제를 막았습니다.
- 실행 중인 Bash가 SIGTERM을 받으면 자식 프로세스까지 종료하고 코드 `143`으로 끝나도록 바꿨습니다.
- Windows에서 PowerShell 5.1이 막혀도 PowerShell 7을 우선 사용해 background 실행 실패를 줄였습니다.
- web search·fetch가 529 또는 속도 제한을 만나면 제한된 횟수로 재시도하고, agent 간 메시지의 중복 기록을 줄여 토큰 사용량을 낮췄습니다.

## Sources

- [Claude Code CHANGELOG](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [Claude Code raw CHANGELOG](https://raw.githubusercontent.com/anthropics/claude-code/main/CHANGELOG.md)
- [npm @anthropic-ai/claude-code](https://www.npmjs.com/package/@anthropic-ai/claude-code)
