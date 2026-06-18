# Claude Code

오늘 Claude Code의 새 제품 버전은 확인되지 않았습니다. 저장 기준은 `2.1.181` 그대로이고, 공개 GitHub changelog도 이제 `2.1.181` 상세 내용을 제공합니다.

## GUI App

- 최신 저장 기준: `2.1.181`
- 공개 changelog 상세 기준: `2.1.181`
- `/config key=value` 형식으로 prompt에서 설정을 바로 바꿀 수 있습니다. interactive, `-p`, Remote Control에서 모두 동작합니다.
- 긴 문단 streaming이 줄 단위로 더 자연스럽게 표시됩니다. 첫 줄바꿈 전까지 화면이 멈춘 것처럼 보이는 상황을 줄인 변경입니다.
- subagent panel은 idle subagent를 자동으로 숨기고, 목록 높이를 제한하며, footer keyboard hint를 더 분명하게 보여줍니다.
- MCP OAuth browser page가 Claude Code 스타일에 맞게 정리되고, 성공하면 자동으로 닫힙니다.
- welcome, focus, AskUserQuestion, copy/paste, `/stats`, transcript cleanup 등 UI와 세션 안정성 관련 문제가 다수 수정됐습니다.

## CLI App

- 최신 저장 기준: `2.1.181`
- 공개 changelog 상세 기준: `2.1.181`
- macOS sandbox에서 Apple Events를 허용하는 `sandbox.allowAppleEvents` opt-in 설정이 추가됐습니다.
- `CLAUDE_CLIENT_PRESENCE_FILE` 환경변수로 사용자가 해당 기기 앞에 있을 때 mobile push notification을 줄일 수 있습니다.
- bundled Bun runtime이 `1.4`로 올라갔습니다.
- API 연결이 thinking 중 끊기면 자동 재시도하도록 개선됐습니다.
- custom `ANTHROPIC_BASE_URL`, Foundry, AWS credential export, relative symlink 설정, Linux clipboard, Windows/OneDrive agent directory 등 환경별 오류가 수정됐습니다.

## Sources

- [Claude Code CHANGELOG](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [npm @anthropic-ai/claude-code](https://www.npmjs.com/package/@anthropic-ai/claude-code)
