# Claude Code 변경사항

기준일: 2026-10-11 (Asia/Seoul). 이전 기록 이후 안정 릴리스 1건을 새로 확인했습니다.

## GUI App / CLI App

### 2.1.296

- 이전 기록: `2.1.295`.
- 공식 공개: 2026-10-09 19:28:59 UTC, 한국 시간 2026-10-10 04:28:59. 점검일과 출시일은 다릅니다.
- 하위 에이전트별 자동 압축 시점(`autoCompactWindow`)과 워크플로 에이전트 공통 모델 설정을 추가했습니다. Read 도구는 필요할 때 큰 텍스트 파일을 한 번에 읽는 `allow_large` 옵션을 지원합니다.
- 관리형 훅의 차단·출력 수정 적용, 비활성화된 MCP 서버의 잘못된 시작, 게이트웨이 로그인 회귀를 수정했습니다.
- 공유 대화·디버그 로그의 비밀정보 가림 누락, 일부 Bash 명령의 승인 누락을 수정했습니다. UTF-8이 아닌 파일을 편집하면서 문자가 손상되는 경우에는 편집을 거부합니다.
- 백그라운드 전환 시 프롬프트 중복 실행, 재시작 후 완료된 턴 재실행, 자체 호스팅 러너의 동시 Git 작업 문제를 수정했습니다.
- 긴 코드 대화의 표시 응답성과 Windows의 PowerShell 권한 검사·MCP 종료 처리를 개선했습니다.
- 저장소의 GUI/CLI 공통 표기를 유지합니다. 이 번호는 Claude Code 패키지 기준입니다.

## 확인 기준

- 공식 CHANGELOG와 GitHub 최신 안정 릴리스가 모두 `2.1.296`입니다.
- 이미 기록한 2.1.295의 변경사항은 다시 집계하지 않습니다.

## Sources

- [Claude Code 공식 변경 로그](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [Claude Code 2.1.296 공식 릴리스](https://github.com/anthropics/claude-code/releases/tag/v2.1.296)
