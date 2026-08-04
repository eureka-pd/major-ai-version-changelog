# Antigravity 변경사항

2026-08-05 확인 결과, Antigravity 앱 `2.5.0`과 CLI `1.1.10`이 새로 기록되었습니다.

## GUI App

- `2.5.0`은 Gemini Enterprise 계정과 Workforce Identity Federation 로그인을 지원합니다. 조직 계정과 정책을 적용한 상태로 사용할 수 있습니다.
- 모델별 추론 강도 선택, 프로젝트 선택 검색·키보드 이동, 파일 뷰어의 경로 표시 등 작업 흐름이 개선되었습니다.
- 파일·아티팩트 뷰어 충돌, 빈 작업공간 시작 멈춤, OAuth 인증 문제 등 안정성 문제도 수정되었습니다.

## IDE App

- 최신 IDE 버전 `2.1.1` 유지. 새 IDE 전용 릴리스 없음.

## CLI App

- CLI `1.1.10`은 Gemini Enterprise, WIF, Application Default Credentials 인증을 추가했습니다.
- 샌드박스의 `.git` 접근은 읽기 전용으로 바뀌어 저장소 정보를 확인하면서도 내부에서 수정하지 못하게 했습니다.
- `--model`과 `--effort`가 무시되던 문제, 하위 에이전트를 중단해도 일부가 계속 실행되던 문제 등을 수정했습니다.

## Sources

- [Google Antigravity changelog](https://antigravity.google/changelog)
