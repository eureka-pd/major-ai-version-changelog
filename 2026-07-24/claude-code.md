# Claude Code

## GUI App

- Claude Code 공통 최신 기준이 `2.1.217`에서 `2.1.218`로 올라갔습니다.
- GUI 전용으로 따로 구분된 추가 release는 확인되지 않았습니다.

## CLI App

- `/code-review`가 백그라운드 서브에이전트로 실행됩니다. 검토 결과가 현재 대화를 덜 차지하고, 연속으로 입력한 slash command도 검토 대상으로 유지됩니다.
- MCP 서버 연결 실패 시 `claude mcp list`와 `/mcp`가 HTTP 상태와 오류 내용을 보여주며, 설정값의 앞뒤 공백도 경고합니다.
- Windows 경로가 잘못된 문자로 변환되어 파일을 못 찾는 문제, 붙여넣기 줄바꿈이 한 줄로 합쳐지는 문제, 대화 저장·재개 관련 오류가 수정됐습니다.
- 위험한 명령, 백그라운드 실행, 의심스러운 Windows 경로는 Auto 모드가 직접 판단하도록 바뀌어 불필요한 권한 창을 줄였습니다.
- 서브에이전트의 동시 실행 수는 기본 20개로 제한됩니다. 필요한 경우 `CLAUDE_CODE_MAX_CONCURRENT_SUBAGENTS`로 조정할 수 있습니다.

## Sources

- [Claude Code CHANGELOG](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [Claude Code raw CHANGELOG](https://raw.githubusercontent.com/anthropics/claude-code/main/CHANGELOG.md)
