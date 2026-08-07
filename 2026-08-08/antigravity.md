# Antigravity 변경사항

2026-08-08 확인 결과, Antigravity CLI Binary `1.1.11`이 새로 기록되었습니다.

## GUI App

- 버전: `2.5.0`
- 이전 기록 이후 새 GUI 앱 버전은 확인되지 않았습니다.

## IDE App

- 버전: `2.1.1`
- 이전 기록 이후 새 IDE 버전은 확인되지 않았습니다.

## CLI App

- 버전: `2.0` (CLI), `1.1.11` (CLI Binary)
- 선택형 Vim 편집 모드를 추가했습니다. 입력창, 댓글, diff에서 Vim 이동과 편집을 사용할 수 있습니다.
- `-p` 모드에서 `/usage`, `/quota`, `/credits`, `/model`, `/effort`, `/skills` 같은 읽기 전용 명령은 에이전트를 실행하지 않고 결과만 출력합니다.
- 플러그인의 켜짐·꺼짐 상태를 사용자 설정에만 저장해, 플러그인 업데이트가 기존 선택을 임의로 바꾸지 않게 했습니다.
- 빈 명령 허용 규칙이 모든 명령을 자동 승인할 수 있던 문제, 엄격 권한 모드의 자동 승인 문제, MCP 관리자 제어 누락 문제를 수정했습니다.

## Sources

- [Google Antigravity changelog](https://antigravity.google/changelog)
