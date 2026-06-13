# Claude Code

- 확인 결과: Claude Code에는 새 버전이 있습니다.
- 이전 저장 기준: `2.1.175` (2026-06-12)
- 최신 확인 기준: npm package `2.1.177` (publish: 2026-06-13)
- changelog 공개 기준: `2.1.176`까지 상세 변경 내용이 공개되어 있습니다.
- 중복 보고 방지 상태: `.version`의 Claude Code GUI/CLI 기준을 `2.1.177`로 저장했습니다.
- 출처: [Claude Code CHANGELOG](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md), [npm @anthropic-ai/claude-code](https://www.npmjs.com/package/@anthropic-ai/claude-code)

## GUI App

### `2.1.177`

- npm에는 `2.1.177`이 최신 패키지로 올라왔습니다.
- 다만 요청된 GitHub changelog 페이지에는 아직 `2.1.177`의 상세 항목이 공개되어 있지 않습니다.
- 그래서 버전 기준은 `2.1.177`로 갱신하되, 아래 상세 설명은 changelog에 공개된 `2.1.176` 항목 기준으로 정리합니다.

### `2.1.176`

- 대화 언어에 맞춰 session title이 자동 생성됩니다. 예를 들어 한국어로 대화하면 제목도 한국어에 맞춰질 수 있습니다.
- footer row에 표시되는 link badge를 regex로 잡아낼 수 있는 `footerLinksRegexes` 설정이 추가되었습니다.
- Bedrock 인증 정보 캐싱이 개선되어 `awsCredentialExport`가 준 만료 시간까지 credential을 재사용합니다.
- `availableModels` 제한이 더 강하게 적용됩니다. 환경 변수 alias로 차단된 모델을 우회하거나 `/fast`가 허용 목록 밖 모델로 바꾸는 일이 막혔습니다.
- Fable 5 auto mode, hook path 조건, Linux sandbox symlink, tmux/SSH clipboard, Remote Control, `/cd`, background session, Windows daemon, cloud session 인증 등 여러 안정성 문제가 수정되었습니다.

## CLI App

- npm 기준 최신 패키지는 `2.1.177`입니다.
- CLI 사용자는 `availableModels` enforcement, Bedrock credential caching, hook path matching, tmux clipboard, `/cd`, background session, Remote Control 관련 수정의 영향을 받습니다.
- 운영 관점에서는 모델 정책 우회 가능성이 줄고, remote/background 작업 상태가 더 정확하게 유지되는 업데이트입니다.
