# Cursor

오늘 새로 반영할 기준은 Cursor `3.11`입니다. 저장된 `3.9` 이후 `3.10`과 `3.11`이 공개 changelog에 추가되었습니다.

## GUI App

- 최신 저장 기준을 2026-07-10 Cursor `3.11`로 올렸습니다.
- `/side`, `/btw` 또는 plus 버튼으로 main agent 작업을 멈추지 않고 별도의 side chat을 열 수 있습니다.
- agent 대화 기록을 이름이나 PR 번호뿐 아니라 내용으로 검색할 수 있고, 현재 대화 안에서는 `Cmd+F` 검색을 사용할 수 있습니다.
- project와 repository 선택기가 단순해졌고, local, cloud, remote machine, multi-repo 위치를 선택기 안에서 바로 고를 수 있습니다.
- cloud agent hook이 prompt, response, thought, subagent, compaction, turn 완료까지 관찰하고 제어할 수 있도록 확장되었습니다.
- `3.10`에서는 관리자가 team MCP를 한 번 설정해 cloud agent, agent window, IDE, CLI에 배포하고 조직 그룹별 marketplace 접근을 제한할 수 있게 되었습니다.

## CLI App

- CLI 전용 새 안정 버전 번호는 공개 changelog에서 확인되지 않았습니다.
- 다만 team MCP 배포 대상에 CLI가 포함되므로 관리자가 승인한 MCP 설정을 CLI에서도 공유할 수 있습니다.
- 별도 CLI version baseline이 없어 `.version`의 CLI 값은 계속 `null`로 유지합니다.

## Sources

- [Cursor changelog](https://cursor.com/ko/changelog)
