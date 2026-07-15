# SUMMARY

오늘 새로 반영한 안정 기준은 Claude Code `2.1.210`과 Antigravity `2.3.0`입니다. Codex 안정판은 `0.144.4` 그대로이며 prerelease만 `0.145.0-alpha.13`으로 올렸습니다. Cursor는 `3.11`을 유지합니다.

## Claude Code

### GUI App

- 최신 저장 기준을 `2.1.209`에서 `2.1.210`으로 올렸습니다.
- 긴 tool 작업의 경과 시간을 보여주고, 응답 streaming 중 화면 전체를 다시 그리는 일을 줄였습니다.
- 긴 대화 스크롤, bash mode 깜빡임, background session 재접속과 `claude attach`가 더 안정적으로 바뀌었습니다.

### CLI App

- npm `latest`와 `next`는 모두 `2.1.210`입니다.
- 잘못된 permission rule을 시작할 때 경고하고, 격리 worktree의 subagent가 main checkout을 변경할 수 있던 문제를 막았습니다.
- hook timeout, background `cd`, plugin MCP 재연결, plugin cache 임시 파일과 worktree lock 문제를 고쳤습니다.
- 간접 prompt injection 방어를 강화하고 binary와 시작 메모리 사용량을 줄였습니다.

## Codex

### GUI App

- 최신 숫자 저장 기준은 계속 Codex 앱 `26.616`입니다.
- 2026-07-09 ChatGPT desktop app 통합 이후 새 GUI release는 확인되지 않았습니다.

### CLI App

- 안정 버전 최신 기준은 계속 `0.144.4`입니다.
- 사전 공개 테스트 빌드는 `0.145.0-alpha.11`에서 `0.145.0-alpha.13`으로 올라갔습니다.
- alpha는 안정판과 분리해 기록하며, 공개 changelog에 세부 변경 설명은 없습니다.

### Mobile

- 최신 저장 기준은 계속 ChatGPT for iOS `1.2026.188`입니다.
- 새 mobile release는 확인되지 않았습니다.

## Cursor

### GUI App

- 최신 저장 기준은 계속 Cursor `3.11`입니다.
- 새 GUI release는 확인되지 않았습니다.

### CLI App

- CLI 전용 새 안정 버전 번호는 확인되지 않았습니다.
- `.version`의 CLI 값은 계속 `null`입니다.

## Antigravity

### GUI App

- 최신 저장 기준을 Antigravity 2.0 `2.2.1`에서 `2.3.0`으로 올렸습니다.
- queued messages, 실행 방식 설정, `Send Now`, `.txt` 파일 첨부를 지원합니다.
- 시작 속도와 backend overload 복구를 개선하고 system theme을 기본값으로 따릅니다.
- `Cmd+F`, 큰 diff 렌더링, archive 뒤 background task, `/btw`, subagent 종료 뒤 멈춤 문제를 고쳤습니다.

### IDE App

- 최신 저장 기준은 계속 Antigravity IDE `2.1.1`입니다.
- 새 IDE release는 확인되지 않았습니다.

### CLI App

- 제품군 기준은 계속 `2.0`입니다.
- 설치 manifest의 별도 binary version은 계속 `1.1.2`입니다.
- CLI 전용 새 release는 확인되지 않았습니다.

## Sources

- [Claude Code CHANGELOG](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [Claude Code raw CHANGELOG](https://raw.githubusercontent.com/anthropics/claude-code/main/CHANGELOG.md)
- [npm @anthropic-ai/claude-code](https://www.npmjs.com/package/@anthropic-ai/claude-code)
- [OpenAI Codex changelog](https://developers.openai.com/codex/changelog)
- [npm @openai/codex](https://www.npmjs.com/package/@openai/codex)
- [Cursor changelog](https://cursor.com/ko/changelog)
- [Google Antigravity changelog](https://antigravity.google/changelog)
- [Google Antigravity releases](https://antigravity.google/releases)
- [Antigravity Hub release API](https://antigravity-hub-auto-updater-974169037036.us-central1.run.app/releases)
- [Antigravity IDE release API](https://antigravity-ide-auto-updater-974169037036.us-central1.run.app/releases)
- [Antigravity CLI manifest](https://antigravity-cli-auto-updater-974169037036.us-central1.run.app/manifests/darwin_arm64.json)
