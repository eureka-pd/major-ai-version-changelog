# Antigravity

오늘 Antigravity는 Antigravity 2.0 `2.2.1`과 Antigravity IDE `2.1.1`이 새로 확인되었습니다. `.version`에 저장된 Antigravity `2.1.4`, IDE `2.0.4` 이후 새 보고 대상입니다.

## GUI App

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

## IDE App

- 최신 저장 기준을 Antigravity IDE `2.1.1`로 올렸습니다.
- Settings의 Models tab에서 사용한 credit과 남은 credit을 더 명확히 보여주는 quota screen redesign이 적용되었습니다.
- agent security mode 변경이 저장되지 않던 권한 문제가 수정되었습니다.
- MCP server 안정성이 개선되었고, Chrome DevTools MCP server 사용 시 browser agent의 self-troubleshooting 능력이 좋아졌습니다.
- `mcp_config.json` schema가 `serverUrl`뿐 아니라 `url` 필드도 받습니다.
- strict mode에서 agent 접근 전 명시 확인이 필요한 sensitive path 목록에 `.vscode`와 `.cache`가 추가되었습니다.

## CLI App

- Antigravity 2.0 제품군 기준의 CLI baseline은 유지합니다.
- 공식 changelog에서 별도 새 CLI 패치 버전 번호는 확인되지 않았습니다.

## Sources

- [Google Antigravity changelog](https://antigravity.google/changelog)
- [Google Antigravity releases](https://antigravity.google/releases)
