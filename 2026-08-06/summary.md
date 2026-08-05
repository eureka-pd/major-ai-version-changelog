# SUMMARY

2026-08-06 확인 결과, Claude Code `2.1.222`와 Codex CLI `0.146.1`이 새로 기록되었습니다. Cursor와 Antigravity는 새 버전이나 공지가 없습니다.

## Claude Code

### GUI App

- 버전: `2.1.222`
- 작업트리 격리 세션과 하위 에이전트가 메인 체크아웃에서 파괴적인 Git 명령을 실행할 수 있던 문제를 수정했습니다. 이제 모든 세션 유형에서 파일 편집과 Bash 격리가 적용됩니다.
- 화면 읽기, 파일 감시, 웹 세션의 diff 표시 등 앱 사용 중 발생할 수 있던 오류와 접근성 문제를 개선했습니다.

### CLI App

- 버전: `2.1.222`
- 백그라운드 작업의 자동 허용 훅이 도구 제한을 우회하던 문제를 수정하고, 에이전트 간 메시지에도 권한 분류를 적용했습니다.
- HTTPS 프록시 환경의 시작 연결 검사, 이미 완료된 응답의 연결 오류 표시, MCP 서버별 사용량 과다 집계 문제를 수정했습니다.
- 푸시 뒤 생성한 PR 연결, 긴 `SendMessage` 요약 전송, 조직 제한 모델의 하위 에이전트 선택 등 협업 흐름의 오류를 바로잡았습니다.

## Codex

### GUI App

- 버전: `26.727`
- 이전 기록 이후 새 GUI 앱 버전은 확인되지 않았습니다.

### CLI App

- 버전: `0.146.1`
- 보안 역량이 높은 모델에서 자동 코드 리뷰를 실행할 때 더 안전한 기본값을 적용했습니다.
- 터미널에서 권한 변경 이유를 더 명확히 설명합니다.

### General

- 이전 기록 이후 새 일반 공지는 확인되지 않았습니다.

### Mobile

- 버전: `1.2026.202`
- 이전 기록 이후 새 모바일 앱 버전은 확인되지 않았습니다.

## Cursor

### GUI App

- 버전: `3.11`
- 이전 기록 이후 새 GUI 앱 버전은 확인되지 않았습니다.

### CLI App

- 현재 공개 변경 로그에서 새 CLI 버전은 확인되지 않았습니다.

## Antigravity

### GUI App

- 버전: `2.5.0`
- 이전 기록 이후 새 GUI 앱 버전은 확인되지 않았습니다.

### IDE App

- 버전: `2.1.1`
- 이전 기록 이후 새 IDE 버전은 확인되지 않았습니다.

### CLI App

- 버전: `2.0` (CLI), `1.1.10` (CLI Binary)
- 이전 기록 이후 새 CLI 또는 CLI Binary 버전은 확인되지 않았습니다.

## Sources

- [Claude Code changelog](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [OpenAI Codex changelog](https://developers.openai.com/codex/changelog)
- [Cursor changelog](https://cursor.com/ko/changelog)
- [Google Antigravity changelog](https://antigravity.google/changelog)
