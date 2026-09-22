# Claude Code 변경사항

## GUI App

- 버전: `2.1.280` (이전: `2.1.278`)
- Claude Opus 5.5(`claude-opus-5-5`)를 추가했고, 기본 Opus 모델로 씁니다. 컨텍스트 1M, 입력/출력 $4/$20 per Mtok, 캐시 읽기 $0.20/Mtok입니다.
- Pro·Team Standard 기본 모델을 Sonnet에서 Opus로 바꿨습니다(Max·Team Premium·Enterprise와 동일).
- 전체 화면 목록 마우스 지원, MCP 설명 길이 환경변수, 심링크 Write 판정·auto mode 재시도/백오프, Write 인자 별칭, 다이얼로그 Ctrl+C/키바인딩·Windows 프롬프트 정리, 음성 받아쓰기, 프롬프트 캐시·서브에이전트·플러그인·VSCode·클라우드·Claude Tag·Code Review 등 다수 수정·개선이 포함됩니다.

## CLI App

- 버전: `2.1.280` (이전: `2.1.278`)
- GUI와 동일 릴리스입니다. Opus 5.5 기본화와 위 수정·개선이 포함됩니다.

## Sources

- [Claude Code changelog](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
