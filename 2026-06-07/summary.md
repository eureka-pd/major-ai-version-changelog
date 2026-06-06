# SUMMARY

오늘 새로 보고할 내용은 Claude Code `2.1.167` 업데이트와 Antigravity IDE `2.0.4` 업데이트입니다. Codex와 Cursor는 `.version` 기준으로 새 중복 보고 대상이 없습니다.

## Claude Code

### GUI App

- 최신 기준: `2.1.167`
- `2.1.167`은 버그 수정과 안정성 개선 릴리스입니다.
- `2.1.166`에서는 fallback 모델 설정, deny 규칙 glob 지원, cross-session messaging 권한 강화, thinking 비활성화 동작 개선, 업데이트 안내 개선, 이미지/원격 세션/터미널/PowerShell/macOS 프로세스 관련 안정성 수정이 포함됐습니다.
- 요지는 새 기능보다 장애 대응과 안정성 개선이 중심입니다.

### CLI App

- 최신 기준: `2.1.167`
- CLI 흐름에서도 fallback 모델, 권한 규칙, thinking 설정, `claude update`, `claude agents`, 터미널/PowerShell/macOS 관련 수정이 영향을 줍니다.
- 요지는 CLI가 모델 장애와 터미널 문제에 더 안정적으로 대응하도록 다듬어진 것입니다.

## Codex

### GUI App

- 최신 기준: Codex app `26.602` (2026-06-04)
- 새 GUI 앱 버전은 없습니다.
- 이미 기록된 프로필 인사이트, 공유 카드, Computer Use 시작 준비 상태, 브라우저/리뷰 UI 개선이 최신입니다.

### CLI App

- 최신 기준: Codex CLI `0.137.0` (2026-06-04)
- 새 CLI 버전은 없습니다.
- 이미 기록된 키바인딩, 검색 메뉴 붙여넣기, 관리 설정, 플러그인 JSON 출력, 원격 제어 개선이 최신입니다.

## Cursor

### GUI App

- 최신 기준: `3.7` (2026-06-05)
- 새 changelog 날짜나 새 버전은 없습니다.
- 이미 기록된 브라우저 디자인 모드의 여러 요소 선택과 음성 입력 개선이 최신입니다.

### CLI App

- CLI 전용 새 버전 번호는 확인되지 않았습니다.
- 오늘 Cursor 쪽 신규 보고 대상은 없습니다.

## Antigravity

### GUI App

- 최신 기준: Antigravity 2.0 `2.0.10` (2026-05-28), Antigravity IDE `2.0.4` (2026-06-02)
- Antigravity 2.0 본체는 새 버전이 없고 `2.0.10`이 계속 최신입니다.
- Antigravity IDE `2.0.4`는 Enterprise 계정 인증에서 빈 화면이 뜨는 문제를 고친 릴리스입니다.
- 요지는 2.0 본체가 아니라 IDE의 회사 계정 인증 문제를 고친 업데이트입니다.

### CLI App

- CLI는 `2.0` 제품군 기준으로 유지합니다.
- CLI만의 별도 패치 번호는 오늘 공식 changelog에서 확인되지 않았습니다.

## Sources

- [Claude Code CHANGELOG](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [OpenAI Codex changelog](https://developers.openai.com/codex/changelog)
- [Cursor changelog](https://cursor.com/ko/changelog)
- [Google Antigravity changelog](https://antigravity.google/changelog)
- [Google Antigravity releases](https://antigravity.google/releases?hl=en)
