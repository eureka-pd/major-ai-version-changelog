# Codex
- 기준일: 2026-11-13 (Asia/Seoul)
- 확인 시각: 2026-11-13 04:18 KST
- 비교 기준: main의 기존 .version 및 2026-11-12 기록

## 신규 안정판 CLI 0.167.2
- 공식 날짜는 **2026-11-11**, GitHub 게시 시각은 **2026-11-11 22:44:46 UTC**다.
- Google Cloud Vertex AI에서 도구 정의의 변경분을 전송하는 기능이 기본으로 켜졌다. 이전 요청과 같은 도구 정의를 매번 전부 보내는 대신 변경분을 전달한다.
- 기존 동작을 유지하려면 config.toml의 [features] 아래 incremental_tools_legacy_gcp = false로 설정한다. 이 설명은 설정 변경을 수행했다는 뜻이 아니다.

## 모바일 1.2026.307
공식 날짜는 **2026-11-10**이다. 전체 화면 입력창에 이미지·파일 붙여넣기와 음성 주석을 추가하고, 실행 중 클라우드 작업 재진입 및 메시지 표시·키보드 동작을 개선했다. 오늘 새로 확인한 항목이지 오늘 출시됐다는 의미는 아니다.

## 시험판 관찰
새로 확인한 시험판은 **0.170.0-alpha.1**, **0.170.0-alpha.2**, **0.169.0-alpha.11.1**, 별도 계열 **0.167.0-alpha.4.3**다. 최신 관찰값 alpha.2는 2026-11-12 01:30:28 UTC에 게시됐다. 상세 기능 설명은 없어 안정판 기능으로 추정하지 않았다. 기존 데스크톱 버전과 공지 상태는 보존했다.

## Sources
- [지정 공식 변경 로그](https://developers.openai.com/codex/changelog)
- [공식 통합 변경 로그](https://learn.chatgpt.com/docs/changelog)
- [CLI 0.167.2](https://github.com/openai/codex/releases/tag/rust-v0.167.2)
- [공식 릴리스 목록](https://github.com/openai/codex/releases)
- [시험판 alpha.2](https://github.com/openai/codex/releases/tag/rust-v0.170.0-alpha.2)
