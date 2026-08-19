# Claude Code 변경사항

## GUI App

- 버전: `2.1.235` (이전: `2.1.234`)
- 입력창에서 맞춤법 검사(`spellcheck`)를 켤 수 있으며, 설치된 `aspell`·`hunspell`·`ispell`을 사용합니다.
- 권한 대화상자의 안내와 "다시 묻지 않기" 항목이 실제 허용 범위와 맞게 표시되고, 내용을 다 보여 주지 못하면 해당 옵션을 숨깁니다.
- 클라우드 세션 백그라운드 메모리·CPU 사용을 줄이고, VS Code에서 창을 복원할 때 Claude 탭 포커스가 혼자 바뀌던 문제를 고쳤습니다.

## CLI App

- 버전: `2.1.235` (이전: `2.1.234`)
- 중첩 마크다운 목록 정렬, 여러 줄 프롬프트의 하이라이트 어긋남, Shift+Tab이 권한 댓글 칸에서 편집을 승인하던 문제를 수정했습니다.
- 내장 `grep`이 위험한 패턴에서 메모리를 소진하지 않고 빨리 실패하며, `-m N`과 `-A`/`-C` 컨텍스트가 맞게 출력됩니다.
- `SendMessage`는 세션 간 전달 한도를 넘는 메시지를 미리 거절하고, `claude rc`는 대화형 시작과 같은 엔터프라이즈 게이트웨이 가용성 검사를 적용합니다. 공식 로그는 GUI와 CLI의 별도 빌드가 아닌 공통 릴리스로 게시합니다.

## Sources

- [Claude Code changelog](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
