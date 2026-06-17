# Claude Code

오늘 Claude Code는 새 기준을 반영했습니다. npm `latest`는 `2.1.181`까지 올라갔고, 공개 GitHub changelog에는 `2.1.179`까지 상세 변경사항이 올라와 있습니다. 그래서 중복 방지 기준은 `2.1.181`로 올리고, 아래 설명은 공개 changelog에서 확인되는 `2.1.179` 내용만 다룹니다.

## GUI App

- 최신 저장 기준: `2.1.181`
- 공개 changelog 상세 기준: `2.1.179`
- 응답 스트리밍 중 연결이 끊겨도 부분 응답을 보존하도록 수정됐습니다. 예전처럼 raw error만 보이거나 spinner가 계속 도는 상황을 줄인 변경입니다.
- welcome 화면에서 여러 홍보 배너가 겹쳐 쌓이던 문제가 고쳐졌습니다. 이제 세션당 최대 하나만 보입니다.
- subagent 화면에서 Ctrl+O를 눌렀을 때 해당 subagent의 transcript가 제대로 보이지 않던 문제가 수정됐습니다.
- subagent/footer 패널에서 prompt 입력칸을 클릭했을 때 focus가 돌아오지 않던 문제도 고쳐졌습니다.

## CLI App

- 최신 저장 기준: `2.1.181`
- 공개 changelog 상세 기준: `2.1.179`
- WSL2의 Windows Terminal과 VS Code에서 mouse-wheel scrolling이 깨지던 회귀가 수정됐습니다.
- Linux에서 큰 디렉터리 트리를 대상으로 sandbox `denyRead`/`allowRead` glob을 걸면 Bash tool 설명이 지나치게 커져 세션을 쓰기 어려워지던 문제가 고쳐졌습니다.
- feedback survey가 턴 직후 한 자리 숫자 답변을 곧바로 세션 평점으로 잡아버리던 문제가 수정됐습니다.
- remote session에서 background task가 턴 사이에 계속 "still running"처럼 보이던 상태 표시 문제가 고쳐졌습니다.
- remote session의 plugin loading 성능이 개선됐습니다.

## Sources

- [Claude Code CHANGELOG](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [npm @anthropic-ai/claude-code](https://www.npmjs.com/package/@anthropic-ai/claude-code)
