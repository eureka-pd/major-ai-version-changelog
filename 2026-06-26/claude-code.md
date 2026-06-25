# Claude Code

오늘 Claude Code는 새 기본 설치 버전 `2.1.191`이 확인되었습니다. `.version`에 저장된 `2.1.190` 이후 새로 보고할 변경입니다.

## GUI App

- 최신 저장 기준을 `2.1.191`로 올렸습니다.
- `/clear` 이전 시점으로 대화를 되돌려 이어갈 수 있는 `/rewind` 지원이 추가되었습니다.
- 스트리밍 응답을 읽는 중 화면이 맨 아래로 튀는 문제와, tasks panel에서 멈춘 background agent가 다시 살아나는 문제가 수정되었습니다.
- 조직 정책으로 `/voice`가 비활성화된 경우 이제 단순 오류가 아니라 정책 제한임을 더 명확히 안내합니다.
- agent panel 스크롤, welcome splash 화면 overflow, Ghostty fullscreen Cmd+click URL 열기 같은 터미널 UI 문제가 수정되었습니다.
- 스트리밍 텍스트 업데이트를 100ms 단위로 묶어 CPU 사용량을 약 37% 줄였고, 긴 세션에서 terminal output cache로 메모리가 커지는 문제도 줄였습니다.

## CLI App

- npm `@anthropic-ai/claude-code`의 `latest` 기본 설치 버전도 `2.1.191`입니다. `next`도 같은 버전을 가리킵니다.
- comma-separated hook matcher 예: `"Bash,PowerShell"`가 조용히 동작하지 않던 문제가 수정되었습니다.
- `/permissions`의 Recently-denied 탭에서 거부 항목을 승인해도 닫을 때 사라지던 문제가 수정되었습니다.
- MDM 또는 file policy로 설정한 `forceRemoteSettingsRefresh`가 실제로 적용되고, stale proxy cache를 피하도록 설정 fetch에 `Cache-Control: no-cache`가 붙습니다.
- sandbox network permission dialog에서 한 번 허용한 host는 같은 세션 동안 다시 묻지 않도록 개선되었습니다.
- MCP server capability discovery, MCP OAuth discovery/token request가 일시적 네트워크 오류에서 짧게 재시도하도록 개선되었습니다.
- MCP HTTP 404 오류는 이제 URL과 MCP config 확인 안내를 같이 보여줍니다.

## Sources

- [Claude Code CHANGELOG](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [Claude Code raw CHANGELOG](https://raw.githubusercontent.com/anthropics/claude-code/main/CHANGELOG.md)
- [npm @anthropic-ai/claude-code](https://www.npmjs.com/package/@anthropic-ai/claude-code)
