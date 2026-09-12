# Claude Code 변경사항

## GUI App

- 버전: `2.1.269` (이전: `2.1.268`)
- `claude plugin eval`로 플러그인 eval 스위트를 실행해 JSON·HTML 점수 리포트를 받을 수 있습니다(`claude plugin eval --help`).
- `/output-style [name]`으로 출력 스타일을 목록·전환합니다. Remote Control·클라우드·기타 헤드리스 세션에서도 동작합니다.
- Bash 도구가 파일 편집을 처리할 때(`bashEditDiffEnabled`) 변경된 파일 diff를 Bash 결과에 붙입니다.
- `OTEL_METRICS_INCLUDE_REPOSITORY`로 OpenTelemetry 메트릭·이벤트에 `vcs.*` 저장소 태그를 넣고, 커밋 이벤트는 `OTEL_LOG_TOOL_DETAILS`와 함께 `vcs.ref.head.*`를 붙입니다.
- `CLAUDE_CODE_GATEWAY_MODEL_DISCOVERY_TIMEOUT_MS`로 LLM gateway `/v1/models` 발견 타임아웃을 늘릴 수 있습니다(기본 3초).
- 스피너 tip이 `/focus`를 안내합니다. 프롬프트·한 줄 작업 요약·응답만 보이는 화면입니다.
- `CLAUDE_CODE_WORKFLOW_MAX_CONCURRENT_AGENTS`(1–256)로 Workflow 도구 실행당 동시 에이전트 한도를 올릴 수 있습니다.
- 출력 토큰 한도로 잘린 뒤 자동 재개한 다음 턴의 프롬프트 캐시 부분 무효화, 생각 중 중단 후 resume이 이전 컨텍스트 재전송 방식을 바꿔 캐시 재사용이 나빠지던 문제를 고쳤습니다.
- kitty 프로토콜 터미널의 F1/F2/F4, st의 Delete, rxvt-unicode의 Alt+화살표가 Escape로 동작, WezTerm에서 Shift+문장부호가 비Shift로 입력되던 회귀(2.1.247)를 고쳤습니다.
- 원격·헤드리스가 백그라운드 에이전트 실행 중에도 “입력 대기”로 보이던 문제(`CLAUDE_CODE_BG_TASKS_REPORT_RUNNING=0`이면 이전 동작), 터미널 capability 응답이 기동 시 프롬프트에 섞이던 문제를 고쳤습니다.
- 전체화면에서 터미널 리사이즈 후 트랜스크립트 상·하단 줄이 비던 문제, `!`로 시작하는 deny/ask 규칙이 기록한 설정 소스 밖으로 적용되던 문제(단독 `!`는 무시), compaction 후 git status가 세션 시작 값으로 남던 문제를 고쳤습니다.
- 원격 resume 시 동기화 플러그인 MCP 미연결, 헤드리스 resume에서 모델 전환·재시도 중 턴 응답 유실, 백그라운드 태스크 on-disk 기록의 escape·줄바꿈·과장 텍스트가 태스크 목록·알림에 새던 문제를 고쳤습니다.
- CMYK JPEG 첨부 실패, gRPC 텔레메트리 엔드포인트(스킴 없음) 승인 다이얼로그의 collector 이름 누락, 플러그인 `headersHelper` 동의 URL 경로가 다른 호스트로 보이던 문제, Windows에서 `@`로 시작하는 폴더가 `[redacted URL]`로 보이던 문제를 고쳤습니다.
- 네이티브 커서 모드에서 permission-rule·auto-mode-rule·add-directory·session-rename·feedback-review 입력란 커서 누락, `/fork` 영수증을 1초 미만 간격으로 반복 클릭해도 도구 종료 전 바로 백그라운드되지 않던 문제를 고쳤습니다.
- `shutdown`을 거절하는 플러그인 LSP(예: rust-analyzer)에 `exit` 전송, CLAUDE.md·memory의 커밋/PR attribution 금지 규칙을 알림이 덮던 문제(managed settings 줄은 유지), 단어 사이 공백 없는 언어의 prompt suggestion 누락을 고쳤습니다.
- GNOME Terminal·Konsole이 동기화 출력을 지원하지 않는데도 이름만으로 가정하던 문제, path-scoped deny의 Read/Edit/Write가 `permission_denials`(stream-json)에서 빠지던 문제, SDK·데스크톱 세션이 다른 세션 에이전트 목록에서 unknown이던 문제를 고쳤습니다.
- Bedrock·Vertex·Foundry·gateway에서 `/insights`가 기본 Opus에 닿지 못해 실패하던 문제(세션 모델 사용), 다른 프로세스가 동시에 로그인을 갱신해 org policy 한도가 안 불러지던 문제, Desktop의 Bedrock/Vertex/gateway에 turn-end “무엇을 필요한지” 안내가 없던 문제를 고쳤습니다.
- MCP URL 쿼리 순서만 바뀐 재연결, 백그라운드 에이전트 이름·설명 줄바꿈·폭 초과로 프롬프트 상단 테두리가 쪼개지던 문제, auto-compaction할 이전 교환이 없을 때 “Prompt is too long”에 영구 고착되던 문제(주로 큰 프롬프트 Agent SDK)를 고쳤습니다.
- `/goal`이 API·네트워크·토큰 한도 후 조용히 멈추던 문제(백오프 재시도 또는 사유와 함께 일시정지), 클라우드 세션이 첫 요청 전 서버 설정을 잠시 기다려 프롬프트 캐시 미스를 줄이도록 했습니다.
- `/btw`가 가짜 도구 호출·출력을 쓰던 문제(작성 금지·표시), `CLAUDE_CODE_RESUME_INTERRUPTED_TURN`이 6시간(또는 `CLAUDE_CODE_RESUME_INTERRUPTED_TURN_MAX_AGE_MS`) 지난 API 오류 턴을 다시 돌리던 문제를 고쳤습니다.
- managed settings로 켠 조직 플러그인이 헤드리스·Claude Desktop에서 안 불러지던 문제(다음 세션부터), 플러그인 아카이브가 다른 로컬 사용자에게 읽히거나 world-writable·잔존 파일로 남던 문제를 고쳤습니다.
- Bash `tee` 대상에 `Edit()` deny·쓰기 경로 검사가 적용되지 않던 문제(`Bash(tee:*)` allow가 작업 디렉터리 밖을 덮지 않음), ssh·브라우저 터미널 기동의 `22c` 등 stray 문자, rxvt-unicode 전체화면 블록 커서·외부 에디터 복귀 커서, 전체화면 밖 Ctrl+G·Konsole 외부 에디터 복귀 이중 그리기를 고쳤습니다.
- Windows: 백그라운드로 보낸 PowerShell 도구가 Claude Code 종료와 함께 멈추던 문제를 고쳤습니다.
- `/diff` 패널이 로딩 없이 바로 렌더되고, 일본어·중국어·한국어 prompt suggestion 필터(혼용·단일어 유지, 평가성 문구 제거), Skill “Unknown skill”에 플러그인 전체 이름, kitty keyboard 질의에 답하는 터미널(foot·Alacritty 0.16+ 등)의 Shift+Enter·Ctrl+Shift, 긴 세션 transcript 갱신 성능, telemetry off 세션에서 `alwaysLoad` MCP 즉시 사용을 개선했습니다.
- `/ultrareview --post`가 두 번째 클라우드 세션 없이 바로 PR 댓글을 달고 링크를 출력합니다. 아티팩트 DB 읽기→scratchpad 저장은 working-folder 승인을 막지 않습니다.
- 클라우드에서 claude.ai 동기화 스킬 이름이 Desktop과 같이 `anthropic-skills:<name>`입니다(충돌 없으면 짧은 이름도 유효).
- [VSCode] 에이전트 맵(푸터 “N agents”·카드·Stop·읽기 전용 transcript), 명령 메뉴 Hooks 다이얼로그, Focus의 서브에이전트 live progress, Permission rules 다이얼로그, Switch account Cancel을 추가했습니다.
- [VSCode] 예약 작업 등 plain-text로 시작된 턴이 이전 턴에 붙던 문제, 좁은 패널에서 프롬프트 캐시 시계 분 숨김, `CLAUDE_CONFIG_DIR` 설정 시 세션 목록이 기본 폴더를 유지하던 문제, 늦은 plan preview 댓글 상자·닫힌 탭 댓글, compaction 후 재오픈 cold 표시, Remote Control 중 이름 미동기화, Remote Control 전체 토글 잔존, reload 후 탭 open 미집계·이중 탭, Switch account 후 usage 경고 재노출, 긴 턴 중 rename이 생성 이름으로 덮이던 문제, 사라진 weekly limit 행 잔존, 새 채팅 시작 중 @-mention 지연 삽입, Account & usage 헤더로 목록이 내려가던 문제를 고쳤습니다.
- [VSCode] 사용자 외 청중용 문서·메시지 작성, 슬래시·@·output-style·Send/Stop·권한·질문·온보딩 접근성을 개선했고, 현재 파일 chip은 X로 제거합니다. 탭 우클릭·에디터 “...”의 Claude Code 항목은 해당 탭에 동작하지 않아 제거했습니다.
- [웹] 클라우드 큐 메시지를 Claude가 읽기 전 회수(큐에서 제거 또는 Esc/Up), `/model default`가 org 모델 제한에서 이후 메시지 전부 실패하던 문제, 일회 루틴 중복 실행, 서브에이전트 루틴 조기 완료, repo 하위 폴더 작업의 GitHub 404 링크, Cloud environments 5행 제한, Free 플랜의 “Disabled by org admin” 대신 업그레이드 경로를 고치거나 바꿨습니다.
- [Claude Tag] GitHub Connect all/Disconnect 확인, Slack rate-limit으로 실패 알림이 떨어져 스레드가 조용해지던 문제(재시도), 미허용 모델 전환 후 조용한 폴백 대신 거절, 파일 첨부 시 표가 raw pipe로 가던 문제, 비활성 채널 `@Claude !restart`, 플러그인 행 unlabeled ID, Slack 시작 세션 공유 배너의 org 전체 오안내, 관리 설정·채널 picker 로딩, 루틴의 기존 스레드 답글, progress checklist의 로컬 시각·경과를 고치거나 개선했습니다.

## CLI App

- 버전: `2.1.269` (이전: `2.1.268`)
- GUI와 동일 릴리스입니다. plugin eval·`/output-style`·Bash edit diff·OTEL 저장소 태그·gateway 모델 발견 타임아웃·Workflow 동시성, 프롬프트 캐시·터미널·권한·MCP·`/goal`·플러그인 보안, VS Code·웹·Claude Tag 수정을 포함합니다.

## Sources

- [Claude Code changelog](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
