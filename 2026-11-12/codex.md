# Codex
- 기준일: 2026-11-12 (Asia/Seoul)
- 확인 시각: 2026-11-12 04:16 KST
- 비교 기준: main의 기존 .version 및 2026-11-11 기록

## 신규 안정판 CLI 0.167.1
- 공식 변경 로그 날짜: **2026-11-10**.
- GitHub 게시: **2026-11-10 21:32:01 UTC** (한국 11월 11일 06:32).
- 릴리스 본문은 비교 링크만 제공한다. 연결된 공식 커밋과 실제 변경을 확인하면, Amazon Bedrock의 일반 Responses 요청에 도구 정의의 변경분을 전달하는 선택 기능을 추가한 업데이트다.
- 이 기능은 **기본적으로 꺼져 있으며** Bedrock 제공자로 제한된다. 대화 압축과 도구 추가·제거 처리를 지원하고 웹 검색 설정은 요청의 최상위에 유지한다. 모든 사용자의 기본 동작이 바뀌었다고 해석하지 않는다.

## 새 시험판 관찰
기존 0.169.0-alpha.7 이후 다음 시험판을 확인했다. 시각은 GitHub 게시 기준이다.
- **0.169.0-alpha.9**: 2026-11-10 22:09:09 UTC.
- **0.169.0-alpha.10**: 2026-11-11 03:33:09 UTC.
- **0.169.0-alpha.11**: 2026-11-11 10:11:06 UTC.
- **0.167.0-alpha.4.2**: 2026-11-11 01:29:15 UTC. 별도 버전 계열이다.

시험판에는 상세 기능 설명이 없어 안정판 변경으로 추정하지 않았다. 최신 시험판 관찰값은 **0.169.0-alpha.11**로 갱신했다. 기존 데스크톱 **26.1007**, iOS **1.2026.300**, 해당 날짜와 공지 상태는 유지했다.

## Sources
- [지정 공식 변경 로그](https://developers.openai.com/codex/changelog)
- [현재 공식 통합 변경 로그](https://learn.chatgpt.com/docs/changelog)
- [안정판 0.167.1](https://github.com/openai/codex/releases/tag/rust-v0.167.1)
- [공식 버전 비교](https://github.com/openai/codex/compare/rust-v0.167.0...rust-v0.167.1)
- [Bedrock 적용 범위 커밋](https://github.com/openai/codex/commit/ba8b40354160fa078cf36e24bb696d34100d8b1f)
- [시험판 alpha.9](https://github.com/openai/codex/releases/tag/rust-v0.169.0-alpha.9)
- [시험판 alpha.10](https://github.com/openai/codex/releases/tag/rust-v0.169.0-alpha.10)
- [시험판 alpha.11](https://github.com/openai/codex/releases/tag/rust-v0.169.0-alpha.11)
- [별도 시험판 0.167.0-alpha.4.2](https://github.com/openai/codex/releases/tag/rust-v0.167.0-alpha.4.2)
