# Claude Code
- 기준일: 2026-11-26 (Asia/Seoul)
- **CLI 2.1.331 → 2.1.332**. GitHub 게시 시각은 11월 25일 01:32 UTC(한국 10:32)다.
- MCP 서버가 제공하는 스킬을 베타로 지원한다. 슬래시 메뉴에서 `서버:스킬` 형태로 표시된다. 새 `PreSkillShellCommand` 훅에서 스킬을 불러올 때 인라인 셸 명령을 거부할 수 있다. 이전 버전과 설정을 공유한다면 이 훅을 선언한 설정이 2.1.331 이하에서 시작 대화상자를 띄울 수 있다.
- 반복된 자동 압축 실패로 긴 대화가 끝나거나 로컬 MCP 서버가 출력을 과도하게 내보낼 때 터미널이 멈추던 문제를 수정했다. VS Code와 Desktop의 Code 탭에서 재개한 대화의 이전 메시지를 불러오지 못했을 때 이를 표시한다.
- Desktop 앱의 별도 배포 버전은 변경하지 않았다.

## 출처
- [Anthropic · v2.1.332 릴리스](https://github.com/anthropics/claude-code/releases/tag/v2.1.332)
- [Anthropic · 공식 변경 로그](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
