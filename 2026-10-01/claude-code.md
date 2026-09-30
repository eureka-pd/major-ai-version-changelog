# Claude Code 변경사항

## GUI App

- 버전: `2.1.286` (이전: `2.1.284`)
- **2.1.286**: 권한 요청이 쌓일 때 "2 of 5"처럼 순번을 보여 주고, 전체화면 목록의 "N more" 행을 마우스로 클릭·호버할 수 있습니다. 병렬 도구 호출 후 `--resume`/`--continue`가 턴을 잃던 문제, API 400(비텍스트 tool/hook 결과), 클라우드 세션 대용량 히스토리 기동, gateway spend meter 요금·입력 토큰 집계, macOS 로그인 상태, Remote Control 정책 해제 시 연결 유지, MCP/시크릿 마스킹, 서브에이전트·워크플로, `/compact`/`/clear`/`/rewind`가 백그라운드 에이전트 트랜스크립트에 잘못 적용되던 점 등을 고쳤습니다. VS Code에는 북마크 사이드 패널, 질문 카드에 답변·옵션 미리보기, 메시지에 붙은 터미널/브라우저/선택 코드 행이 추가됐고 Stop/Esc는 현재 턴만 끝냅니다. (중간에 **2.1.285**: `CLAUDE_CODE_DISABLE_WEB_FETCH`, `claude --desktop`, `claude plugin configure`, `allowedProviders` 관리 설정 등.)

## CLI App

- 버전: `2.1.286`
- GUI와 동일합니다.

## Sources

- [Claude Code changelog](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
