# Claude Code

오늘 새로 반영할 기준은 Claude Code `2.1.207`입니다. 기본 npm 설치 경로의 `latest`와 공개 CHANGELOG가 저장된 `2.1.206`에서 한 단계 올라갔습니다.

## GUI App

- 최신 저장 기준을 `2.1.207`로 올렸습니다.
- background agent와 worktree session을 다시 연결하거나 복구하는 흐름이 더 안정적으로 바뀌었습니다.
- Remote Control은 연결이 끊겼다가 돌아올 때 상태와 진행 상황을 더 정확하게 복원합니다.
- agent teams의 잘못된 mailbox 데이터가 반복 crash를 일으키던 문제가 수정되었습니다.

## CLI App

- npm `@anthropic-ai/claude-code`의 기본 `latest`와 `next`는 `2.1.207`입니다. 별도 `stable` 태그는 계속 `2.1.197`입니다.
- Bedrock, Vertex AI, Foundry에서도 별도 환경변수 없이 Auto mode를 사용할 수 있으며, 필요하면 `disableAutoMode`로 끌 수 있습니다.
- Bedrock, Vertex, AWS 기반 Claude Platform의 기본 모델이 Claude Opus 4.8로 바뀌었습니다.
- 긴 목록, 표, 코드가 출력될 때 터미널이 멈추거나 키 입력이 늦어지고 완료 시 화면이 튀던 문제가 개선되었습니다.
- 플러그인 shell 명령에서 사용자 설정 값을 직접 확장하지 못하게 막아 shell injection 위험을 줄였습니다.
- 업데이트가 `~/.local/bin/claude`의 사용자 launcher나 symbolic link를 덮어쓰지 않도록 수정되었습니다.
- AWS SSO 인증 반복 요청, Windows AWS credential 확인 지연, background session 복구 문제를 포함한 안정성 수정이 들어갔습니다.

## Sources

- [Claude Code CHANGELOG](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [Claude Code raw CHANGELOG](https://raw.githubusercontent.com/anthropics/claude-code/main/CHANGELOG.md)
- [npm @anthropic-ai/claude-code](https://www.npmjs.com/package/@anthropic-ai/claude-code)
