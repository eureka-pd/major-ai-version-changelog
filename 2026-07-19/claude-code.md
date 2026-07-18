# Claude Code

## GUI App

- 최신 저장 기준을 `2.1.212`에서 `2.1.214`로 올렸습니다.
- 오래 걸리는 도구 호출에 주기적인 진행 신호를 추가해 멈춘 것처럼 보이는 상황을 줄였습니다.
- background session을 다시 열거나 삭제할 때 생기던 오류와 daemon 교체 과정의 소켓 충돌을 고쳤습니다.
- 설정 파일, memory frontmatter, feature flag 캐시가 잘못되거나 지나치게 커졌을 때 더 안전하게 처리합니다.

## CLI App

- npm `latest`와 `next`는 모두 `2.1.214`입니다. 공개 changelog에는 별도의 `2.1.213` 항목 없이 `2.1.214`가 이어집니다.
- `Edit(src/**)` 같은 허용 규칙이 현재 저장소 밖의 같은 이름 폴더까지 잘못 승인하던 문제를 고쳤습니다.
- Windows PowerShell 권한 우회, Bash 파일 디스크립터 리다이렉션, 매우 긴 명령, zsh 조건식 등 권한 판정의 빈틈을 보강했습니다.
- Docker·Podman 원격 daemon 옵션은 자동 실행하지 않고 권한을 묻도록 바뀌었습니다.
- Windows의 프록시 연결, PowerShell 표준 입력·문자 인코딩·리다이렉션 문제를 다수 수정했습니다.
- plugin, MCP 새로고침, OpenTelemetry 추적과 background 작업 종료 안정성을 개선했습니다.

## Sources

- [Claude Code CHANGELOG](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [Claude Code raw CHANGELOG](https://raw.githubusercontent.com/anthropics/claude-code/main/CHANGELOG.md)
- [npm @anthropic-ai/claude-code](https://www.npmjs.com/package/@anthropic-ai/claude-code)
