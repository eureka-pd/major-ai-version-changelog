# SUMMARY

오늘 새로 반영할 기준은 Claude Code `2.1.193`, Codex의 2026-06-25 일반 changelog 항목, Antigravity 2.0 `2.2.1`, Antigravity IDE `2.1.1`입니다. Cursor는 저장된 최신 기준과 같아서 중복 보고하지 않았습니다.

## Claude Code

### GUI App

- 최신 저장 기준을 `2.1.193`으로 올렸습니다.
- bash 모드 `!`에서 파일 경로 자동완성이 바로 뜨도록 개선되었습니다.
- MCP 서버에 로그인이 필요하면 시작할 때 `/mcp`로 안내하는 알림이 추가되었습니다.
- idle 상태의 background shell command를 메모리 압박 상황에서 자동 정리할 수 있게 되었습니다.
- `/login` 직후 `/model` 같은 UI가 오래된 빈 상태를 보여주던 문제가 수정되었습니다.
- background agent와 subagent 화면에서 중복 재개, 숨겨진 sibling agent, phantom subagent 같은 혼란스러운 동작이 수정되었습니다.
- marketplace plugin 이름이 바뀐 경우 설정을 새 이름으로 자동 반영합니다.

### CLI App

- npm `@anthropic-ai/claude-code`의 `latest` 기본 설치 버전은 `2.1.193`입니다.
- `next` 태그는 `2.1.195`를 가리키지만 기본 안정 설치 경로가 아니어서 이번 안정 기준에는 포함하지 않았습니다.
- `autoMode.classifyAllShell` 설정이 추가되어 Bash/PowerShell 명령 전체를 auto-mode classifier로 보낼 수 있습니다.
- auto-mode 거절 사유가 transcript, toast, `/permissions` recent denials에 남습니다.
- OpenTelemetry에 `claude_code.assistant_response` 로그 이벤트가 추가되었습니다. 기본은 redaction이며, prompt 로그를 이미 켠 배포에서는 응답 텍스트도 기록될 수 있으므로 필요하면 `OTEL_LOG_ASSISTANT_RESPONSES=0`으로 막아야 합니다.
- MCP `headersHelper` 인증은 401/403이 나오면 helper를 다시 실행하고 재연결합니다.
- `/add-dir`에서 이미 작업 디렉터리인 경로를 넣었을 때 안내가 더 명확해졌습니다.

## Codex

### GUI App

- 최신 앱 버전 저장 기준은 계속 `26.616`입니다.
- 새 버전 번호는 없지만 Codex Remote가 일반 제공 상태가 되었습니다.
- ChatGPT 모바일 앱, ChatGPT 데스크톱 앱, 웹에서 Codex를 사용할 수 있고, GitHub repository 연결, PR 생성, 이미지/로그 기반 작업, Slack/Linear/Notion/Jira/Dropbox 연동 흐름을 공식적으로 안내합니다.
- DigitalOcean plugin으로 Droplet을 만들고 SSH를 구성한 뒤 Codex를 원격 개발 환경에 연결할 수 있습니다.

### CLI App

- 최신 저장 기준은 계속 `0.142.2`입니다.
- npm `@openai/codex`의 `latest` 안정 태그도 `0.142.2`입니다.
- `alpha`는 `0.143.0-alpha.25`까지 올라왔지만 prerelease 채널이므로 안정 버전 보고에는 포함하지 않았습니다.
- 공개 Codex changelog에는 이번 안정 CLI 패치 상세 항목이 별도 노출되지 않았습니다.

### Mobile

- 최신 저장 기준은 ChatGPT for iOS `1.2026.167`입니다.
- OpenAI Codex changelog의 최신 모바일 항목도 2026-06-22 `1.2026.167`입니다.

## Cursor

### GUI App

- 최신 저장 기준: Cursor `3.9`
- 최신 changelog 항목도 2026-06-22 `3.9`입니다.
- `Cursor Customize`에서 플러그인, skills, MCP, subagents, rules, commands, hooks를 한 화면에서 관리하는 변경은 기존 최신 기준으로 유지됩니다.
- Marketplace leaderboard, plugin canvas, GitLab/BitBucket/Azure DevOps 플러그인 repository 가져오기 지원도 기존 최신 기준입니다.

### CLI App

- CLI 전용 새 안정 버전 번호는 확인되지 않았습니다.
- 별도 CLI baseline 변경이 없어 `.version`의 CLI 값은 계속 `null`로 유지합니다.

## Antigravity

### GUI App

- 최신 저장 기준을 Antigravity 2.0 `2.2.1`로 올렸습니다.
- 새 내장 `Antigravity Guide` skill이 추가되어 Antigravity 관련 질문에 제품 사용 안내를 더 잘 제공합니다.
- markdown code/diff block에서 C++, Python, Protobuf syntax highlighting을 지원합니다.
- sidebar file viewer와 artifact viewer에서 `.mp3`, `.wav`, `.ogg`, `.m4a` audio file을 렌더링하고 재생할 수 있습니다.
- Appearance 설정에 `Conversation Width`가 추가되어 대화 패널 폭을 Default, Narrow, Wide로 조정할 수 있습니다.
- workspace file search가 정확한 prefix뿐 아니라 substring도 찾도록 개선되었습니다.
- OAuth token refresh 결과를 OS keyring에 자동 저장해 인증 요청 반복을 줄입니다.
- 권한 요청 dialog가 실행하려는 action/command 설명을 더 분명하게 보여줍니다.
- breadcrumb/file tree 이동, sidebar resizing, slash command autocomplete, high-frequency file write 상황에서 lag와 flicker가 줄었습니다.
- workspace context가 history page 이동 중 사라지는 문제, permission prompt loop, subagent hang, token usage 계산 crash 등이 수정되었습니다.

### IDE App

- 최신 저장 기준을 Antigravity IDE `2.1.1`로 올렸습니다.
- Settings의 Models tab에서 사용한 credit과 남은 credit을 더 명확히 보여주는 quota screen redesign이 적용되었습니다.
- agent security mode 변경이 저장되지 않던 권한 문제가 수정되었습니다.
- MCP server 안정성이 개선되었고, Chrome DevTools MCP server 사용 시 browser agent의 self-troubleshooting 능력이 좋아졌습니다.
- `mcp_config.json` schema가 `serverUrl`뿐 아니라 `url` 필드도 받습니다.
- strict mode에서 agent 접근 전 명시 확인이 필요한 sensitive path 목록에 `.vscode`와 `.cache`가 추가되었습니다.

### CLI App

- Antigravity 2.0 제품군 기준의 CLI baseline은 유지합니다.
- 공식 changelog에서 별도 새 CLI 패치 버전 번호는 확인되지 않았습니다.

## Sources

- [Claude Code CHANGELOG](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [Claude Code raw CHANGELOG](https://raw.githubusercontent.com/anthropics/claude-code/main/CHANGELOG.md)
- [npm @anthropic-ai/claude-code](https://www.npmjs.com/package/@anthropic-ai/claude-code)
- [OpenAI Codex changelog](https://developers.openai.com/codex/changelog)
- [npm @openai/codex](https://www.npmjs.com/package/@openai/codex)
- [Cursor changelog](https://cursor.com/ko/changelog)
- [Google Antigravity changelog](https://antigravity.google/changelog)
- [Google Antigravity releases](https://antigravity.google/releases)
