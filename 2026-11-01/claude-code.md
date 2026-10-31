# Claude Code
- 기준일: 2026-11-01 (Asia/Seoul)
- 확인 시각: 2026-11-01 04:11 KST
- 비교 기준: main의 기존 .version 및 2026-10-31 기록

## 새 버전: 2.1.316
공식 발행 시각은 2026-10-31 01:01:35 UTC(10:01:35 KST)다. 공식 CHANGELOG의 최신 항목과 GitHub 정식 릴리스를 대조했다.

- 하위 에이전트의 기본 추론 강도를 별도로 지정하는 `CLAUDE_CODE_SUBAGENT_EFFORT`를 추가했다. 모델을 상속한 하위 에이전트가 다시 깨어날 때 메인 모델로 바뀌던 문제도 수정했다.
- macOS와 Linux에서 Claude Code가 스스로 종료된 뒤 셸 명령이 남아 실행되던 문제를 수정했다.
- 제한 모드에서 읽기 허용 규칙 때문에 작업 폴더 밖 파일이 업로드되던 문제를 수정했다.
- 클라우드 세션의 MCP 입력 양식을 화면에서 작성하거나 거절할 수 있게 했다.
- Opus 4.8 fast mode는 10월 30일부터 사용 중단 예고 상태이며 11월 30일 제거 예정이다. 제거 후 해당 요청은 일반 모드로 자동 전환되지 않고 오류를 반환한다고 안내한다. 현재 사용자의 모델 설정을 변경한 것은 아니다.

기존 GUI 값은 별도 배포 검증 없이 유지했다. 설치하지 않았다.

## Sources
- [공식 변경 로그](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [공식 정식 릴리스 2.1.316](https://github.com/anthropics/claude-code/releases/tag/v2.1.316)
