# SUMMARY

오늘 새로 반영할 기준은 Claude Code `2.1.206`, Codex CLI `0.144.1`, Cursor `3.11`입니다. Codex의 ChatGPT desktop app 통합 소식도 새로 기록했으며, Antigravity는 저장된 최신 기준과 같아 중복 보고하지 않았습니다.

## Claude Code

### GUI App

- 최신 저장 기준을 `2.1.206`으로 올렸습니다.
- Claude in Chrome이 정식 제공되었고, background agent 상태와 완료·입력 요청 알림을 `claude agents`에서 더 분명하게 확인할 수 있습니다.
- background agent는 기본적으로 뒤에서 실행되며, worktree 작업을 마치면 commit, push, draft PR 생성까지 이어갈 수 있습니다.
- background session의 재연결, 중지, SSH 시작, 저메모리 안내, Remote Control 상태 동기화 문제가 여러 차례 수정되었습니다.
- agent 목록의 상태 표시와 완료 세션 정리가 개선되어 오래 실행한 작업을 관리하기 쉬워졌습니다.

### CLI App

- npm `@anthropic-ai/claude-code`의 기본 `latest`와 `next` 설치 버전은 `2.1.206`입니다.
- 별도 `stable` 태그는 `2.1.197`이며, 이 저장소는 기존처럼 기본 설치 경로인 `latest`를 기준으로 기록합니다.
- Claude Sonnet 5가 기본 모델이 되었고, 기본 1M-token context window를 지원합니다.
- 여러 slash skill을 한 명령에서 최대 5개까지 연속으로 불러올 수 있게 되었습니다.
- 기본 permission mode의 표시 이름이 `Manual`로 정리되었고, `AskUserQuestion`은 사용자가 별도로 설정하지 않으면 자동으로 넘어가지 않습니다.
- `/cd` 경로 자동완성과 과도하게 긴 `CLAUDE.md` 정리를 제안하는 `/doctor` 검사가 추가되었습니다.
- SSL 인증서, 네트워크 재시도, worktree 정리, background daemon과 hook 오류 처리 안정성이 개선되었습니다.

## Codex

### GUI App

- 숫자로 공개된 최신 Codex 앱 버전 저장 기준은 계속 `26.616`입니다.
- Codex가 macOS와 Windows의 ChatGPT desktop app 안에 통합되었습니다. 기존 프로젝트와 설정은 유지됩니다.
- Markdown과 code를 앱에서 직접 편집하고 선택 영역에 annotation을 붙여 수정 요청을 보낼 수 있습니다.
- sidebar에서 GitHub PR diff와 reviewer feedback을 함께 보고 Codex에게 수정 작업을 맡길 수 있습니다.
- 하나의 project에서 여러 repository를 함께 다룰 수 있습니다.
- Computer Use 속도, 작업 진행 표시, plugin 설정, mobile 연결과 SSH video rendering이 개선되었습니다.

### CLI App

- 최신 저장 기준을 `0.144.1`로 올렸습니다.
- remote plugin 기본 활성화, system proxy 지원, remote-control pairing code, Bedrock GPT-5.6 model, MCP tool search 기본 사용이 추가되었습니다.
- 사용량 reset credit 정보, `writes` app approval mode, MCP interactive authentication, 외부 host 인증 흐름이 추가되었습니다.
- Windows sandbox, Intel Mac Code Mode, connector 인증 갱신, WebSocket proxy와 `/review` branch picker가 개선되었습니다.
- `0.144.1`은 standalone installer와 macOS code-mode host의 설치·fallback 신뢰성을 보강한 patch입니다.
- `0.145.0-alpha.2`는 prerelease이므로 안정 버전 기준에는 포함하지 않았습니다.

### Mobile

- 최신 숫자 저장 기준은 ChatGPT for iOS `1.2026.167`입니다.
- 이번 확인에서 별도의 새 mobile version 번호는 없었습니다.

## Cursor

### GUI App

- 최신 저장 기준을 2026-07-10 Cursor `3.11`로 올렸습니다.
- main agent를 멈추지 않고 질문할 수 있는 side chat과 agent 대화 기록 검색이 추가되었습니다.
- project와 repository 선택기가 local, cloud, remote machine, multi-repo 흐름을 한곳에서 다루도록 개편되었습니다.
- cloud agent hook이 prompt, response, thought, subagent, compaction, turn 완료까지 관찰하고 제어할 수 있도록 확장되었습니다.
- `3.10`에서는 team MCP의 중앙 배포와 조직 그룹별 marketplace 접근 제어가 추가되었습니다.

### CLI App

- CLI 전용 새 안정 버전 번호는 확인되지 않았습니다.
- team MCP 배포 대상에 CLI가 포함되지만 별도 version baseline은 없어 `.version`의 CLI 값은 계속 `null`입니다.

## Antigravity

### GUI App

- 최신 저장 기준은 계속 Antigravity 2.0 `2.2.1`입니다.
- 공개 download bundle과 Hub release API 모두 `2.2.1`을 최신 버전으로 제공합니다.
- 새 GUI release는 확인되지 않았습니다.

### IDE App

- 최신 저장 기준은 계속 Antigravity IDE `2.1.1`입니다.
- IDE release API에서도 새 버전은 확인되지 않았습니다.

### CLI App

- Antigravity 2.0 제품군의 CLI baseline은 계속 `2.0`입니다.
- 별도 새 CLI patch version은 확인되지 않았습니다.

## Sources

- [Claude Code CHANGELOG](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [Claude Code raw CHANGELOG](https://raw.githubusercontent.com/anthropics/claude-code/main/CHANGELOG.md)
- [npm @anthropic-ai/claude-code](https://www.npmjs.com/package/@anthropic-ai/claude-code)
- [OpenAI Codex changelog](https://developers.openai.com/codex/changelog)
- [npm @openai/codex](https://www.npmjs.com/package/@openai/codex)
- [Cursor changelog](https://cursor.com/ko/changelog)
- [Google Antigravity changelog](https://antigravity.google/changelog)
- [Google Antigravity releases](https://antigravity.google/releases)
