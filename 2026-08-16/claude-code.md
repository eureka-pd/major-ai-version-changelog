# Claude Code 변경사항

## GUI App

- 버전: `2.1.233` (이전: `2.1.232`)
- GitLab 병합 요청 URL을 `--worktree`와 에이전트 목록에서 바로 열 수 있고, 권한 확인 알림이 데스크톱·VS Code에서도 동작합니다.
- 클라우드 세션이 권한 대기 중 끊긴 것으로 표시되던 문제와 Windows `\??\` 경로 우회를 수정했습니다.
- 2.1.232에서 생긴 Windows Bash 권한 회귀를 되돌렸습니다.

## CLI App

- 버전: `2.1.233` (이전: `2.1.232`)
- Linux Bash 메모리 한도와 WebFetch 캐시 유지 시간을 설정할 수 있고, GitLab MR·게이트웨이 사용자 식별 전달을 추가했습니다.
- MCP 재연결 루프, 유휴 세션 CPU 점유, 번들 스킬 별칭 인식, self-hosted runner 시작 속도를 개선했습니다.
- 최신 모델에서는 Todo 도구가 기본으로 꺼지며, 공식 로그는 GUI와 CLI의 별도 빌드가 아닌 공통 릴리스로 게시합니다.

## Sources

- [Claude Code changelog](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
