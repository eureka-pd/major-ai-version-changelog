# SUMMARY

2026-08-08 확인 결과, Claude Code `2.1.224`, Codex CLI `0.147.0`, Antigravity CLI Binary `1.1.11`이 새로 기록되었습니다. Cursor에는 새 버전이나 공지가 없습니다.

## Claude Code

### GUI App

- 버전: `2.1.224`
- Team·Enterprise 플랜은 자체 PC나 컨테이너를 웹·모바일·데스크톱 세션의 실행 환경으로 등록할 수 있습니다.
- macOS와 Linux에서 서로 다른 Claude Code 세션끼리 메시지를 주고받을 수 있습니다.
- 원격 제어 화면에서 압축 진행 상황과 연결 실패 원인을 더 명확하게 보여 줍니다.

### CLI App

- 버전: `2.1.224`
- HTTPS의 ZIP 파일에서 플러그인을 설치할 수 있으며, SHA-256 값으로 파일이 바뀌지 않았는지 확인할 수 있습니다.
- Bedrock 사용 시 선호할 리전을 지정하는 환경 변수를 추가했습니다.
- 긴 경로에서 다른 프로젝트의 세션을 잘못 여는 문제와, 전송 실패를 성공으로 표시하던 문제를 수정했습니다.
- 샌드박스의 파일·네트워크 거부 이유를 명령 결과에서 확인할 수 있도록 했습니다.

## Codex

### GUI App

- 버전: `26.727`
- 이전 기록 이후 새 GUI 앱 버전은 확인되지 않았습니다.

### CLI App

- 버전: `0.147.0`
- 플러그인을 설치하고 로컬·개인·워크스페이스·원격 카탈로그에서 검색할 수 있습니다.
- 대화를 직접 정렬하는 섹션으로 묶고, 긴 기록은 필요한 부분부터 나누어 볼 수 있습니다.
- `--approve-for-me` 옵션으로 자동 검토를 거친 승인 흐름을 사용할 수 있습니다.
- Cursor 스킬을 가져오고, 가져온 Claude·Cursor 대화의 변경사항을 중복 없이 동기화합니다.
- 새 MCP 프로토콜을 선택적으로 지원하며, MCP 서버 시작 전에도 도구 탐색을 이어갈 수 있습니다.
- 화면·대화 기록의 비밀값 마스킹, 터미널 입력 멈춤, Windows 프로세스 종료 처리와 플러그인 격리를 보완했습니다.

### General

- 이전 기록 이후 새 일반 공지는 확인되지 않았습니다.

### Mobile

- 버전: `1.2026.202`
- 이전 기록 이후 새 모바일 앱 버전은 확인되지 않았습니다.

## Cursor

### GUI App

- 버전: `3.11`
- 이전 기록 이후 새 GUI 앱 버전은 확인되지 않았습니다.

### CLI App

- 현재 공개 변경 로그에서 새 CLI 버전은 확인되지 않았습니다.

## Antigravity

### GUI App

- 버전: `2.5.0`
- 이전 기록 이후 새 GUI 앱 버전은 확인되지 않았습니다.

### IDE App

- 버전: `2.1.1`
- 이전 기록 이후 새 IDE 버전은 확인되지 않았습니다.

### CLI App

- 버전: `2.0` (CLI), `1.1.11` (CLI Binary)
- 선택형 Vim 편집 모드를 추가했습니다. 입력창, 댓글, diff에서 Vim 이동과 편집을 사용할 수 있습니다.
- `-p` 모드에서 `/usage`, `/quota`, `/credits`, `/model`, `/effort`, `/skills` 같은 읽기 전용 명령은 에이전트를 실행하지 않고 결과만 출력합니다.
- 플러그인의 켜짐·꺼짐 상태를 사용자 설정에만 저장해, 플러그인 업데이트가 기존 선택을 임의로 바꾸지 않게 했습니다.
- 빈 명령 허용 규칙이 모든 명령을 자동 승인할 수 있던 문제, 엄격 권한 모드의 자동 승인 문제, MCP 관리자 제어 누락 문제를 수정했습니다.

## Sources

- [Claude Code changelog](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [OpenAI Codex changelog](https://developers.openai.com/codex/changelog)
- [Cursor changelog](https://cursor.com/ko/changelog)
- [Google Antigravity changelog](https://antigravity.google/changelog)
