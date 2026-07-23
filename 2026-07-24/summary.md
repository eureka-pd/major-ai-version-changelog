# SUMMARY

## Claude Code

### GUI App

- Claude Code 공통 최신 기준이 `2.1.217`에서 `2.1.218`로 올라갔습니다.
- GUI 전용으로 따로 구분된 추가 release는 확인되지 않았습니다.

### CLI App

- `/code-review`가 백그라운드 서브에이전트로 실행됩니다. 검토 결과가 현재 대화를 덜 차지하고, 연속으로 입력한 slash command도 검토 대상으로 유지됩니다.
- MCP 서버 연결 실패 시 HTTP 상태와 오류 내용을 보여주며, 설정값의 앞뒤 공백도 경고합니다.
- Windows 경로·붙여넣기·대화 저장과 재개 관련 오류가 수정됐습니다.
- 위험한 명령, 백그라운드 실행, 의심스러운 Windows 경로는 Auto 모드가 직접 판단하도록 바뀌어 불필요한 권한 창을 줄였습니다.
- 서브에이전트의 동시 실행 수는 기본 20개로 제한됩니다.

## Codex

### GUI App

- Codex Desktop이 `26.616`에서 `26.707`로 올라갔습니다. 이제 macOS와 Windows의 ChatGPT 데스크톱 앱 안에서 Codex를 사용할 수 있으며, 기존 Codex 앱의 프로젝트·설정·작업 방식은 유지됩니다.
- 앱에서 Markdown·코드를 바로 편집하고 선택 영역에 주석을 달아 수정 요청할 수 있습니다.
- PR Chat으로 GitHub pull request를 검토하고, 문맥을 보며 인라인 피드백과 patch를 처리할 수 있습니다.
- task·서브에이전트 진행 표시, 재개 시 권한 처리, Windows Computer Use와 설치 흐름이 개선됐습니다.

### CLI App

- 최신 안정 버전은 계속 `0.145.0`입니다. 새 CLI release는 확인되지 않았습니다.

### Mobile

- ChatGPT for iOS가 `1.2026.188`에서 `1.2026.195`로 올라갔습니다.
- Codex task 대화 안에서 Mermaid 다이어그램을 바로 보여주고, 입력 양식도 사용할 수 있습니다.
- task·host·workspace를 바꿀 때 전송하지 않은 프롬프트를 복원합니다.
- 최근 활동 기준 task 정렬, Fast 제어, 목표 재개, 받아쓰기와 iPad 탐색이 개선됐습니다.

## Cursor

### GUI App

- 최신 버전 번호는 계속 Cursor `3.11`입니다.
- 7월 22일 Cursor Router 공지 이후 새 changelog는 확인되지 않았습니다.

### CLI App

- CLI 전용 새 안정 버전 번호는 확인되지 않았습니다.
- `.version`의 CLI 값은 계속 `null`입니다.

## Antigravity

### GUI App

- 최신 저장 기준은 계속 Antigravity 2.0 `2.3.1`입니다.
- 새 GUI release는 확인되지 않았습니다.

### IDE App

- 최신 저장 기준은 계속 Antigravity IDE `2.1.1`입니다.
- 새 IDE release는 확인되지 않았습니다.

### CLI App

- 제품군 기준은 계속 `2.0`입니다.
- macOS ARM용 공식 설치 binary는 계속 `1.1.5`입니다.
- 새 CLI binary 또는 별도 변경 설명은 확인되지 않았습니다.

## Sources

- [Claude Code CHANGELOG](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [Claude Code raw CHANGELOG](https://raw.githubusercontent.com/anthropics/claude-code/main/CHANGELOG.md)
- [OpenAI Codex changelog](https://developers.openai.com/codex/changelog)
- [Cursor changelog](https://cursor.com/ko/changelog)
- [Google Antigravity changelog](https://antigravity.google/changelog)
- [Google Antigravity releases](https://antigravity.google/releases)
- [Antigravity Hub release API](https://antigravity-hub-auto-updater-974169037036.us-central1.run.app/releases)
- [Antigravity IDE release API](https://antigravity-ide-auto-updater-974169037036.us-central1.run.app/releases)
- [Antigravity CLI manifest](https://antigravity-cli-auto-updater-974169037036.us-central1.run.app/manifests/darwin_arm64.json)
