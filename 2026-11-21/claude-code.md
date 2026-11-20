# Claude Code
- 기준일: 2026-11-21 (Asia/Seoul)
- CLI: **2.1.328 → 2.1.329** (공식 GitHub 릴리스). GUI는 신규 버전 미확인.

## 달라진 점
- `/tasks`에서 현재 세션의 예약 작업, `/loop`, 목표, 대화 분기를 볼 수 있고 확인을 거쳐 중지할 수 있다.
- 폴더 신뢰 확인 창이 훅의 설정 위치를 표시한다. 원격 HTTP MCP가 연결을 거부하면 `/mcp`에서 서버 오류 메시지를 볼 수 있다.
- macOS 키체인 저장 실패 때 다른 세션까지 로그아웃되거나 파일 잠금·읽기 지연으로 설정이 초기화되던 문제를 수정했다. `/teleport`에서 고른 클라우드 대화는 기존 대화를 덮어쓰지 않고 새 세션에서 열린다.

## 출처
- [Anthropic · v2.1.329 공식 릴리스](https://github.com/anthropics/claude-code/releases/tag/v2.1.329)
- [Anthropic · CHANGELOG](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
