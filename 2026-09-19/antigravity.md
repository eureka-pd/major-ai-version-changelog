# Antigravity 변경사항

## GUI App

- 버전: `2.15.0` (이전: `2.14.0`, 2026-09-18)
- 커스텀 에이전트가 기본 프롬프트·기본 도구를 끄고 필요한 도구만 다시 켤 수 있고, 선택한 커스텀 에이전트가 reload 후에도 유지됩니다(삭제·비활성이면 메인으로 리셋).
- Page Up/Down·Home·End로 대화 스크롤, Escape로 프롬프트 박스에서 빠져나오며, 사이드바 대화 전환을 빠르게 하고 파일 드래그 하이라이트·채팅 bold 굵기를 다듬었습니다.
- 상태 파일 읽기 실패 시 설정·프로젝트 목록 덮어쓰기, permission 중복으로 대화 파일 비대화, 새 대화 가짜 crash recovery, 폴더 없는 대화가 다른 프로젝트 파일을 끌어오던 문제, 재시작으로 죽은 명령을 성공으로 보이던 문제, 바이너리 파일 읽기·malformed tool call·에러 드롭·시스템 메시지 중복, Escape/닫기 단축키·피드백 대용량 로그 실패 등을 고쳤습니다.

## IDE App

- 버전: `2.5.5`
- 이전 기록 이후 새 IDE 버전은 확인되지 않았습니다.

## CLI App

- 제품 탭: `2.0`, 바이너리: `1.2.6` (이전 바이너리: `1.2.0`)
- `1.2.1`–`1.2.6`을 반영했습니다. 세션 범위 Remote Control(`--remote-control`·`/remote-control`), headless 기본 타임아웃 무제한·`AGY_ERROR` stderr JSON, `/skills reload`, `/model` fuzzy 검색, Markdown 커스텀 에이전트 서브에이전트 로스터 주입, `excludeDefaultComponents`, 플러그인 MCP 자동 네임스페이스, `/copy btw`가 주요 추가입니다.
- Remote Control 권한 상속·아티팩트 카드, headless 오류 종료 코드, 무효 자격 정리, thinking 프레임 고정, mid-session Gemini thought_signature, `search_web` 요약 실패, 도구 스키마 자가 교정 등을 고쳤습니다.

## Sources

- [Google Antigravity changelog](https://antigravity.google/changelog)
