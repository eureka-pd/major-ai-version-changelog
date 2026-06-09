# SUMMARY

오늘 새로 보고할 버전은 두 가지입니다. Claude Code는 `2.1.168`에서 `2.1.170`으로 올라갔고, Codex CLI는 `0.137.0`에서 `0.138.0`으로 올라갔습니다. Cursor와 Antigravity는 `.version`에 저장된 최신 기준과 공식 changelog 확인 결과가 일치했습니다.

## Claude Code

### GUI App

- 최신 기준: `2.1.170`
- `2.1.170`은 새 모델 접근 안내와 transcript 저장 문제 수정을 포함합니다.
- `2.1.169`는 `--safe-mode`, `/cd`, bundled skills 숨김 설정, managed MCP 정책, background agent, Remote Control, Windows/macOS 터미널 안정성 같은 운영 개선을 많이 담았습니다.
- 사용자가 체감할 변화는 문제 진단이 쉬워지고, 세션 이어하기와 background 작업이 더 안정적이 된 점입니다.

### CLI App

- 최신 기준: `2.1.170`
- CLI에서는 `--safe-mode`, `/cd`, `claude agents --json` 개선, transcript 저장 수정이 특히 중요합니다.
- 터미널에서 시작한 세션을 나중에 다시 찾거나 이어 쓰는 흐름이 더 안정적입니다.

## Codex

### GUI App

- 최신 기준: Codex app `26.602` (2026-06-04)
- 새 GUI 앱 버전은 없습니다.
- 이번 새 보고 대상은 GUI 앱이 아니라 CLI입니다.

### CLI App

- 최신 기준: Codex CLI `0.138.0` (2026-06-08)
- `/app` 명령으로 CLI thread를 Codex Desktop으로 넘길 수 있고, 로컬 이미지 파일 경로가 모델에 전달되어 이미지 후속 편집이 더 정확해집니다.
- reasoning effort 선택, app-server token 사용량 확인, v2 personal access token 인증, plugin JSON 출력이 개선되었습니다.
- `/goal`, forked thread 제목, TUI 표시, config 오류 메시지, 시작 환경 호환성, `AGENTS.md` 탐지도 더 안정화되었습니다.

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

- 최신 기준: Antigravity 2.0 `2.0.11` (2026-06-03), Antigravity IDE `2.0.4` (2026-06-02)
- Antigravity 2.0 `2.0.11`의 antivirus 환경 시작 문제와 Open IDE 버튼 관련 수정이 최신입니다.
- Antigravity IDE는 `2.0.4`가 계속 최신입니다.
- 오늘 Antigravity 쪽 신규 보고 대상은 없습니다.

### CLI App

- CLI는 `2.0` 제품군 기준으로 유지합니다.
- CLI만의 별도 패치 번호는 오늘 공식 changelog에서 확인되지 않았습니다.

## Sources

- [Claude Code CHANGELOG](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [npm @anthropic-ai/claude-code](https://www.npmjs.com/package/@anthropic-ai/claude-code)
- [OpenAI Codex changelog](https://developers.openai.com/codex/changelog)
- [Codex CLI 0.138.0 release](https://github.com/openai/codex/releases/tag/rust-v0.138.0)
- [npm @openai/codex](https://www.npmjs.com/package/@openai/codex)
- [Cursor changelog](https://cursor.com/ko/changelog)
- [Google Antigravity changelog](https://antigravity.google/changelog)
- [Google Antigravity releases](https://antigravity.google/releases)
