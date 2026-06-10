# Codex

- 확인 결과: Codex 쪽에는 새로 보고할 항목이 있습니다.
- 이전 저장 기준: Codex app `26.602`, Codex CLI `0.138.0`
- 최신 확인 기준: Codex app `26.602`, Codex CLI `0.139.0`, ChatGPT for iOS `1.2026.153`
- 중복 보고 방지 상태: CLI component를 `0.139.0`, mobile component를 `1.2026.153`으로 저장했습니다.
- 출처: [OpenAI Codex changelog](https://developers.openai.com/codex/changelog), [Codex CLI 0.139.0 release](https://github.com/openai/codex/releases/tag/rust-v0.139.0), [npm @openai/codex](https://www.npmjs.com/package/@openai/codex)

## GUI App

- Codex app 최신 기준은 계속 `26.602` (2026-06-04)입니다.
- 데스크톱 GUI 앱 자체의 새 버전 번호는 공식 changelog 상단에서 확인되지 않았습니다.
- 대신 2026-06-09에 ChatGPT for iOS의 Codex 기능이 `1.2026.153`으로 올라갔습니다.
- iOS 새 thread에서 branch 선택, worktree 생성, 환경 setup script 실행을 할 수 있습니다.
- Codex profile 화면에 사용량 통계와 token 활동 차트가 추가되었습니다.
- 첨부 지원, side chat/queued prompt 표시, 메시지 스타일, navigation, tool activity, Face ID, archived thread 탐색 같은 사용성도 다듬어졌습니다.

## CLI App

### `0.139.0` (2026-06-09)

- code mode에서 standalone web search를 직접 호출할 수 있게 되었습니다. 중첩된 JavaScript tool call에서도 plaintext 검색 결과를 받을 수 있어, 코드 작업 중 외부 확인 흐름이 더 자연스러워졌습니다.
- tool/connector schema 처리에서 `oneOf`, `allOf` 보존이 좋아졌고, 큰 schema도 얕은 구조를 더 많이 유지합니다. 복잡한 MCP tool 호환성이 좋아지는 변화입니다.
- `codex doctor`가 editor와 pager 환경 정보를 로컬 진단에 포함합니다. JSON 출력에서는 raw 값이 redaction됩니다.
- plugin marketplace 목록 JSON에 marketplace source가 포함되고, 원격 catalog refresh 전에도 cache 결과를 먼저 돌려줄 수 있습니다.
- `codex resume --last "..."`와 `codex fork --last "..."`가 뒤쪽 문자열을 session ID로 오해하지 않고 initial prompt로 처리합니다.
- image edit은 대화 기록 추측 대신 실제 참조된 이미지 파일 경로를 사용합니다. 첨부 이미지 편집이 엉뚱한 파일에 적용될 위험이 줄었습니다.
- `/new`, `/clear`, `/fork` 같은 thread reset 중 cloud-managed requirements와 feature flags가 사라지지 않도록 수정되었습니다.
- sandbox 실행은 승인된 escalation 결정과 proxy-only networking 설정을 더 일관되게 보존합니다.
