# Claude Code

오늘 새로 반영할 Claude Code 버전은 `2.1.211`입니다. 권한 승인 화면의 보안을 강화하고, background agent와 여러 세션을 오래 실행할 때 생기던 오류를 폭넓게 고쳤습니다.

## GUI App

- 최신 저장 기준을 `2.1.210`에서 `2.1.211`으로 올렸습니다.
- 채팅 채널로 전달되는 권한 미리보기에서 방향 제어 문자, 보이지 않는 문자, 비슷하게 생긴 따옴표를 무력화해 승인 내용을 속여 보이게 만들기 어렵도록 했습니다.
- 잠자기에서 깨어난 뒤 여러 세션이 한꺼번에 로그아웃되거나, 유휴 웹 세션의 plugin MCP server가 다시 연결되지 않던 문제를 고쳤습니다.
- Chrome이 실행 중이 아닐 때 시작이 멈추는 문제, 원격·CLI 세션의 Chrome 파일 업로드 문제, Windows에서 설정 페이지가 열리지 않는 문제를 수정했습니다.
- 중지한 background session을 다시 열 때 빈 대화가 생기거나, 사용자가 종료한 agent가 다시 살아나 오래된 요청을 실행하던 문제를 막았습니다.
- 설정·통계·diff 화면이 늦게 나타나던 지연을 줄이고 terminal 화면 배치와 렌더링 성능을 개선했습니다.

## CLI App

- npm `latest`와 `next`는 모두 `2.1.211`입니다.
- `--forward-subagent-text`와 `CLAUDE_CODE_FORWARD_SUBAGENT_TEXT`를 추가해 `stream-json` 출력에 subagent의 텍스트와 thinking을 포함할 수 있습니다.
- sandbox 밖의 Bash 명령에 대해 `PreToolUse` hook이 `ask`를 반환하면 auto mode도 반드시 사용자 확인을 거치도록 고쳤습니다.
- 명시적으로 지정한 subagent 모델이 resume 또는 follow-up 뒤 부모 모델로 되돌아가던 문제를 수정했습니다.
- background agent가 아직 실행 중이면 실제 완료를 기다리고 현재 상태를 보고하도록 바꿔, 끝나지 않은 작업의 결과를 만들어 내는 문제를 줄였습니다.
- worktree에서 허용한 권한 규칙을 저장소 루트에 보관해 다른 세션과 worktree에서도 유지합니다.
- Bedrock, Vertex, Mantle, Foundry에서 system context의 마지막 블록을 매 요청마다 새 입력 토큰으로 청구하던 prompt caching 회귀를 고쳤습니다.

## Sources

- [Claude Code CHANGELOG](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [Claude Code raw CHANGELOG](https://raw.githubusercontent.com/anthropics/claude-code/main/CHANGELOG.md)
- [npm @anthropic-ai/claude-code](https://www.npmjs.com/package/@anthropic-ai/claude-code)
