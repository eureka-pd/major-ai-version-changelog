# Codex
- 기준일: 2026-10-29 (Asia/Seoul)
- 확인 시각: 2026-10-29 04:13 KST
- 비교 기준: main의 기존 .version 및 2026-10-28 기록

## 확인 결과
**안정판 CLI 0.165.0**을 신규 확인했다. 공식 변경 로그 표기일은 2026-10-27, GitHub 발행 시각은 2026-10-27 20:09:38 UTC(10월 28일 05:09:38 KST)다.

- Google Cloud Vertex AI 공급자를 내장했고, 지원 모델은 대화 중 추론 강도를 바꿀 수 있다.
- 저장소별 세션 필터와 워크트리 디렉터리 그룹화를 추가했다. 새 프로필에서는 memory v2가 기본이며 외부 에이전트 메모리 가져오기를 지원한다.
- 중단·Plan 모드 전환 뒤 대기 메시지가 작업을 재시작하는 문제를 수정했다. Marketplace URL의 검사 대상과 실제 Git 접속 호스트가 달라질 수 있는 검증 빈틈도 수정했다.

GPT-6.1 Terra의 CLI 모델 목록 추가는 이번 버전에 포함되지만 모델 출시 공지는 전날 이미 기록했으므로 재공지하지 않는다. GUI 26.1007·모바일 1.2026.272 및 기존 공지 상태는 보존했다.

### 시험판 관찰(안정판과 별도)
**0.166.0-alpha.5**: 2026-10-28 04:43:10 UTC 발행. 릴리스 본문에는 버전 외 기능 설명이 없어 변경 기능을 추정하지 않는다. 안정판을 대체하거나 설치 권고로 취급하지 않았다.

## Sources
- [공식 변경 로그](https://developers.openai.com/codex/changelog) — 현재 ChatGPT Learn 변경 로그로 이동
- [0.165.0 릴리스](https://github.com/openai/codex/releases/tag/rust-v0.165.0)
- [0.166.0-alpha.5 시험판](https://github.com/openai/codex/releases/tag/rust-v0.166.0-alpha.5)
