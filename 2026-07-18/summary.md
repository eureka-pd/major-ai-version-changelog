# SUMMARY

오늘 새로 반영한 안정 기준은 Claude Code `2.1.212`와 Antigravity `2.3.1`입니다. Codex 안정판은 `0.144.5`를 유지하고 prerelease만 `0.145.0-alpha.22`까지 올렸으며, Cursor는 `3.11`을 유지합니다.

## Claude Code

### GUI App

- 최신 저장 기준을 `2.1.211`에서 `2.1.212`로 올렸습니다.
- `/fork`는 대화를 별도 background session으로 복사하고, 기존 in-session subagent 동작은 `/subtask`로 분리됐습니다.
- `/resume`에서 과거 세션을 골라 background로 다시 시작할 수 있고, 오래 걸리는 MCP 호출은 자동으로 background로 이동합니다.
- background session 재접속, 입력 대기 상태 표시, 좁은 diff와 승인 화면 배치 문제를 개선했습니다.

### CLI App

- npm `latest`와 `next`는 모두 `2.1.212`입니다.
- auto mode 초기화 명령과 WebSearch·subagent 반복 실행 제한을 추가했습니다.
- plan mode의 무승인 파일 변경과 worktree 심볼릭 링크를 통한 저장소 밖 파일 생성을 막았습니다.
- SIGTERM의 자식 프로세스 정리, Windows background 실행, web search 재시도와 agent 메시지 토큰 사용을 개선했습니다.

## Codex

### GUI App

- 최신 숫자 저장 기준은 계속 Codex 앱 `26.616`입니다.
- 새 GUI release는 확인되지 않았습니다.

### CLI App

- 안정 버전 최신 기준은 계속 `0.144.5`입니다.
- 사전 공개 테스트 빌드는 `0.145.0-alpha.18`에서 `0.145.0-alpha.22`로 올라갔습니다.
- alpha 빌드는 안정판과 분리해 추적하며, 별도 변경 설명은 공개되지 않았습니다.

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

- 최신 저장 기준을 Antigravity 2.0 `2.3.0`에서 `2.3.1`로 올렸습니다.
- 비어 있거나 형식이 잘못된 설정 파일 때문에 앱이 시작되지 않던 문제를 고쳤습니다.
- 새 기능보다 시작 안정성을 다듬은 단일 patch release입니다.

### IDE App

- 최신 저장 기준은 계속 Antigravity IDE `2.1.1`입니다.
- 새 IDE release는 확인되지 않았습니다.

### CLI App

- 제품군 기준은 계속 `2.0`이고 설치 binary는 `1.1.3`입니다.
- 새 CLI release는 확인되지 않았습니다.

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
