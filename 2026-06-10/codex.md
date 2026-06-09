# Codex

- 확인 결과: Codex CLI에 새 버전이 있습니다.
- 이전 저장 기준: Codex app `26.602`, Codex CLI `0.137.0`
- 최신 확인 기준: Codex app `26.602` (2026-06-04), Codex CLI `0.138.0` (2026-06-08)
- 중복 보고 방지 상태: CLI component를 `0.138.0`으로 저장했습니다.
- 출처: [OpenAI Codex changelog](https://developers.openai.com/codex/changelog), [Codex CLI 0.138.0 release](https://github.com/openai/codex/releases/tag/rust-v0.138.0), [npm @openai/codex](https://www.npmjs.com/package/@openai/codex)

## GUI App

- Codex app 최신 기준은 계속 `26.602`입니다.
- 2026-06-04 이후 새 GUI 앱 버전 번호는 공식 changelog 상단에 보이지 않았습니다.
- 이번 보고에서 새로 반영할 대상은 GUI 앱이 아니라 CLI입니다.

## CLI App

### `0.138.0` (2026-06-08)

- `/app` 명령으로 현재 CLI 작업 thread를 Codex Desktop으로 넘길 수 있게 되었습니다. macOS와 native Windows에서 CLI와 Desktop 사이 이동이 더 자연스러워졌습니다.
- 로컬 이미지 첨부와 이미지 생성 결과의 저장 경로가 모델에 전달됩니다. 후속 편집이나 파일 참조가 더 정확해집니다.
- reasoning effort 선택이 더 유연해졌고, 터미널이 일부 `Alt` 단축키를 놓쳐도 대체 입력을 사용할 수 있습니다.
- app-server 연동은 계정 token 사용량을 읽을 수 있고, CLI와 app-server 인증 흐름에서 v2 personal access token을 지원합니다.
- plugin 명령의 JSON 출력과 plugin 상세 정보가 더 풍부해졌습니다.
- `/goal`, forked thread 제목, TUI streaming 여백, config 쓰기 오류 메시지, 시작 환경 호환성, remote/symlink workspace의 `AGENTS.md` 탐지 등이 수정되었습니다.
- 실무적으로는 Desktop 연동, 이미지 기반 작업, plugin 자동화, 목표 workflow 안정성이 좋아진 업데이트입니다.
