# Claude Code 변경사항

## GUI App

- 버전: `2.1.266` (이전: `2.1.263`)
- `2.1.265`에서 `CLAUDE_CODE_USE_GATEWAY`만 있으면 Cloud gateway 로그인을 강제하던 회귀를 `2.1.266`에서 되돌렸습니다. 변수만 두고 API 키·`apiKeyHelper`·커스텀 헤더를 쓰는 구성은 다시 그대로 동작합니다.
- 플러그인 폴더 전체를 `--plugin-dir`로 가리키면 자식 폴더의 매니페스트를 각각 읽고, 실행 중 추가·삭제도 반영합니다.
- 디스크에 저장하는 도구 결과 상한을 1GB로 두고, 잘린 미리보기는 대화에 표시합니다.
- 텔레메트리에 `user.email`·`user.groups`를 넣고, Claude apps gateway 세션은 관리 설정이 지정한 OTLP 수집기로 직접 보내게 바꿨습니다.
- 포그라운드 서브에이전트 재개 시 도구·시스템 프롬프트가 바뀌어 프롬프트 캐시가 깨지던 문제, 프로세스 사망 후 재개 시 마지막 프롬프트 재작성·중단된 도구 처리, `/model opusplan[1m]` 거부를 고쳤습니다.
- Remote Control이 답 끝나기 전에 종료 신호를 내거나, `--bg` 세션이 유휴 타임아웃 직전에 종료되던 문제를 고쳤습니다.
- HTTP MCP가 legacy SSE만 말할 때 연결되지 않던 문제, 비대화형 세션에서 매 메시지마다 cwd가 리셋되던 문제, Windows AppContainer에서 Read/Write/Edit가 전부 거절되던 문제를 고쳤습니다.
- [VSCode] 비활성 세션 자동 아카이브(기본 14일), Reload Window 후 10분 이상 연 채팅이 비던 문제, Remote Control 활성 문구의 타임라인 점 정렬을 고쳤습니다.

## CLI App

- 버전: `2.1.266` (이전: `2.1.263`)
- GUI와 동일 릴리스입니다. gateway 로그인 회귀 수정, 플러그인 디렉터리 로드, 도구 결과 상한, 서브에이전트·Remote Control·MCP·Windows 샌드박스 수정을 포함합니다.

## Sources

- [Claude Code changelog](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
