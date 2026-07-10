# Claude Code

오늘 새로 반영할 기준은 Claude Code `2.1.206`입니다. 기본 npm 설치 경로의 `latest`가 저장된 `2.1.195`에서 `2.1.206`으로 올라갔고, 공개 CHANGELOG에도 같은 버전까지 반영되었습니다.

## GUI App

- 최신 저장 기준을 `2.1.206`으로 올렸습니다.
- Claude in Chrome이 정식 제공되었고, background agent 상태와 완료·입력 요청 알림을 `claude agents`에서 더 분명하게 확인할 수 있습니다.
- background agent는 기본적으로 뒤에서 실행되며, worktree 작업을 마치면 commit, push, draft PR 생성까지 이어갈 수 있습니다.
- background session의 재연결, 중지, SSH 시작, 저메모리 안내, Remote Control 상태 동기화 문제가 여러 차례 수정되었습니다.
- agent 목록의 상태 표시와 완료 세션 정리가 개선되어 오래 실행한 작업을 관리하기 쉬워졌습니다.

## CLI App

- npm `@anthropic-ai/claude-code`의 기본 `latest`와 `next` 설치 버전은 `2.1.206`입니다.
- 별도 `stable` 태그는 `2.1.197`이며, 이 저장소는 기존처럼 기본 설치 경로인 `latest`를 기준으로 기록합니다.
- Claude Sonnet 5가 기본 모델이 되었고, 기본 1M-token context window를 지원합니다.
- 여러 slash skill을 한 명령에서 최대 5개까지 연속으로 불러올 수 있게 되었습니다.
- 기본 permission mode의 표시 이름이 `Manual`로 정리되었고, `AskUserQuestion`은 사용자가 별도로 설정하지 않으면 자동으로 넘어가지 않습니다.
- `/cd` 경로 자동완성과 과도하게 긴 `CLAUDE.md` 정리를 제안하는 `/doctor` 검사가 추가되었습니다.
- `/commit-push-pr`은 저장소에 설정된 push remote로 보내는 정상적인 `git push`를 자동 허용할 수 있습니다.
- SSL 인증서 오류, 일시적 네트워크·rate limit, Windows worktree 정리, background daemon과 hook 오류 처리 안정성이 개선되었습니다.

## Sources

- [Claude Code CHANGELOG](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [Claude Code raw CHANGELOG](https://raw.githubusercontent.com/anthropics/claude-code/main/CHANGELOG.md)
- [npm @anthropic-ai/claude-code](https://www.npmjs.com/package/@anthropic-ai/claude-code)
