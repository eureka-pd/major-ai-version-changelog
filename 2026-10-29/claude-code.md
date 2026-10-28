# Claude Code
- 기준일: 2026-10-29 (Asia/Seoul)
- 확인 시각: 2026-10-29 04:13 KST
- 비교 기준: main의 기존 .version 및 2026-10-28 기록

## 확인 결과
**CLI 2.1.312**를 신규 확인했다. GitHub 릴리스 발행 시각은 2026-10-27 20:24:20 UTC(10월 28일 05:24:20 KST)다.

- 큰 CLAUDE.md·규칙 파일을 일부만 읽은 상태에서 전체 덮어쓰기를 시도하면 전체 읽기 또는 부분 편집을 요구하도록 보호했다.
- VS Code 로그인 직후 조직 관리 설정이 적용되지 않던 문제, 재개한 대화의 첫 응답 저장 문제를 수정했다.
- Cloud 전송 실패 후 동일 요청 재시도의 중복 실행과 Code Review의 오래된 PR 커밋 검토를 수정했다. 훅 동시 실행에도 상한을 적용했다.

실무상 파일 손실과 중복 작업을 줄이는 안정성 개선이다. GUI 2.1.300 등 별도 컴포넌트 기록은 그대로 유지했다. 설치·업데이트는 수행하지 않았다.

## Sources
- [공식 CHANGELOG](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [2.1.312 공식 릴리스](https://github.com/anthropics/claude-code/releases/tag/v2.1.312)
