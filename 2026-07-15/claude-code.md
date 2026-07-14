# Claude Code

오늘 새로 반영할 Claude Code 버전은 `2.1.208`과 `2.1.209`이며, 최신 기준은 `2.1.209`입니다. 접근성, background agent 안정성, 대용량 출력 처리가 크게 개선되었습니다.

## GUI App

- 최신 저장 기준을 `2.1.207`에서 `2.1.209`로 올렸습니다.
- `2.1.208`은 화면 낭독기용 plain-text 모드와 fullscreen 다중 선택 메뉴의 마우스 클릭을 지원합니다.
- model 변경 뒤 fast mode가 꺼진 채 남는 문제, background agent 답변이 전달 실패 때 사라지는 문제, 업데이트 뒤 background session에 다시 붙지 못하는 문제를 고쳤습니다.
- `2.1.209`는 `claude agents` background session에서 `/model` 같은 dialog가 막히던 회귀를 되돌렸습니다.

## CLI App

- npm `latest`와 `next`는 모두 `2.1.209`입니다.
- vim insert mode에서 `jj` 같은 두 글자 조합을 Escape로 바꾸는 `vimInsertModeRemaps` 설정이 추가되었습니다.
- 기업용 launcher를 거치도록 모든 Claude Code 자체 실행을 감싸는 `CLAUDE_CODE_PROCESS_WRAPPER`를 지원합니다.
- `claude -p`의 큰 JSON/stream-json 출력이 잘리거나 종료 결과가 빠지는 문제, 긴 session의 메모리 누수, 200행이 넘는 markdown 표의 렌더링 정지를 줄였습니다.
- Edit, Read, Grep, Glob의 경계 사례와 환경 변수의 과학적 표기 값 처리 오류도 수정했습니다.

## Sources

- [Claude Code CHANGELOG](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [Claude Code raw CHANGELOG](https://raw.githubusercontent.com/anthropics/claude-code/main/CHANGELOG.md)
- [npm @anthropic-ai/claude-code](https://www.npmjs.com/package/@anthropic-ai/claude-code)
