# Antigravity
- 기준일: 2026-11-21 (Asia/Seoul)
- CLI 바이너리: **1.5.12 → 1.5.13** (공식 GitHub 릴리스). 앱·IDE·확장은 신규 버전 미확인.

## 달라진 점
- 개인 API 키 경로와 별개로, Application Default Credentials(ADC)와 기업 모델 게이트웨이에서도 Gemini 4 Neon을 이용할 수 있도록 지원 범위를 넓혔다.
- 명시적으로 `/swarm`을 요청하지 않았는데 에이전트가 자체적으로 스웜 작업을 시작해 사용량이 늘 수 있던 문제를 수정했다.
- 모델 요청 재시도가 성공했는데도 JSON 출력에 오류가 남거나, ACP를 통해 실행한 명령이 프로젝트 대신 에디터 시작 폴더에서 실행되던 문제를 수정했다.

## 출처
- [Google Antigravity · CLI 1.5.13 공식 릴리스](https://github.com/google-antigravity/antigravity-cli/releases/tag/1.5.13)
- [Google Antigravity · 공식 변경 로그](https://antigravity.google/docs/changelog)
