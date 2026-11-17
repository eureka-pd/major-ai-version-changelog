# Claude Code
- 기준일: 2026-11-18 (Asia/Seoul)
- 새로 확인한 CLI: **2.1.326** (이전 2.1.325). GitHub 게시 표시는 11월 16일 22:11 UTC / 11월 17일 07:11 KST다.

## 핵심 변경
- 에이전트 팀을 켠 상태에서 Code Mode를 함께 사용할 수 있다. 이미 Code Mode를 켜 둔 경우 팀 세션도 해당 모드로 시작한다.
- 잘못된 도구 허용·차단 규칙을 시작 시 경고한다. 세션 도중 관리자 MCP 설정 파일이 생겨 서버를 더 이상 불러오지 않을 때도 이유를 표시한다.
- 충돌이나 메모리 부족 뒤 세션을 재개하면 대화가 일부 사라지던 문제를 고쳤다. 백그라운드 세션에 지정된 모델 게이트웨이를 다시 연결하지 못하면 모델 요청 전에 중단한다.
- GUI 버전 기록은 유지했다.

## 출처
- [공식 변경 로그](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [v2.1.326 릴리스](https://github.com/anthropics/claude-code/releases/tag/v2.1.326)
