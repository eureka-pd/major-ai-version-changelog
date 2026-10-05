# Codex 변경사항

기준일: 2026-10-06 (Asia/Seoul). 이전 기록 이후 새로 확인한 안정 릴리스입니다.

## GUI App

- 버전: `26.924`; 변경 없음.

## CLI App

- 버전: `0.160.1` (이전 기록: `0.160.0`)
- Unix 계열 컴퓨터에서 Windows 원격 실행기에 연결해 MCP 도구 서버를 시작할 때, 직접 지정한 환경변수가 있어도 Windows 실행에 필요한 `SYSTEMROOT`, `TEMP`, `TMP`를 유지하도록 수정했습니다.
- 원격 Windows에서 도구 서버를 켤 때 필요한 시스템·임시 폴더 정보가 빠지지 않게 하는 안정성 수정입니다.
- GitHub 공식 안정 릴리스 게시 시각: 2026-10-05 18:29:37 UTC, 한국 시간 2026-10-06 03:29:37.
- 지정된 공식 변경 로그는 현재 ChatGPT Learn으로 연결됩니다. 점검 시 해당 페이지에서 `0.160.1` 항목은 확인되지 않아, 버전·수정 내역·게시 시각은 OpenAI 공식 GitHub 릴리스로 교차 확인했습니다.
- 알파 릴리스는 최신 안정 버전에 포함하지 않습니다.

## General / Mobile

- 모바일 `1.2026.258` 유지. 공식 변경 로그의 최상단 공지 날짜는 2026-09-29입니다.
- 과거 공지 보완: 공식 변경 로그에 따르면 `GPT-5.3-Codex-Spark` 연구 프리뷰는 2026-09-14 종료되어 데스크톱 앱·CLI·IDE 확장에서 사용할 수 없습니다. 해당 모델을 지정한 설정이나 스크립트는 지원 모델로 바꿔야 합니다.
- 위 종료 공지는 이번 점검에서 저장소에 보완한 과거 정보이며, 오늘 출시된 업데이트로 집계하지 않습니다.

## Sources

- [OpenAI Codex changelog](https://developers.openai.com/codex/changelog)
- [현재 공식 변경 로그](https://learn.chatgpt.com/docs/changelog)
- [Codex CLI 0.160.1 공식 릴리스](https://github.com/openai/codex/releases/tag/rust-v0.160.1)
- [원격 Windows MCP 환경변수 수정 PR](https://github.com/openai/codex/pull/51121)
