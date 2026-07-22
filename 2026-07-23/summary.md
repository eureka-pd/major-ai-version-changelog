# SUMMARY

## Claude Code

### GUI App

- Claude Code 공통 최신 기준이 `2.1.216`에서 `2.1.217`으로 올라갔습니다.
- GUI 전용으로 따로 구분된 추가 release는 확인되지 않았습니다.

### CLI App

- npm 최신 안정 버전이 `2.1.217`로 올라갔으며, 2026년 7월 22일 04:55 KST에 공개됐습니다.
- 입력창에서 `:heart:` 같은 이모지 단축어를 자동 완성할 수 있습니다. 필요하면 `emojiCompletionEnabled` 설정으로 끌 수 있습니다.
- 저장 공간 부족이나 세션 저장 비활성화 때문에 대화 기록을 못 쓰는 상황을 경고해, 기록이 조용히 사라지는 일을 줄였습니다.
- MCP 도구 출력이 잘린 뒤에도 전체 내용을 메모리에 붙잡아 두던 누수와 긴 대화 재개 관련 문제가 수정됐습니다.
- Windows 자동 업데이트 실패 시 실행 파일을 복구하고, 회사 네트워크의 인증서·프록시 설정을 Desktop 세션에서도 반영하도록 개선했습니다.
- 백그라운드 세션·심볼릭 링크 경로·worktree 격리를 더 안전하게 처리하며, 기본 동시 서브에이전트 수는 20개로 제한됩니다.

## Codex

### GUI App

- 최신 저장 기준은 계속 Codex 앱 `26.616`입니다.
- 새 GUI release는 확인되지 않았습니다.

### CLI App

- 최신 안정 버전은 계속 `0.145.0`입니다.
- 새 CLI release는 확인되지 않았습니다.

### Mobile

- 최신 저장 기준은 계속 ChatGPT for iOS `1.2026.188`입니다.
- 새 mobile release는 확인되지 않았습니다.

## Cursor

### GUI App

- 최신 버전 번호는 계속 Cursor `3.11`입니다.
- 7월 22일 Cursor Router 공지가 추가됐습니다. `Auto` 모드가 요청의 작업 종류와 복잡도를 보고 알맞은 모델로 자동 연결합니다.
- 품질 우선(Intelligence), 균형(Balance), 비용 우선(Cost) 중 방식을 고를 수 있으며, 관리자는 팀·그룹별 활성화, 기본값, 사용 모델을 제어할 수 있습니다.
- 이 기능은 데스크톱, 웹, iOS, CLI, SDK에서 사용할 수 있습니다. 별도 데스크톱 앱 버전은 발표되지 않았습니다.

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

- 제품군 기준은 계속 `2.0`이며, macOS ARM용 공식 설치 binary는 계속 `1.1.5`입니다.
- 새 CLI release 또는 binary 변경 설명은 확인되지 않았습니다.

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
