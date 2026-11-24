# Antigravity
- 기준일: 2026-11-25 (Asia/Seoul)
- **앱 2.34.0 → 2.35.0**. 공식 변경 로그의 11월 23일자 항목이다. 앱도 로컬 대화를 500개로 제한하지 않는다. 에이전트와 스크립트가 대화를 검색·정리할 수 있는 관리 API가 생겼고 전체 화면 HTML 산출물에 Ctrl/Cmd+F 검색이 추가됐다.
- **CLI 바이너리 1.5.15 → 1.5.16**. 공식 GitHub의 11월 24일자 릴리스다. `agy --resume <ID>` 또는 `agy -r <ID>`로 특정 대화를 다시 열 수 있다. `~/.agents/skills`의 공용 스킬도 인식하며 이름이 겹치면 `~/.gemini` 쪽이 우선한다.
- CLI에서 에이전트 질문에 직접 답을 쓸 때 한글 등 IME 조합 위치가 어긋나던 문제와 macOS SSH에서 잠금 해제된 로그인 키체인을 재사용하지 못하던 문제를 수정했다.
- **권한 변경:** CLI Auto 모드는 작업 공간 밖이라도 버전 관리 저장소 내의 파일이거나 기존 내용을 교체하지 않고 추가만 하는 변경이라면 확인 없이 허용할 수 있다. 외부 파일을 건드리면 안 되는 작업에서는 기본 Auto 모드를 그 경계로 간주하지 않는 편이 좋다.
- 별도 **Antigravity IDE 2.8.0**은 유지.

## 출처
- [Google · Antigravity 공식 변경 로그](https://antigravity.google/docs/changelog)
- [Google · Antigravity CLI 1.5.16 릴리스](https://github.com/google-antigravity/antigravity-cli/releases/tag/1.5.16)
