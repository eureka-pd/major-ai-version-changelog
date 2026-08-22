# Claude Code 변경사항

## GUI App

- 버전: `2.1.240` (이전: `2.1.238`)
- `2.1.240`은 버그 수정과 안정성 개선입니다. `2.1.239`에서 비용 추정(`/cost`, 상태줄, `--max-budget-usd`)에 데이터 레지던시 워크스페이스의 미국 전용 추론 1.1× 프리미엄이 포함됩니다.
- Bedrock·Vertex·Foundry 등 이전 제외 환경에도 전체화면 렌더러를 한 번 제안하며, 그곳의 새 설치는 전체화면으로 시작합니다.
- 월 한도가 이미 소진됐을 때 세션·주간 한도 리셋 시각도 안내하고, Windows에서 교차 세션 메시징(`SendMessage`/`ListAgents`)이 됩니다.
- 클라우드 세션의 claude.ai 동기화 플러그인은 `name@synced`로 표시되며 같은 이름 로컬 플러그인을 덮어쓰지 않습니다. VS Code 사용량 배너의 "View usage"는 경고 문구 옆에 붙습니다.

## CLI App

- 버전: `2.1.240` (이전: `2.1.238`)
- `/claude-api upgrade`로 Python 프로젝트의 `anthropic` 0.x → 1.x 마이그레이션을 지원합니다(타임아웃은 `anthropic.Timeout`).
- Alpine/musl 빌드에서 이미지 붙여넣기·클립보드·오디오 캡처 네이티브 애드온이 로드됩니다.
- 프록시가 Content-Type을 떼면 Bedrock 스트리밍이 비스트리밍으로 재실행되며 과금이 두 배가 되던 문제를 고쳤고, Bedrock SSO+`awsAuthRefresh` 시작이 `HTTPS_PROXY`를 존중합니다.
- WebFetch가 만료 페이지를 세션 내내 붙들던 문제, `/goal` 점검 주기(30분→1시간→2시간), `ListAgents`의 실제 팀원 표시, readline 단어 이동·삭제를 포함합니다. 공식 로그는 GUI와 CLI의 별도 빌드가 아닌 공통 릴리스로 게시합니다.

## Sources

- [Claude Code changelog](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
