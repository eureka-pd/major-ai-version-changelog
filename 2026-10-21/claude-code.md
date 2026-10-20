# Claude Code

- 기준일: 2026-10-21 (Asia/Seoul)
- 확인 시각: 2026-10-21 04:18 KST
- 비교 기준: 직전 `.version` 및 2026-10-20 기록

## 신규 버전: 2.1.304

- 자동 모드가 프로젝트와 최근 세션을 참고해 환경에 맞게 설정하도록 돕는 `/auto-mode-setup`이 추가됐다. Bedrock·Vertex·Foundry 등의 환경도 지원한다.
- 오래 쉬었던 대화를 재개할 때 5시간 사용량 한도를 많이 쓸 수 있으면 Pro·Max 사용자에게 미리 경고한다.
- worktree 종료 시 브랜치와 커밋이 확인 없이 삭제될 수 있던 문제, 마운트된 드라이브 삭제 시 안전 확인이 빠지던 문제를 수정했다.
- 대화 압축 중 중단 뒤 발생하던 길이 초과 오류와 하위 에이전트의 최근 작업 누락을 수정하고, 긴 대화 재개·다수 에이전트 동시 실행 성능을 개선했다.
- Code Review에 Quick·Standard·Deep 검토 수준과 조직의 모든 저장소를 자동으로 검토 대상으로 포함하는 옵션이 추가됐다.

공식 릴리스 게시 시각은 **2026-10-19 21:34:39 UTC / 2026-10-20 06:34:39 KST**다. 이번 확인에서 처음 기록한 버전이며, 10월 21일에 출시됐다는 뜻은 아니다. CLI와 공개 CHANGELOG 최신 값만 갱신하고 별도 GUI 값은 유지한다.

## Sources

- [공식 CHANGELOG](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [공식 2.1.304 릴리스](https://github.com/anthropics/claude-code/releases/tag/v2.1.304)
