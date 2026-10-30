# Claude Code
- 기준일: 2026-10-31 (Asia/Seoul)
- 확인 시각: 2026-10-31 04:14 KST
- 비교 기준: main의 기존 .version 및 2026-10-30 기록

## 새 버전: 2.1.314
공식 발행 시각은 2026-10-30 01:06:26 UTC(10:06:26 KST)다. 이번 확인에서 새로 기록한 버전이며 설치하지 않았다.

- 작업 디렉터리 밖의 파일 쓰기를 차단하는 설정을 추가했다. 모든 권한 모드에서 Write·Edit·NotebookEdit에 적용된다.
- VS Code와 Claude Desktop의 Code 탭에서 20만 토큰 이상 대화를 유휴 시간에 요약하는 기능을 추가했다. 프롬프트 캐시가 만료되면 다음 메시지에 이 요약을 사용한다.
- 많은 하위 에이전트를 실행하는 긴 SDK·비대화형 작업의 메모리 사용을 줄였다.
- 이어서 실행한 worktree에 샌드박스 보호가 적용되지 않던 문제와 차단된 도구 호출이 실행된 것처럼 표시되던 문제를 수정했다.
- macOS의 일부 git grep 명령에 C 로캘을 사용하도록 바꿨다. UTF-8이 아닌 파일에서 보고된 정규식 라이브러리 메모리 누수를 피하기 위한 변경이다.

기존 GUI 버전 값은 별도 배포 확인 없이 바꾸지 않았다. 새 설정 추가가 사용자의 설정을 자동으로 켰다는 의미는 아니다.

## Sources
- [공식 변경 로그](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [공식 릴리스 2.1.314](https://github.com/anthropics/claude-code/releases/tag/v2.1.314)
