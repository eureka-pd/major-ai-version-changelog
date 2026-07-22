# Claude Code

## GUI App

- Claude Code 공통 최신 기준이 `2.1.216`에서 `2.1.217`으로 올라갔습니다.
- GUI 전용으로 따로 구분된 추가 release는 확인되지 않았습니다.

## CLI App

- npm 최신 안정 버전이 `2.1.217`로 올라갔으며, 2026년 7월 22일 04:55 KST에 공개됐습니다.
- 입력창에서 `:heart:` 같은 이모지 단축어를 자동 완성할 수 있습니다. 필요하면 `emojiCompletionEnabled` 설정으로 끌 수 있습니다.
- 저장 공간 부족이나 세션 저장 비활성화 때문에 대화 기록을 못 쓰는 상황을 경고해, 기록이 조용히 사라지는 일을 줄였습니다.
- MCP 도구 출력이 잘린 뒤에도 전체 내용을 메모리에 붙잡아 두던 누수와 긴 대화 재개 관련 문제가 수정됐습니다.
- Windows 자동 업데이트 실패 시 실행 파일을 복구하고, 회사 네트워크의 인증서·프록시 설정을 Desktop 세션에서도 반영하도록 개선했습니다.
- 백그라운드 세션·심볼릭 링크 경로·worktree 격리를 더 안전하게 처리하며, 기본 동시 서브에이전트 수는 20개로 제한됩니다.

## Sources

- [Claude Code CHANGELOG](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [Claude Code raw CHANGELOG](https://raw.githubusercontent.com/anthropics/claude-code/main/CHANGELOG.md)
- [npm @anthropic-ai/claude-code](https://www.npmjs.com/package/@anthropic-ai/claude-code)
