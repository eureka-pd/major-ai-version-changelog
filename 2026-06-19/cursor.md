# Cursor

오늘 Cursor는 2026-06-18 changelog 항목을 새로 반영했습니다. 별도 새 제품 버전 번호는 표시되지 않았지만, 저장 기준일은 2026-06-18로 올렸습니다.

## GUI App

- 최신 저장 기준: Cursor `3.7`, changelog date `2026-06-18`
- `/automate` skill이 추가되어 local agent session에서 자연어로 자동화를 만들 수 있습니다. Cursor가 trigger, instruction, tool 설정을 대신 구성합니다.
- Slack 메시지에 지정한 emoji reaction을 달면 자동화를 실행할 수 있습니다.
- GitHub trigger가 늘었습니다. issue comment, PR review comment, PR review submit, review thread update, workflow run complete 이벤트를 자동화 시작점으로 쓸 수 있습니다.
- 실패한 GitHub Actions 처리와 PR 리뷰 댓글 자동 수정을 위한 marketplace template이 추가됐습니다.
- cloud Agent automation은 전용 computer use tool로 데모나 결과물을 만들 수 있고, 이 도구는 automation에 기본 활성화됩니다.
- automation을 미완성 상태로 저장하고 MCP 인증 같은 설정을 마친 뒤 이어서 진행할 수 있습니다.
- automation이 기본적으로 PR을 열 수 있게 되어, UI에서 별도 도구를 매번 지정할 필요가 줄었습니다.
- UI에서 memory file을 삭제하거나, automation 실행 시 오래된 memory를 삭제하도록 지시할 수 있습니다.

## CLI App

- CLI 전용 새 안정 버전 번호는 확인되지 않았습니다.
- 이번 항목은 Cursor automation과 cloud Agent 중심의 제품 변경입니다.

## Sources

- [Cursor changelog](https://cursor.com/ko/changelog)
