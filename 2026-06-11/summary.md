# SUMMARY

오늘 새로 보고할 변화는 세 가지입니다. Codex CLI가 `0.139.0`으로 올라갔고, Codex iOS 기능이 `1.2026.153`으로 갱신되었으며, Cursor는 `2026-06-10` Bugbot 개선 항목이 새로 올라왔습니다. Claude Code와 Antigravity는 저장된 최신 기준과 일치했습니다.

## Claude Code

### GUI App

- 최신 기준: `2.1.170`
- 새 버전은 없습니다.
- 직전 업데이트의 핵심은 새 모델 접근 안내와 VS Code 통합 터미널에서 시작한 세션 transcript 저장 문제 수정입니다.

### CLI App

- 최신 기준: `2.1.170`
- npm 패키지도 `2.1.170`으로 확인되었습니다.
- 오늘 새 CLI 변경사항은 없어 이전 내용을 반복하지 않았습니다.

## Codex

### GUI App

- 최신 기준: Codex app `26.602` (2026-06-04), ChatGPT for iOS `1.2026.153` (2026-06-09)
- 데스크톱 Codex app의 새 버전 번호는 없지만, iOS Codex 기능은 새로 갱신되었습니다.
- iOS에서 새 thread를 만들 때 branch 선택, worktree 생성, 환경 setup script 실행을 할 수 있습니다.
- profile 화면에 사용량 통계와 token 활동 차트가 추가되었습니다.
- 첨부 지원, side chat/queued prompt 표시, 메시지 스타일, Face ID, archived thread 탐색도 개선되었습니다.

### CLI App

- 최신 기준: Codex CLI `0.139.0` (2026-06-09)
- code mode에서 standalone web search를 직접 호출할 수 있습니다.
- 복잡한 tool/connector schema 보존이 좋아져 MCP tool 호환성이 개선되었습니다.
- `codex doctor` 진단 정보가 늘었고, plugin marketplace JSON/cache 동작이 좋아졌습니다.
- `resume --last`, `fork --last`, image edit file path 처리, thread reset 중 cloud requirement 보존, sandbox escalation/proxy 처리가 수정되었습니다.

## Cursor

### GUI App

- 최신 기준: `3.7`, changelog 날짜 `2026-06-10`
- 새 제품 버전 번호는 없지만 Bugbot 개선 항목이 새로 올라왔습니다.
- Bugbot은 review당 3배 이상 빨라지고, 비용은 22% 낮아졌으며, 더 많은 버그를 찾도록 개선되었습니다.
- push 전에 review를 실행할 수 있는 `/review` 명령이 추가되었습니다.

### CLI App

- CLI 전용 새 버전 번호는 확인되지 않았습니다.
- `/review` 명령은 명령 기반 검토 workflow에 영향을 주는 항목으로 기록했습니다.

## Antigravity

### GUI App

- 최신 기준: Antigravity 2.0 `2.0.11` (2026-06-03), Antigravity IDE `2.0.4` (2026-06-02)
- 공식 페이지와 번들 검색에서 더 높은 `2.0.x` 버전 번호는 확인되지 않았습니다.
- 검색 인덱스에는 antivirus 환경의 어두운 빈 화면 수정 신호가 보였지만, 버전 번호를 확정할 수 없어 새 버전으로 처리하지 않았습니다.

### CLI App

- CLI는 `2.0` 제품군 기준으로 유지합니다.
- CLI만의 별도 패치 번호는 오늘 확인되지 않았습니다.

## Sources

- [Claude Code CHANGELOG](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [npm @anthropic-ai/claude-code](https://www.npmjs.com/package/@anthropic-ai/claude-code)
- [OpenAI Codex changelog](https://developers.openai.com/codex/changelog)
- [Codex CLI 0.139.0 release](https://github.com/openai/codex/releases/tag/rust-v0.139.0)
- [npm @openai/codex](https://www.npmjs.com/package/@openai/codex)
- [Cursor changelog](https://cursor.com/ko/changelog)
- [Cursor 2026-06-10 Bugbot update](https://cursor.com/changelog/bugbot-updates-june-2026)
- [Google Antigravity changelog](https://antigravity.google/changelog)
- [Google Antigravity releases](https://antigravity.google/releases)
