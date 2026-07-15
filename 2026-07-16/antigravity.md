# Antigravity

오늘 새로 반영할 GUI 버전은 Antigravity 2.0 `2.3.0`입니다. 메시지를 순서대로 예약해 보내는 기능과 plain-text 파일 첨부가 추가되고, 긴 작업과 큰 diff의 안정성이 좋아졌습니다.

## GUI App

- 최신 저장 기준을 `2.2.1`에서 `2.3.0`으로 올렸습니다.
- 메시지를 queue에 넣고 실행 방식을 설정하거나, 필요한 메시지를 `Send Now`로 바로 보낼 수 있습니다.
- 대화에 `.txt` 파일을 첨부하고 내용을 표시할 수 있습니다.
- file watching과 초기화 순서를 다듬어 시작 속도를 개선했고, 일시적인 backend overload는 자동으로 다시 시도합니다.
- system theme을 기본값으로 따르며, queued-message 카드와 diff comment 버튼의 배치가 정리되었습니다.
- 가상화된 파일 화면의 `Cmd+F`, 1,000행이 넘는 파일의 diff 렌더링, archive 뒤 background task가 계속 도는 문제를 고쳤습니다.
- `/btw` 질문이 대화 전환 뒤에도 유지되고 agent의 생각 진행을 표시하며, subagent 종료 뒤 main agent가 멈추는 문제도 수정했습니다.

## IDE App

- 최신 저장 기준은 계속 Antigravity IDE `2.1.1`입니다.
- IDE release API에서 새 IDE release는 확인되지 않았습니다.

## CLI App

- 제품군 기준은 계속 `2.0`입니다.
- 설치 manifest의 별도 binary version은 계속 `1.1.2`입니다.
- 공개 changelog에서 CLI 전용 새 버전이나 변경 설명은 확인되지 않았습니다.

## Sources

- [Google Antigravity changelog](https://antigravity.google/changelog)
- [Google Antigravity releases](https://antigravity.google/releases)
- [Antigravity Hub release API](https://antigravity-hub-auto-updater-974169037036.us-central1.run.app/releases)
- [Antigravity IDE release API](https://antigravity-ide-auto-updater-974169037036.us-central1.run.app/releases)
- [Antigravity CLI manifest](https://antigravity-cli-auto-updater-974169037036.us-central1.run.app/manifests/darwin_arm64.json)
