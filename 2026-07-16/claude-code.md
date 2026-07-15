# Claude Code

오늘 새로 반영할 Claude Code 버전은 `2.1.210`입니다. 오래 걸리는 작업의 진행 상태가 더 잘 보이고, background session과 worktree, plugin 연결의 안정성이 크게 개선되었습니다.

## GUI App

- 최신 저장 기준을 `2.1.209`에서 `2.1.210`으로 올렸습니다.
- 접힌 tool 요약에 경과 시간 표시가 추가되어, 긴 작업이 멈춘 것처럼 보이지 않습니다.
- 긴 응답을 받을 때 화면 전체를 계속 다시 그리지 않도록 바뀌어 반응성이 좋아졌습니다.
- 긴 대화 스크롤 중 화면이 튀는 현상, bash mode 입력 중 깜빡임, background session 재접속 때 escape 문자가 보이는 문제를 고쳤습니다.
- `claude attach`가 session 전환 중 실패하는 문제와 background agent가 끝났는데도 `/exit`가 실행 중이라고 경고하는 문제를 줄였습니다.

## CLI App

- npm `latest`와 `next`는 모두 `2.1.210`입니다.
- 잘못된 `Write(path)`, `NotebookEdit(path)`, `Glob(path)` permission rule을 시작할 때 경고합니다.
- 격리 worktree의 subagent가 main checkout에서 git 변경 명령을 실행할 수 있던 문제를 막았습니다.
- hook timeout을 사용자 거절로 잘못 처리하던 문제, background로 넘어간 `cd`가 적용됐다고 오인하던 문제, MCP 재동기화 때 plugin MCP server가 종료되던 문제를 고쳤습니다.
- 실패한 plugin cache 쓰기의 임시 파일, 종료된 background session의 worktree lock, background worker 재시작 반복 문제를 정리했습니다.
- subagent가 읽은 외부 내용으로부터 들어오는 간접 prompt injection 방어를 강화했고, binary와 시작 메모리 사용량도 각각 약 7 MB 줄였습니다.

## Sources

- [Claude Code CHANGELOG](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [Claude Code raw CHANGELOG](https://raw.githubusercontent.com/anthropics/claude-code/main/CHANGELOG.md)
- [npm @anthropic-ai/claude-code](https://www.npmjs.com/package/@anthropic-ai/claude-code)
