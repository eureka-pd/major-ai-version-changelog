# Claude Code 변경사항

2026-08-08 확인 결과, Claude Code `2.1.224`이 새로 기록되었습니다.

## GUI App

- 버전: `2.1.224`
- Team·Enterprise 플랜은 자체 PC나 컨테이너를 웹·모바일·데스크톱 세션의 실행 환경으로 등록할 수 있습니다.
- macOS와 Linux에서 서로 다른 Claude Code 세션끼리 메시지를 주고받을 수 있습니다.
- 원격 제어 화면에서 압축 진행 상황과 연결 실패 원인을 더 명확하게 보여 줍니다.

## CLI App

- 버전: `2.1.224`
- HTTPS의 ZIP 파일에서 플러그인을 설치할 수 있으며, SHA-256 값으로 파일이 바뀌지 않았는지 확인할 수 있습니다.
- Bedrock 사용 시 선호할 리전을 지정하는 환경 변수를 추가했습니다.
- 긴 경로에서 다른 프로젝트의 세션을 잘못 여는 문제와, 전송 실패를 성공으로 표시하던 문제를 수정했습니다.
- 샌드박스의 파일·네트워크 거부 이유를 명령 결과에서 확인할 수 있도록 했습니다.

## Sources

- [Claude Code changelog](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
