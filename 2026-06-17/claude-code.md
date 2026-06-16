# Claude Code

오늘 새로 보고할 안정 버전은 `2.1.178`입니다. 이전 저장 기준은 `2.1.177`이었고, npm `latest`와 GitHub 공개 changelog 모두 `2.1.178`을 확인했습니다. npm `next`에는 `2.1.179`가 있지만, 안정 기준은 `latest`인 `2.1.178`로만 반영했습니다.

## GUI App

- 최신 저장 기준: `2.1.178`
- 권한 규칙에서 `Tool(param:value)` 형태로 도구 입력값까지 조건에 넣을 수 있습니다. 예를 들어 특정 모델을 쓰는 subagent만 막는 식의 세밀한 규칙을 만들 수 있습니다.
- 중첩된 `.claude/skills`, `.claude/workflows`, output style, agent 정의를 더 잘 처리합니다. 하위 폴더에 가까운 설정이 우선 적용되고, 이름이 겹치면 디렉터리 이름이 붙어 구분됩니다.
- `/doctor` 화면은 섹션 상태와 명령어 이름이 더 읽기 쉽게 정리됐습니다.
- Remote Control 연결 실패 메시지가 더 구체적입니다. 단순히 실패했다고만 보이지 않고, 기능 게이트, 상태 검사 실패, 오래된 권한, 조직 정책 중 어디에서 막혔는지 구분합니다.
- `/bug`는 설명 없이 제출할 수 없고, 모델 거절 문구를 GitHub 이슈 제목으로 쓰지 않도록 바뀌었습니다.
- VS Code에서는 CJK IME 후보창을 닫기 위해 Esc를 눌렀을 때 실행 중인 Claude 작업이 취소되던 문제가 수정됐습니다.

## CLI App

- 최신 저장 기준: `2.1.178`
- auto mode에서 subagent 시작도 분류기가 먼저 평가합니다. subagent가 검토 없이 막혀야 하는 작업을 요청하는 경로를 줄인 변경입니다.
- 오래된 websocket/OAuth 파일 디스크립터 환경변수를 상속한 CLI가 메모리 부족으로 충돌하던 문제를 고쳤습니다.
- Chrome 연결, nested skill 권한, subagent transcript/progress 표시, background session 상태 표시, compaction fallback model 처리 등 여러 안정성 문제가 수정됐습니다.
- custom API gateway 환경에서 `claude agents` worker가 `401 Invalid bearer token`으로 실패하던 문제도 고쳤습니다.
- vim mode undo는 빠르게 이어진 NORMAL/VISUAL 모드 동작을 하나로 뭉개지 않고 단계별로 되돌립니다.

## Sources

- [Claude Code CHANGELOG](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [npm @anthropic-ai/claude-code](https://www.npmjs.com/package/@anthropic-ai/claude-code)
