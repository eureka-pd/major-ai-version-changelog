# Claude Code

- 기준일: 2026-10-23 (Asia/Seoul)
- 확인 시각: 2026-10-23 04:16 KST
- 비교 기준: 직전 `.version` 및 2026-10-22 기록

## 새로 확인한 버전

- **2.1.307**: 2026-10-21 22:17 UTC / 10월 22일 07:17 KST 게시.
- **2.1.308**: 2026-10-22 04:34 UTC / 10월 22일 13:34 KST 게시.
- 현재 공식 CHANGELOG와 정식 릴리스가 모두 2.1.308을 가리킨다. GUI의 기존 별도 버전 필드는 근거 없이 변경하지 않았다.

## 핵심 변경

- 2.1.307은 연결이 끊긴 HTTP MCP 호출을 중복 실행하던 문제를 수정했다. 자동 재시도는 읽기 전용 또는 멱등 도구로 제한된다.
- 도구 실행이 권한·안전 검사 등으로 차단되거나 확인을 요구한 일을 OpenTelemetry의 안전 이벤트로 관찰할 수 있다.
- macOS 키체인 잠금 및 절전 후 MCP 연결 복구, 대용량 PDF·이미지를 읽는 세션의 자동 압축, 클라우드 대화 재시작 안정성이 개선됐다.
- Claude API 코드를 2026-10-21 API 버전으로 옮기는 명령이 추가됐다. 자체 호스팅 체크아웃 훅에는 기본 30분 제한이 적용된다.
- 2.1.308은 일반적인 버그 수정과 신뢰성 개선으로 안내됐으며, 구체적 수정 목록은 공개되지 않았다.

## Sources

- [공식 CHANGELOG](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [2.1.307 릴리스](https://github.com/anthropics/claude-code/releases/tag/v2.1.307)
- [2.1.308 릴리스](https://github.com/anthropics/claude-code/releases/tag/v2.1.308)
