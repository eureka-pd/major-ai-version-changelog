# Claude Code

오늘 Claude Code는 새 안정 버전 `2.1.190`이 확인되었습니다. `.version`에 저장된 `2.1.186` 이후 `2.1.187`과 `2.1.190`이 새로 보고할 변경입니다.

## GUI App

- 최신 저장 기준을 `2.1.190`으로 올렸습니다.
- `2.1.190`은 별도 상세 항목 없이 버그 수정과 안정성 개선 릴리스로 공개되어 있습니다.
- `2.1.187`에서는 조직에서 제한한 모델을 model picker, `--model`, `/model`, `ANTHROPIC_MODEL`에서 더 명확히 막고 안내하도록 바뀌었습니다.
- fullscreen mode의 선택 메뉴에서 마우스 클릭을 지원하고, Ghostty의 Cmd+click URL 열기, `/btw` 이전 답변 이동, `/plugin` 정리 노출 같은 사용성 수정이 들어갔습니다.
- background jobs, channel 연결, subagent depth, leaked worktree registration, VS Code extension resume 같은 장시간 작업 안정성 문제가 다수 수정되었습니다.

## CLI App

- npm `@anthropic-ai/claude-code` latest도 `2.1.190`입니다. `next` 태그 `2.1.191`은 다음 채널이라 안정 버전 보고에는 포함하지 않았습니다.
- `sandbox.credentials` 설정이 추가되어 sandboxed command가 credential 파일이나 secret 환경변수를 읽지 못하게 막을 수 있습니다.
- `--resume`이 원래 `-p` 실행에서 모델 턴을 만들지 않았을 때 실패하던 문제를 고쳤습니다.
- `--json-schema`와 workflow `agent({schema})` 구조화 출력이 성공 후 무한 재호출되거나 후속 턴에서 불안정하던 문제가 수정되었습니다.
- remote MCP tool call이 5분 동안 응답 없이 멈추면 이제 계속 기다리지 않고 오류로 중단합니다.

## Sources

- [Claude Code CHANGELOG](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [Claude Code raw CHANGELOG](https://raw.githubusercontent.com/anthropics/claude-code/main/CHANGELOG.md)
- [npm @anthropic-ai/claude-code](https://www.npmjs.com/package/@anthropic-ai/claude-code)
