# Claude Code

오늘 새로 반영할 기준은 Claude Code `2.1.195`입니다. 기본 npm 설치 경로의 `latest`가 `2.1.193`에서 `2.1.195`로 올라갔고, 공개 CHANGELOG에도 같은 버전 항목이 올라왔습니다.

## GUI App

- 최신 저장 기준을 `2.1.195`로 올렸습니다.
- fullscreen mode에서 mouse click, drag, hover만 끄고 wheel scroll은 유지할 수 있는 `CLAUDE_CODE_DISABLE_MOUSE_CLICKS` 설정이 추가되었습니다.
- macOS voice dictation이 기본 입력 장치 변경 후 긴 세션에서 무음을 잡던 문제가 수정되었습니다.
- Japanese, Chinese, Thai처럼 공백 없이 쓰는 언어에서 voice dictation auto-submit이 동작하지 않던 문제가 수정되었습니다.
- crashed background task를 다시 열 때 최대 5초 동안 blank screen이 보이던 문제가 수정되었습니다.
- background agent daemon의 control socket 시작 실패가 restart를 막던 문제가 수정되었습니다.
- `claude agents` 완료 목록이 작은 터미널에서도 더 많은 세션을 보여주도록 개선되었습니다.
- Remote session 시작 중 provisioning checklist를 보여주도록 개선되었습니다.

## CLI App

- npm `@anthropic-ai/claude-code`의 기본 `latest` 설치 버전은 `2.1.195`입니다.
- `next` 태그도 `2.1.195`를 가리킵니다.
- npm의 별도 `stable` 태그는 아직 `2.1.181`에 머물러 있지만, 이 저장소의 기준은 기존처럼 기본 설치 경로인 `latest`를 따릅니다.
- hyphen이 들어간 hook matcher가 의도치 않게 substring match 되던 문제가 수정되어 이제 정확히 일치해야 합니다. 예를 들어 hyphenated MCP 서버 전체를 잡으려면 `mcp__brave-search__.*`처럼 써야 합니다.
- project `.claude/settings.json`만으로 활성화된 external plugin이 일부 loader path에서 설치 동의를 반복 요구하던 문제가 수정되었습니다.
- `/plugin` Enable/Disable이 plugin manifest 이름과 marketplace 이름이 다를 때 동작하지 않던 문제가 수정되었습니다.
- newer Claude Code가 쓴 background job이 `claude agents`에서 사라지거나 데이터를 잃던 문제가 수정되었습니다.
- Linux voice mode는 SoX가 설치되어 있지만 capture device가 없을 때와 SoX 자체가 없을 때를 구분해서 안내합니다.

## Sources

- [Claude Code CHANGELOG](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [Claude Code raw CHANGELOG](https://raw.githubusercontent.com/anthropics/claude-code/main/CHANGELOG.md)
- [npm @anthropic-ai/claude-code](https://www.npmjs.com/package/@anthropic-ai/claude-code)
