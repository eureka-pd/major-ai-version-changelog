# Claude Code

- 기준일: 2026-10-24 (Asia/Seoul)
- 확인 시각: 2026-10-24 04:15 KST
- 비교 기준: 직전 `.version` 및 2026-10-23 기록

## 새로 확인한 버전

- **2.1.309**: 2026-10-22 22:18 UTC / 10월 23일 07:18 KST 게시.
- 공식 CHANGELOG와 정식 릴리스가 일치한다. 기존 GUI 별도 버전은 변경하지 않았다.

## 핵심 변경

- macOS·Linux에서 셸 시작 파일이 샌드박스 밖에서 실행되던 문제, 심볼릭 링크를 통한 쓰기 제한 누락, MCP 설정 파일 변경 허점을 수정했다.
- 분할 화면의 팀원이 리더의 도구 금지 규칙을 제대로 이어받고, SDK·출력 모드에서 꺼 둔 MCP 서버가 권한 대화 뒤 다시 연결되지 않도록 했다.
- 데스크톱 연결 갱신 시 메시지 유실, 큰 CLAUDE.md로 인한 반복 압축, 재개 뒤 세션 이름 문제를 수정했다.
- `sed -i`는 실제 셸 명령으로 실행되며 `/rewind`로 복원되지 않는다. 기존 작업 흐름에서 주의할 변경이다.
- `claude ultrareview`는 작업 폴더 신뢰 확인을 요구한다.

## Sources

- [공식 CHANGELOG](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [정식 2.1.309 릴리스 및 게시 시각](https://github.com/anthropics/claude-code/releases/tag/v2.1.309)
