# Claude Code 변경사항

기준일: 2026-10-08 (Asia/Seoul). 이전 기록 `2.1.292` 이후 안정 릴리스 1건을 새로 확인했습니다.

## GUI App / CLI App

### 2.1.293

- 공식 공개: 2026-10-07 18:10:20 UTC, 한국 시간 2026-10-08 03:10:20.
- 저장소의 GUI/CLI 공통 버전 표기를 유지하며, 이 번호는 Claude Code 패키지 기준입니다.
- Claude Haiku 5.5를 추가했습니다. Anthropic API의 기본 Haiku 모델이며 100만 토큰 문맥을 지원합니다.
- 대화 압축 이후 이미 끝낸 일을 취소하거나 반복하던 문제, 백그라운드 전환 중 보낸 메시지가 사라지던 문제를 수정했습니다.
- HTTP MCP 연결의 메모리 누수, 추론 노력 선택의 끝에서 반대쪽 값으로 넘어가던 문제, Chrome 연결 및 긴 원격 세션의 응답 표시를 개선했습니다.
- Bash로 파일을 읽을 때 경로별 규칙과 하위 CLAUDE.md가 누락되던 문제를 수정했습니다. Windows에서 명령 종료가 무관한 프로세스를 함께 끝낼 수 있던 문제도 고쳤습니다.
- 주의: 컨테이너 재시작으로 예약 작업이나 `/loop` 깨우기 정보가 유실됐을 때 클라우드 세션을 복구하던 2.1.290 수정이 되돌려졌습니다. 해당 상황에서는 세션이 계속 대기할 수 있습니다.

## 확인 기준

- 공식 CHANGELOG와 GitHub 최신 안정 릴리스가 모두 `2.1.293`입니다.
- 상태 파일에는 공식 공개 시각의 UTC 날짜를 기록합니다. 점검일과 출시일을 구분합니다.

## Sources

- [Claude Code 공식 변경 로그](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [Claude Code 2.1.293 공식 릴리스](https://github.com/anthropics/claude-code/releases/tag/v2.1.293)
