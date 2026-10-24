# Claude Code

- 기준일: 2026-10-25 (Asia/Seoul)
- 확인 시각: 2026-10-25 04:20 KST
- 비교 기준: 직전 `.version` 및 2026-10-24 기록

## 새로 확인한 버전

- **2.1.310**: 2026-10-23 23:39 UTC / 10월 24일 08:39 KST 게시. 오늘 처음 기록했으며 오늘 출시라는 뜻은 아니다.
- 공식 CHANGELOG의 최신 버전과 GitHub 정식 릴리스가 일치한다. GUI 별도 버전 2.1.300은 보존했다.

## 핵심 변경

- Agent SDK·출력 모드에서 매우 큰 대화 기록을 압축할 때 메모리 사용을 개선했다. 긴 입력 오류 뒤 압축이 부족해 다시 실패하던 문제도 수정했다.
- Windows에서 Git Bash가 없고 훅 명령이 따옴표 문자열뿐일 때 권한 훅이 도구 실행을 통과시키던 문제를 수정했다. 심볼릭 링크 읽기 권한 화면에 실제 대상도 표시한다.
- VS Code의 계획 검토에서 ‘피드백을 보내고 계속 계획’ 버튼에 Enter를 눌렀을 때 계획이 승인되던 오류를 수정했다.
- Bedrock·Vertex·Foundry 및 텔레메트리 비활성 환경에도 Monitor 도구·플러그인 모니터를 제공한다.
- Enterprise 사용자 지정 역할에 Cloud sessions·Remote Control 권한을 추가하고, 관리자 활성화 시 해당 권한을 가진 역할과 확인 절차를 표시한다. 개인 SDK 세션이 자동으로 데스크톱에 나타난다는 의미는 아니다.

## Sources

- [공식 CHANGELOG](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [원문 읽기](https://raw.githubusercontent.com/anthropics/claude-code/main/CHANGELOG.md)
- [정식 2.1.310 및 게시 시각](https://github.com/anthropics/claude-code/releases/tag/v2.1.310)
