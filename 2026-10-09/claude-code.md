# Claude Code 변경사항

기준일: 2026-10-09 (Asia/Seoul). 이전 기록 이후 안정 릴리스 1건을 새로 확인했습니다.

## GUI App / CLI App

### 2.1.294

- 이전 기록: `2.1.293`.
- 공식 공개: 2026-10-08 05:03:54 UTC, 한국 시간 2026-10-08 14:03:54.
- 명령문 형태로 작성한 `prompt`·`agent` 훅이 차단해야 할 작업을 허용하던 문제를 수정했습니다.
- Stop·SubagentStop의 지시형 `prompt` 훅 판단을 개선해, 빌드가 깨진 상태처럼 계속 작업해야 하는 상황에서 일찍 종료할 가능성을 줄였습니다.
- 저장소의 GUI/CLI 공통 표기를 유지합니다. 이 번호는 Claude Code 패키지 기준입니다.

## 확인 기준

- 공식 CHANGELOG와 GitHub 최신 안정 릴리스가 모두 `2.1.294`입니다.
- 출시일은 UTC 공개 날짜이며 점검일과 구분합니다. 이미 기록한 2.1.293의 변경사항은 재집계하지 않습니다.

## Sources

- [Claude Code 공식 변경 로그](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [Claude Code 2.1.294 공식 릴리스](https://github.com/anthropics/claude-code/releases/tag/v2.1.294)
