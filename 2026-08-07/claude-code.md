# Claude Code 변경사항

2026-08-07 확인 결과, Claude Code `2.1.223`이 새로 기록되었습니다.

## GUI App

- 버전: `2.1.223`
- 조직 관리자가 특정 GitHub 조직의 모든 플러그인 저장소를 한꺼번에 허용하거나 차단할 수 있습니다.
- 클라우드 세션을 로컬에서 계속하는 `/teleport` 안내를 추가했습니다.
- 재개한 세션, 파일 감시, Git 푸시 결과 처리에서 드물게 멈추거나 오류가 나는 문제를 수정했습니다.

## CLI App

- 버전: `2.1.223`
- 숨은 문자나 조작된 명령으로 Bash 권한 검사를 우회할 수 있던 문제를 차단했습니다.
- 워크플로 스크립트가 샌드박스 밖에서 코드를 실행할 수 있던 경로를 막았습니다.
- 에이전트 정의의 권한 우회 설정이 조직 정책을 무시하던 문제를 수정했습니다.
- `/review`는 현재 변경 또는 PR을 검토하는 `/code-review`의 별칭이 되었습니다.

## Sources

- [Claude Code changelog](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
