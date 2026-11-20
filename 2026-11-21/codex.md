# Codex
- 기준일: 2026-11-21 (Asia/Seoul)
- CLI 안정판: **0.170.0 → 0.171.0**, 공식 변경 로그 날짜 11월 20일.
- CLI 시험판: **0.172.0-alpha.2 → 0.173.0-alpha.1**. 태그에서 상세 변경 설명은 확인하지 못했다.
- 데스크톱·모바일은 신규 버전 미확인.

## 안정판 변경
- GPT-6.2 Sol과 Astra가 CLI 모델 목록에 추가됐고 목록 기본값은 Sol이다.
- 터미널 워크스페이스를 기본 활성화했다. 메인 대화 옆에서 문서·이미지 미리보기와 하위 에이전트 기록을 열 수 있다.
- 기존 앱 서버에서 비대화형 실행을 시작하거나 재개하는 `codex exec --remote <ADDR>`와 터미널 원격 연결 관리 명령이 추가됐다.
- 대화를 전환하거나 재개할 때 입력 초안과 대기 중인 후속 메시지를 원래 스레드에 보존하도록 수정했다.

## 출처
- [OpenAI · 공식 변경 로그](https://developers.openai.com/codex/changelog)
- [OpenAI · 안정판 태그](https://github.com/openai/codex/releases/tag/rust-v0.171.0)
- [OpenAI · 시험판 태그](https://github.com/openai/codex/releases/tag/rust-v0.173.0-alpha.1)
