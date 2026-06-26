# Claude Code

오늘 Claude Code는 기본 설치 버전 `2.1.193`이 확인되었습니다. `.version`에 저장된 `2.1.191` 이후 새로 보고할 변경입니다.

## GUI App

- 최신 저장 기준을 `2.1.193`으로 올렸습니다.
- bash 모드 `!`에서 파일 경로 자동완성이 바로 뜨도록 개선되었습니다.
- MCP 서버에 로그인이 필요하면 시작할 때 `/mcp`로 안내하는 알림이 추가되었습니다.
- idle 상태의 background shell command를 메모리 압박 상황에서 자동 정리할 수 있게 되었습니다.
- `/login` 직후 `/model` 같은 UI가 오래된 빈 상태를 보여주던 문제가 수정되었습니다.
- background agent와 subagent 화면에서 중복 재개, 숨겨진 sibling agent, phantom subagent 같은 혼란스러운 동작이 수정되었습니다.
- marketplace plugin 이름이 바뀐 경우 설정을 새 이름으로 자동 반영합니다.

## CLI App

- npm `@anthropic-ai/claude-code`의 `latest` 기본 설치 버전은 `2.1.193`입니다.
- `next` 태그는 `2.1.195`를 가리키지만 기본 안정 설치 경로가 아니어서 이번 안정 기준에는 포함하지 않았습니다.
- `autoMode.classifyAllShell` 설정이 추가되어 Bash/PowerShell 명령 전체를 auto-mode classifier로 보낼 수 있습니다.
- auto-mode 거절 사유가 transcript, toast, `/permissions` recent denials에 남습니다.
- OpenTelemetry에 `claude_code.assistant_response` 로그 이벤트가 추가되었습니다. 기본은 redaction이며, prompt 로그를 이미 켠 배포에서는 응답 텍스트도 기록될 수 있으므로 필요하면 `OTEL_LOG_ASSISTANT_RESPONSES=0`으로 막아야 합니다.
- MCP `headersHelper` 인증은 401/403이 나오면 helper를 다시 실행하고 재연결합니다.
- `/add-dir`에서 이미 작업 디렉터리인 경로를 넣었을 때 안내가 더 명확해졌습니다.

## Sources

- [Claude Code CHANGELOG](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [Claude Code raw CHANGELOG](https://raw.githubusercontent.com/anthropics/claude-code/main/CHANGELOG.md)
- [npm @anthropic-ai/claude-code](https://www.npmjs.com/package/@anthropic-ai/claude-code)
