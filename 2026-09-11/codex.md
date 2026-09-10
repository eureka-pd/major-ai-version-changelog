# Codex 변경사항

## GUI App

- 버전: `26.727`
- 이전 기록 이후 새 GUI 앱 버전은 확인되지 않았습니다.

## CLI App

- 버전: `0.154.0` (이전: `0.153.4`, 2026-09-09 공개)
- 모델 피커와 Amazon Bedrock 카탈로그에 GPT-6-Astra를 넣었습니다.
- 실험적 worktree로 `--worktree`·`/worktree`에서 격리 체크아웃을 만들고 목록·재개할 수 있습니다.
- Codex가 일하는 동안 선택지·직접 입력으로 인라인 질문에 답해도 본문 초안이 유지됩니다.
- Windows 세션이 백그라운드 Codex 서버를 공유하고, 데몬 수명 주기 명령과 관리 업데이트를 지원합니다.
- Vim `R` 치환 모드(실행 취소·점 반복)와 레거시 터미널 Escape 처리를 다듬었고, 응답 복사 시 서식을 유지하며 `/copy`로 상태·개별 필드를 복사할 수 있습니다.
- 기존 세션이 새로 설치한 플러그인 도구·스킬·훅을 다시 읽고, MCP OAuth 갱신을 맞추며, trust 전에 workspace 헬퍼를 돌리지 않고 macOS 샌드박스가 터미널 입력 주입을 막습니다.
- 원격 resume·fork가 저장 권한을 유지하고, 다른 앱에서 열린 대화를 resume하면 읽기 전용 트랜스크립트와 재시도 옵션을 보여 줍니다.
- 자동 승인 리뷰가 compaction 뒤에도 권한 맥락을 더 잘 지키고, 새 지시·답변으로 무효가 된 승인을 거절합니다.
- 번들 OpenAI Docs 스킬에 GPT-6-Astra 이전·호환·프롬프트 안내를 넣었고, deprecated `codex mcp-server` 진입점은 제거되었습니다.

## General

- 이전 기록 이후 새 공지는 확인되지 않았습니다.

## Mobile

- 버전: `1.2026.244`
- 이전 기록 이후 새 모바일 버전은 확인되지 않았습니다.

## Sources

- [OpenAI Codex changelog](https://developers.openai.com/codex/changelog)
