# Claude Code 변경사항

## GUI App

- 버전: `2.1.227` (이전: `2.1.226`)
- 만료된 로그인 토큰으로 시작한 세션이 요금제 정보를 잘못 판단해 불필요한 사용량 크레딧 안내를 띄우던 문제를 수정했습니다.
- 처음 메시지 이전으로 되감은 대화를 `/tui`가 다시 불러오던 문제를 수정했습니다.
- 슬래시 명령 메뉴에서 선택 항목과 검색 일치 항목을 더 명확히 표시하고, 특수 문자 이름도 정상적으로 보이게 했습니다.
- 파일을 찾지 못했을 때의 추천과 `@` 멘션 크기 확인 중 발생하던 화면 멈춤을 줄였습니다.

## CLI App

- 버전: `2.1.227` (이전: `2.1.226`)
- GitHub-hosted runner에서 `claude-code-action`의 `allowed_non_write_users` 설정을 쓸 때 모든 Bash 명령이 실패하던 문제를 수정했습니다.
- 위 로그인·대화 복원·명령 메뉴·성능 개선은 Claude Code 공통 변경사항입니다.

## Sources

- [Claude Code changelog](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
