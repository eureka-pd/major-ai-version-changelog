# Codex 변경사항

## GUI App

- 버전: `26.908`
- 이전 기록 이후 새 GUI 버전은 확인되지 않았습니다. 최신은 2026-09-11 Pets Quick Chat·Windows Appshots입니다.

## CLI App

- 버전: `0.155.0` (이전: `0.154.0`, 2026-09-17)
- 실험적 `/voice` 대화(라이브 트랜스크립트·마이크, `/experimental`), TUI 상태 줄의 라이브 reasoning 요약·턴 완료 시각, agents overview에서 작업 숨김·보관·삭제와 worktree 소유자·정리된 managed worktree 확인 삭제를 넣었습니다.
- 지원 Mac에서 MCP 요청 Touch ID 검증, daemon 업데이트 일정 설정·`codex app-server daemon update`, daemon 재시작 후 저장 스레드·active goal 복구, Amazon Bedrock용 명령 기반 AWS 자격 증명(캐시·만료 갱신·재인증)을 추가했습니다.
- compaction 실패 시에도 수락한 프롬프트 보존, tmux resize·트랜스크립트 뷰포트·스레드 전환 후 stale history, MCP OAuth 만료·reconnect 안내, 자동 승인 리뷰의 액션·권한 증거 보존·일시 실패 재시도, 계정 전환 시 remote-control·WebSocket·모델 카탈로그 무효화, WSL 샌드박스 탈출·셸 스냅샷 자격 노출을 고쳤습니다.
- Python SDK·런타임 게시를 안정 CLI 버전과 맞췄습니다.

## General

- 이전 기록에서 이미 반영한 2026-09-14 GPT-5.5 종료(2026-10-14, `gpt-5.6-sol` 전환) 외에 새 공지는 없습니다.

## Mobile

- 버전: `1.2026.244`
- 이전 기록 이후 새 모바일 버전은 확인되지 않았습니다.

## Sources

- [OpenAI Codex changelog](https://developers.openai.com/codex/changelog)
