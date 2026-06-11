# SUMMARY

오늘 새로 보고할 변화는 두 가지입니다. Claude Code가 `2.1.173`으로 올라갔고, Codex app이 `26.608`로 올라갔습니다. Cursor와 Antigravity는 저장된 최신 기준과 일치했습니다.

## Claude Code

### GUI App

- 최신 기준: `2.1.173` (2026-06-11)
- Fable 5 모델 이름의 1M context 표시를 잘못 처리하던 문제가 수정되었습니다.
- Windows sandbox 사용 시 불필요한 startup warning이 뜨던 문제가 수정되었습니다.
- `2.1.172`에서는 sub-agent가 다시 sub-agent를 만들 수 있게 되었고, marketplace plugin 검색, background/remote session 안정성, 긴 대화 성능이 개선되었습니다.

### CLI App

- 최신 기준: `2.1.173`
- npm 패키지도 `2.1.173`으로 확인되었습니다.
- CLI 사용자는 sub-agent 중첩, Bedrock region 자동 인식, remote/background session 안정화, 권한/모델 선택 관련 수정의 영향을 받습니다.

## Codex

### GUI App

- 최신 기준: Codex app `26.608` (2026-06-09), ChatGPT for iOS `1.2026.153` (2026-06-09)
- Codex app에 Claude Code와 Claude Cowork 설정을 가져오는 migration flow가 추가되었습니다.
- plugins 화면이 탭, marketplace, category filter, keyboard navigation 중심으로 개편되었습니다.
- Settings 검색 범위가 넓어졌고, goal timer 겹침, notification 과다 표시, review diff 정렬, Windows rendering 문제가 개선되었습니다.

### CLI App

- 최신 기준: Codex CLI `0.139.0` (2026-06-09)
- npm 기준도 `0.139.0`입니다.
- 오늘 새 CLI 버전은 없어 이전 CLI 변경사항을 반복하지 않았습니다.

## Cursor

### GUI App

- 최신 기준: `3.7`, changelog 날짜 `2026-06-10`
- 새 제품 버전 번호나 새 changelog 날짜는 확인되지 않았습니다.
- 2026-06-10 Bugbot 개선 항목은 이미 저장된 기준이라 반복 보고하지 않았습니다.

### CLI App

- CLI 전용 새 버전 번호는 확인되지 않았습니다.
- `/review` 관련 내용은 기존 보고 기준과 같습니다.

## Antigravity

### GUI App

- 최신 기준: Antigravity 2.0 `2.0.11`, Antigravity IDE `2.0.4`
- 공식 changelog 검색 결과와 release 기준에서 더 높은 `2.0.x` 버전은 확인되지 않았습니다.
- 오늘 새 GUI/IDE 보고 대상은 없습니다.

### CLI App

- CLI는 `2.0` 제품군 기준으로 유지합니다.
- CLI만의 별도 패치 번호는 오늘 확인되지 않았습니다.

## Sources

- [Claude Code CHANGELOG](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [npm @anthropic-ai/claude-code](https://www.npmjs.com/package/@anthropic-ai/claude-code)
- [OpenAI Codex changelog](https://developers.openai.com/codex/changelog)
- [npm @openai/codex](https://www.npmjs.com/package/@openai/codex)
- [Cursor changelog](https://cursor.com/ko/changelog)
- [Cursor 2026-06-10 Bugbot update](https://cursor.com/changelog/bugbot-updates-june-2026)
- [Google Antigravity changelog](https://antigravity.google/changelog)
- [Google Antigravity releases](https://antigravity.google/releases)
