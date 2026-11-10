# Claude Code
- 기준일: 2026-11-11 (Asia/Seoul)
- 확인 시각: 2026-11-11 04:17 KST
- 비교 기준: main의 기존 .version 및 2026-11-10 기록

## 신규 안정판 2.1.321 · 2.1.322
기존 2.1.319 이후 공개된 두 버전을 확인했다. 확인일과 실제 릴리스 날짜는 구분한다.

### 2.1.322
- 공식 게시: 2026-11-10 02:29:43 UTC.
- Vertex AI의 global·us·eu 리전에서 빠른 모드를 지원한다. 빠른 처리를 사용할 수 없으면 일반 속도로 전환한다.

### 2.1.321
- 공식 게시: 2026-11-09 19:22:30 UTC.
- Claude Fable 5.2를 기본 Fable 모델로 추가했다. 100만 토큰 문맥을 지원한다.
- MCP 인증 리디렉션으로 비밀정보가 다른 호스트에 전달되거나, Bash·파일 복사/이동의 권한 검사가 빠지는 문제를 수정했다.
- 네트워크 드라이브의 파일·노트북 편집, 장시간 세션 메모리 사용, 원격 세션 재연결과 플러그인 중복 다운로드를 개선했다.
- Remote Control에 세션별 설정 파일을 지정하는 기능을 추가했다. 설정 파일 변경 후에는 재시작이 필요하다.

CLI 및 공개 변경 로그 버전만 **2.1.322**로 갱신했다. 기존 GUI 관찰값 **2.1.300**은 그대로 보존하며 이번 CLI 릴리스와 동일시하지 않는다.

## Sources
- [공식 변경 로그](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [공식 안정판 2.1.322](https://github.com/anthropics/claude-code/releases/tag/v2.1.322)
- [공식 안정판 2.1.321](https://github.com/anthropics/claude-code/releases/tag/v2.1.321)
