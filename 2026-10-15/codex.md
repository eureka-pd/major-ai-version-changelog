# Codex 변경사항

기준일: 2026-10-15 (Asia/Seoul). 앱·CLI 새 버전은 없으며 모델 지원 상태 변경을 확인했습니다.

## 버전

- GUI `26.924` (2026-09-25), CLI `0.162.1` (2026-10-09), iOS `1.2026.272` (2026-10-07) 유지.
- CLI는 공식 변경 로그와 GitHub 최신 안정 릴리스를 대조했습니다. 알파판은 포함하지 않습니다.

## GPT-5.5 지원 종료 발효

- 공식 공지일: 2026-10-14.
- 발효: 2026-10-14 19:00 UTC / 2026-10-15 04:00 KST.
- ChatGPT 로그인으로 사용하는 Codex에서 GPT-5.5 지원이 종료됐습니다. OpenAI API와 API 키 인증 Codex 세션은 영향이 없습니다.
- 저장된 모델 기본값이나 작업이 `gpt-5.5`를 지정한다면, 플랜·클라이언트에서 제공하는 GPT-6.1 Sol 등 지원 모델로 변경해야 합니다. 사용자 설정을 실제로 변경하지는 않았습니다.
- 9월 14일의 기존 예고 기록은 보존하고, 이번 발효 공지를 별도 상태로 기록합니다. 새 모델 출시로 집계하지 않습니다.

## Sources

- [요청된 Codex 변경 로그](https://developers.openai.com/codex/changelog)
- [리디렉션된 공식 통합 변경 로그](https://learn.chatgpt.com/docs/changelog)
- [CLI 0.162.1 안정 릴리스](https://github.com/openai/codex/releases/tag/rust-v0.162.1)
