# Claude Code 변경사항

## GUI App

- 버전: `2.1.234` (이전: `2.1.233`)
- GitLab 병합 요청 배지가 푸터·상태줄에 표시되고, claude.ai 사용량 한도가 풀리면 세션을 자동으로 이어갈 수 있습니다.
- Remote Control에서 계정·조직 전환 시 세션을 바로 멈추고, 권한 모드·effort를 연결된 클라이언트와 맞춥니다.
- Windows `\??\` 경로를 막고, 긴 세션의 네트워크 재확인·권한 답변 유실·마크다운 렌더링 문제를 수정했습니다.

## CLI App

- 버전: `2.1.234` (이전: `2.1.233`)
- `CLAUDE_CODE_PROJECT_DIR_NAME`으로 트랜스크립트 폴더 이름을 지정할 수 있고, 작업 중 `/permissions`·`/add-dir`를 열 수 있습니다.
- `/goal`은 복구 불가 오류에서 해제되며, 백그라운드 작업이 30분 이상이면 점검을 시작합니다.
- MCP 진단의 시크릿 노출을 줄이고, `claude-api` 스킬 컨텍스트 비용을 낮췄습니다. 공식 로그는 GUI와 CLI의 별도 빌드가 아닌 공통 릴리스로 게시합니다.

## Sources

- [Claude Code changelog](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
