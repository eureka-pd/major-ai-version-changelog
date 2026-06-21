# Claude Code

Claude Code는 새 안정 버전 `2.1.185`가 확인되었습니다. 저장 기준이던 `2.1.183` 이후 새로 보고할 항목입니다.

## GUI App

- 최신 저장 기준을 `2.1.183`에서 `2.1.185`로 갱신했습니다.
- 공식 changelog 최신 항목은 `2.1.185`입니다.
- 이번 변경은 API 응답이 잠시 멈춘 것처럼 보일 때 표시되는 안내 문구를 더 정확하게 바꾼 항목입니다.
- 기존에는 10초 침묵 후 “응답 없음, 재시도 중”처럼 보였지만, 이제는 20초 침묵 후 “API 응답 대기 중, 곧 재시도”라는 의미로 보여 줍니다.
- 사용자가 장애처럼 오해하기 쉬운 순간을 줄이고, 실제로는 재시도 대기 상태임을 더 분명히 알려 주는 UX 수정입니다.

## CLI App

- npm `@anthropic-ai/claude-code` latest도 `2.1.185`입니다.
- npm dist-tag 기준 `latest`와 `next`는 `2.1.185`, `stable`은 `2.1.176`으로 확인했습니다.
- CLI 관점에서도 같은 변경입니다. 긴 응답 대기 중 터미널 안내가 더 늦게, 더 정확한 문구로 나타납니다.
- 별도 `2.1.184` public changelog 섹션은 확인되지 않았습니다. 이번 보고는 공개 changelog에 있는 `2.1.185` 항목만 반영합니다.

## Sources

- [Claude Code CHANGELOG](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [npm @anthropic-ai/claude-code](https://www.npmjs.com/package/@anthropic-ai/claude-code)
