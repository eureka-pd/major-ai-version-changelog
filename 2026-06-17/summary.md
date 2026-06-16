# SUMMARY

오늘 새로 보고할 안정 버전은 Claude Code `2.1.178`과 Codex CLI `0.140.0`입니다. Codex app은 버전 번호가 바뀌지는 않았지만, 2026-06-16 공식 changelog에 EEA, UK, Switzerland 지역 제공 범위 공지가 추가되어 중복 방지 기준에 함께 반영했습니다. Cursor와 Antigravity는 저장된 최신 기준과 일치합니다.

## Claude Code

### GUI App

- 최신 저장 기준: `2.1.178`
- 권한 규칙에서 `Tool(param:value)` 형태로 도구 입력값까지 조건에 넣을 수 있습니다. 예를 들어 특정 모델을 쓰는 subagent만 막는 식의 세밀한 규칙을 만들 수 있습니다.
- 중첩된 `.claude/skills`, `.claude/workflows`, output style, agent 정의를 더 잘 처리합니다. 하위 폴더에 가까운 설정이 우선 적용되고, 이름이 겹치면 디렉터리 이름이 붙어 구분됩니다.
- `/doctor` 화면은 섹션 상태와 명령어 이름이 더 읽기 쉽게 정리됐습니다.
- Remote Control 연결 실패 메시지가 더 구체적입니다.
- `/bug`는 설명 없이 제출할 수 없고, 모델 거절 문구를 GitHub 이슈 제목으로 쓰지 않도록 바뀌었습니다.
- VS Code에서는 CJK IME 후보창을 닫기 위해 Esc를 눌렀을 때 실행 중인 Claude 작업이 취소되던 문제가 수정됐습니다.

### CLI App

- 최신 저장 기준: `2.1.178`
- auto mode에서 subagent 시작도 분류기가 먼저 평가합니다.
- 오래된 websocket/OAuth 파일 디스크립터 환경변수를 상속한 CLI가 메모리 부족으로 충돌하던 문제를 고쳤습니다.
- Chrome 연결, nested skill 권한, subagent transcript/progress 표시, background session 상태 표시, compaction fallback model 처리 등 여러 안정성 문제가 수정됐습니다.
- custom API gateway 환경에서 `claude agents` worker가 `401 Invalid bearer token`으로 실패하던 문제도 고쳤습니다.
- vim mode undo는 빠르게 이어진 NORMAL/VISUAL 모드 동작을 하나로 뭉개지 않고 단계별로 되돌립니다.

## Codex

### GUI App

- 최신 앱 버전 저장 기준: `26.609`
- 새 앱 버전 번호는 아직 없습니다.
- 2026-06-16 공식 changelog에는 EEA, UK, Switzerland 사용자에게 더 많은 Codex app 기능이 제공된다는 공지가 추가됐습니다.
- Computer Use, Codex Chrome extension, Memories, Chronicle 제공 범위가 핵심입니다.
- Memories는 해당 지역에서 기본값이 꺼져 있고, Chronicle은 macOS의 ChatGPT Pro 사용자를 위한 opt-in research preview로 제공됩니다.

### CLI App

- 최신 저장 기준: `0.140.0`
- npm `@openai/codex`의 `latest` 태그가 `0.140.0`으로 올라갔습니다.
- 공식 Codex changelog에는 `0.140.0` CLI 상세 항목이 아직 별도로 보이지 않습니다. 따라서 이번 문서에는 npm 안정 버전 상승만 기록했습니다.
- npm `alpha` 태그는 `0.141.0-alpha.3`입니다. pre-release이므로 안정 버전 보고 대상에는 넣지 않았습니다.

### Mobile

- 최신 저장 기준: ChatGPT for iOS `1.2026.153`
- 오늘 확인한 공식 changelog에서 모바일 새 버전 번호는 보이지 않았습니다.

## Cursor

### GUI App

- 최신 저장 기준: Cursor `3.7`, changelog date `2026-06-10`
- Cursor changelog 상단은 2026년 6월 10일 Bugbot 성능 개선 항목입니다.
- 이 항목은 이미 저장된 기준일과 같으므로 중복 보고하지 않았습니다.
- 2026년 6월 5일의 Cursor `3.7` 항목도 계속 최신 제품 버전 기준입니다.

### CLI App

- CLI 전용 새 안정 버전 번호는 확인되지 않았습니다.
- Cursor changelog는 `/review` 기반 Bugbot 실행이 Cursor 3.7+와 cursor.com/agents에서 가능하고, CLI 지원은 곧 추가될 예정이라고 안내합니다.

## Antigravity

### GUI App

- 최신 저장 기준: Antigravity 2.0 `2.1.4` (2026-06-11)
- 공개 사이트 번들에서 확인되는 최신 2.x 계열 버전도 `2.1.4`입니다.
- quota screen redesign, PDF attachment support, `/btw`, conversation search, breadcrumbs, nested subagents 관련 항목이 최신 기준으로 유지됩니다.

### IDE App

- 최신 저장 기준: Antigravity IDE `2.0.4` (2026-06-02)
- 공개 사이트 번들에서 `2.0.4`가 계속 확인됩니다.
- 최신 IDE changelog 항목은 enterprise account authentication blank screen fix 기준입니다.

### CLI App

- CLI는 Antigravity 2.0 제품군 기준으로 유지합니다.
- 별도 새 CLI 패치 버전 번호는 확인되지 않았습니다.

## Sources

- [Claude Code CHANGELOG](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [npm @anthropic-ai/claude-code](https://www.npmjs.com/package/@anthropic-ai/claude-code)
- [OpenAI Codex changelog](https://developers.openai.com/codex/changelog)
- [npm @openai/codex](https://www.npmjs.com/package/@openai/codex)
- [Cursor changelog](https://cursor.com/ko/changelog)
- [Google Antigravity changelog](https://antigravity.google/changelog)
- [Google Antigravity download](https://antigravity.google/download)
