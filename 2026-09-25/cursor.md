# Cursor 변경사항

## GUI App

- 버전: `3.11`
- 2026-09-23에 버전 번호 없는 새 기능 공지가 게시되었습니다. **Rollouts**와 **Security Review** 두 Cursor 봇을 Teams·기업 플랜에 출시했습니다.
- Rollouts는 PR마다 모니터를 붙이고 배포 과정을 환경별로 추적해 verified healthy / regression detected / inconclusive로 보고합니다. PR에 모니터링 플랜을 남기고, 회귀 시 작성자에게 알리며 설정에 따라 revert PR 초안이나 클라우드 Agent 수정을 맡길 수 있습니다. Origin·GitHub, CD, Datadog 등과 연결합니다.
- Security Review는 모든(초안 제외) PR을 코드베이스 맥락에서 읽고 악용 가능한 버그를 한 댓글로 정리합니다. 인젝션·인증/승인 우회·죽은 검사·커밋된 시크릿·SSRF·안전하지 않은 역직렬화·취약 의존성 등을 플래그합니다. 팀 규칙을 추가하면 모든 PR에 적용합니다.
- 앞으로 10일간 Teams 약 50건·기업 약 500건 분량의 Rollouts 사용 크레딧이 제공됩니다. 공지에 새 GUI 버전 번호는 없으므로 버전 기준선은 유지합니다.

## CLI App

- Cursor는 이 변경 로그에서 별도 CLI 버전을 게시하지 않습니다.
- 이전 기록 이후 새 CLI 공지는 확인되지 않았습니다.

## Sources

- [Cursor changelog](https://cursor.com/ko/changelog)
