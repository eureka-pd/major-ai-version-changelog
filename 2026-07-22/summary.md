# SUMMARY

## Claude Code

### GUI App

- Claude Code 공통 최신 기준이 `2.1.215`에서 `2.1.216`으로 올라갔습니다.
- GUI 전용으로 따로 구분된 추가 release는 확인되지 않았습니다.

### CLI App

- npm `latest`와 `next`가 모두 `2.1.216`이며, 2026년 7월 21일 05:19 KST에 공개됐습니다.
- 파일 시스템 격리만 끄고 네트워크 외부 통제는 유지할 수 있는 `sandbox.filesystem.disabled` 설정이 추가됐습니다.
- 대화가 길어질수록 재개와 응답이 크게 느려지던 성능 문제가 수정됐습니다.
- OAuth 토큰이 세션 중 바뀌었을 때 자동 모드가 명령을 `HTTP 401`로 잘못 막던 문제가 해결됐습니다.
- 백그라운드 에이전트의 역할 복원, 격리 worktree, 세션 삭제와 재개 동작이 더 안전해졌습니다.
- 심볼릭 링크를 통한 workflow·예약 작업 쓰기, 권한 검사, Windows 경로와 PowerShell 명령 검증 등 보안 관련 오류가 다수 수정됐습니다.
- 세션 도중 바뀐 skill과 command가 재시작 없이 slash 메뉴에 나타나고, plugin skill 자동완성도 올바르게 표시됩니다.

## Codex

### GUI App

- 최신 숫자 저장 기준은 계속 Codex 앱 `26.616`입니다.
- 새 GUI release는 확인되지 않았습니다.

### CLI App

- 안정 버전이 `0.144.6`에서 `0.145.0`으로 올라갔으며, 2026년 7월 22일 03:21 KST에 공개됐습니다.
- 대화 기록을 페이지 단위로 관리해 재개·검색·이름 저장·서브에이전트·메모리를 더 효율적으로 다루는 실험 기능이 추가됐습니다.
- `/import`가 Cursor와 Claude Code의 설정, MCP 서버, plugin, session, command, 프로젝트 메모리까지 가져올 수 있게 확장됐습니다.
- Amazon Bedrock 로그인과 사용자 지정 endpoint·인증을 지원하며, Bedrock 기본 모델은 GPT-5.6 Sol입니다.
- 오디오 입력·도구 출력과 실시간 V3 대화를 지원하고, opt-in multi-agent V2는 안정화 단계로 올라갔습니다.
- 긴 대화의 화면 갱신 속도, MCP 시작·인증, Windows sandbox, 승인·삭제 명령 안전성이 개선됐습니다.
- 사전 공개 채널도 `0.145.0-alpha.25`에서 `0.145.0-alpha.29`로 올라갔습니다. 이 빌드는 안정판보다 먼저 2026년 7월 21일 20:49 KST에 공개됐고 별도 설명은 없습니다.

### Mobile

- 최신 저장 기준은 계속 ChatGPT for iOS `1.2026.188`입니다.
- 새 mobile release는 확인되지 않았습니다.

## Cursor

### GUI App

- 최신 버전 번호는 계속 Cursor `3.11`입니다.
- 7월 17일 Slack 개선 공지 이후 새 changelog는 확인되지 않았습니다.

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
- macOS ARM용 공식 설치 binary는 `1.1.4`에서 `1.1.5`로 올라갔습니다.
- 새 binary는 2026년 7월 21일 10:08 KST에 배포됐지만 별도 변경 설명은 확인되지 않았습니다.

## Sources

- [Claude Code CHANGELOG](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [Claude Code raw CHANGELOG](https://raw.githubusercontent.com/anthropics/claude-code/main/CHANGELOG.md)
- [npm @anthropic-ai/claude-code](https://www.npmjs.com/package/@anthropic-ai/claude-code)
- [OpenAI Codex changelog](https://developers.openai.com/codex/changelog)
- [Codex CLI 0.145.0 release](https://github.com/openai/codex/releases/tag/rust-v0.145.0)
- [Codex CLI 0.145.0-alpha.29 release](https://github.com/openai/codex/releases/tag/rust-v0.145.0-alpha.29)
- [npm @openai/codex](https://www.npmjs.com/package/@openai/codex)
- [Cursor changelog](https://cursor.com/ko/changelog)
- [Google Antigravity changelog](https://antigravity.google/changelog)
- [Google Antigravity releases](https://antigravity.google/releases)
- [Antigravity Hub release API](https://antigravity-hub-auto-updater-974169037036.us-central1.run.app/releases)
- [Antigravity IDE release API](https://antigravity-ide-auto-updater-974169037036.us-central1.run.app/releases)
- [Antigravity CLI manifest](https://antigravity-cli-auto-updater-974169037036.us-central1.run.app/manifests/darwin_arm64.json)
