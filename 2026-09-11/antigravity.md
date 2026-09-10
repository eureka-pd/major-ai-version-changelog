# Antigravity 변경사항

## GUI App

- 버전: `2.12.2`
- 이전 기록 이후 새 GUI 버전은 확인되지 않았습니다. 최신은 2026-09-03 엔터프라이즈 ADC Gemini 3.8 Flash입니다.

## IDE App

- 버전: `2.5.5`
- 이전 기록 이후 새 IDE 버전은 확인되지 않았습니다.

## CLI App

- 제품 탭: `2.0`, 바이너리: `1.2.0` (이전: `1.1.25`, 2026-09-10 공개)
- `1.2.0`: `remote-control start|status|stop`으로 OS 서비스 매니저에 CLI를 백그라운드 데몬으로 등록하고, half-page 스크롤·`Shift+Up/Down` 키바인딩을 넓혔습니다. 콘텐츠 필터 중단 사유 표시, scratch 감시, 플러그인 MCP 초기화, MCP schema `additionalProperties`, 중복 discovery walk, `unknown step type` resume 실패를 고쳤습니다.
- `1.1.28`(2026-09-09): 모델 API 503 등 재시도 백오프, 캐시 자격으로 기동·로그인 가속, `-p` 종료·stderr 오류·지연 축소, 도구 승인 프롬프트의 구체 동작·Reason, URL fetch 기본 승인 요구를 넣었습니다. 플러그인 재설치 잔여 파일, 플러그인 MCP cwd, 서브에이전트 MCP 레이스·Running 고착, 명령 메모리 누수, `-p` plan 승인 멈춤, 계정 전환 후 프로젝트 캐시를 고쳤습니다.
- `1.1.27`(2026-09-05): 한 번만 다른 모델을 쓰는 `/model`, status line용 `conversation_title`, 커스텀 에이전트 frontmatter `agents` 의존을 넣었고, MCP 미선언 인자 거부, `-p` denied_actions, Vim `?` 검색, print 종료 히스토리 유실을 고쳤습니다.
- `1.1.26`(2026-09-04): 아티팩트 뷰어 half-page 스크롤, `/resume`용 `pickerGrouping`, Mermaid ASCII, 미선택 모델 기본 effort medium, worktree 정리·SQLite WAL flush·서브에이전트 승인 프롬프트를 고쳤습니다.

## Sources

- [Google Antigravity changelog](https://antigravity.google/changelog)
