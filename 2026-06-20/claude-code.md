# Claude Code

오늘 Claude Code는 `2.1.183`으로 올라갔습니다. 핵심은 자동 실행 모드에서 위험한 명령을 더 잘 막고, subagent와 scheduled task 주변의 오류를 줄인 안정성 업데이트입니다.

## GUI App

- 최신 저장 기준: `2.1.183`
- 이전 저장 기준: `2.1.181`
- auto mode에서 사용자가 로컬 작업 삭제를 요청하지 않았을 때 `git reset --hard`, `git checkout -- .`, `git clean -fd`, `git stash drop` 같은 명령을 막습니다. 실수로 작업물을 날릴 가능성을 줄인 변경입니다.
- 모델이 deprecated 되었거나 새 모델로 자동 치환될 때 경고를 보여줍니다. agent frontmatter에 지정된 모델도 대상입니다.
- `/config --help`가 추가되어 `/config key=value`로 바꿀 수 있는 shorthand key를 확인할 수 있습니다.
- `/config` 토글은 Enter와 Space 모두로 바꿀 수 있고, Esc는 되돌리기가 아니라 저장 후 닫기로 동작합니다.
- startup 화면의 setup issues 문구는 제거됐고, 문제 확인은 `/doctor`와 `--debug` 쪽으로 정리됐습니다.
- subagent에서 WebSearch가 빈 결과를 반환하던 문제, user-level skill이 autocomplete에 중복 표시되던 문제, subagent thinking block만 돌아오면 응답 없이 종료되던 문제를 고쳤습니다.

## CLI App

- 최신 저장 기준: `2.1.183`
- 이전 저장 기준: `2.1.181`
- print mode(`-p`)에서도 deprecated model 또는 자동 모델 변경 경고가 stderr로 표시됩니다.
- `attribution.sessionUrl` 설정으로 web 또는 Remote Control session에서 commit/PR에 claude.ai session link를 넣지 않도록 할 수 있습니다.
- `thinking.disabled.display: Extra inputs are not permitted` 400 오류가 subagent spawn과 session title 생성에서 발생하던 문제를 수정했습니다.
- Windows Terminal에서 nested subagent 부하가 클 때 fullscreen TUI가 깨지던 문제를 수정했습니다.
- tmux teammate pane이 느린 shell rc 초기화 때문에 실패하거나, agent spawn 중 입력한 키가 새 pane으로 새는 문제를 수정했습니다.
- scheduled task와 webhook trigger delivery가 키보드 입력처럼 처리되어 pending action을 승인하거나 session title을 바꿀 수 있던 문제를 막았습니다.

## Sources

- [Claude Code CHANGELOG](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [npm @anthropic-ai/claude-code](https://www.npmjs.com/package/@anthropic-ai/claude-code)
