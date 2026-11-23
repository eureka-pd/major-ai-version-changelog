# Antigravity
- 기준일: 2026-11-24 (Asia/Seoul)
- **CLI 바이너리 1.5.14 → 1.5.15**. 공식 GitHub에 11월 23일 게시됐다. 앱 **2.34.0**, IDE **2.8.0**은 유지.
- 자동 대화 압축 시점을 토큰 수 또는 모델 컨텍스트의 백분율로 지정할 수 있고 `/context`에서 현재 기준을 볼 수 있다. 기본 로컬 대화 저장에서 최근 500개 초과분을 자동으로 정리하던 동작도 제거했다.
- Planner·Executor의 미설정 기본 추론 강도는 지원하는 경우 `high`로 바뀌었다. 이미 저장한 오케스트레이터 설정은 그대로다.
- ACP에서 긴 세션을 불러올 때 기록이나 권한 요청이 누락되던 문제, 백그라운드 작업이 끝나기 전에 턴을 종료하던 문제 등을 수정했다. 원격 제어의 프로젝트 선택도 개편했다.

## 출처
- [Google · Antigravity CLI 1.5.15 릴리스](https://github.com/google-antigravity/antigravity-cli/releases/tag/1.5.15)
- [Google · Antigravity 공식 변경 로그](https://antigravity.google/docs/changelog)
