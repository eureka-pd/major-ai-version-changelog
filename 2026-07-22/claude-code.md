# Claude Code

## GUI App

- Claude Code 공통 최신 기준이 `2.1.215`에서 `2.1.216`으로 올라갔습니다.
- GUI 전용으로 따로 구분된 추가 release는 확인되지 않았습니다.

## CLI App

- npm `latest`와 `next`가 모두 `2.1.216`이며, 2026년 7월 21일 05:19 KST에 공개됐습니다.
- 파일 시스템 격리만 끄고 네트워크 외부 통제는 유지할 수 있는 `sandbox.filesystem.disabled` 설정이 추가됐습니다.
- 대화가 길어질수록 재개와 응답이 크게 느려지던 성능 문제가 수정됐습니다.
- OAuth 토큰이 세션 중 바뀌었을 때 자동 모드가 명령을 `HTTP 401`로 잘못 막던 문제가 해결됐습니다.
- 백그라운드 에이전트의 역할 복원, 격리 worktree, 세션 삭제와 재개 동작이 더 안전해졌습니다.
- 심볼릭 링크를 통한 workflow·예약 작업 쓰기, 권한 검사, Windows 경로와 PowerShell 명령 검증 등 보안 관련 오류가 다수 수정됐습니다.
- 세션 도중 바뀐 skill과 command가 재시작 없이 slash 메뉴에 나타나고, plugin skill 자동완성도 올바르게 표시됩니다.

## Sources

- [Claude Code CHANGELOG](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [Claude Code raw CHANGELOG](https://raw.githubusercontent.com/anthropics/claude-code/main/CHANGELOG.md)
- [npm @anthropic-ai/claude-code](https://www.npmjs.com/package/@anthropic-ai/claude-code)
