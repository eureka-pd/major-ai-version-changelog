# Claude Code 변경사항

2026-08-05 확인 결과, `2.1.220` 이후 `2.1.221`이 새로 기록되었습니다.

## GUI App

- VS Code 확장에 Focus view가 추가되었습니다. 도구 실행 내역을 접고, 현재 실행 중인 도구와 턴별 요약만 간단히 볼 수 있습니다.

## CLI App

- Linux와 WSL 샌드박스에서 자격 증명 파일을 가려서 다루는 `mode: "mask"` 옵션이 추가되었습니다. 명령은 실제 비밀값을 직접 읽지 못하고, 외부 통신에 필요할 때만 값이 적용됩니다.
- `claude plugin validate`는 Claude Desktop의 관리형 마켓플레이스 동기화에서 거부될 이름을 미리 경고합니다.

## Sources

- [Claude Code CHANGELOG](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
