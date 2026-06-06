# Claude Code

- 확인 결과: 새 버전이 있습니다.
- 이전 저장 기준: `2.1.165`
- 최신 확인 기준: `2.1.167`
- 중복 보고 방지 상태: `.version`을 `2.1.167`로 갱신했습니다.
- 출처: [Claude Code CHANGELOG](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)

## GUI App

### `2.1.167`

- 공개 changelog 기준으로 버그 수정과 안정성 개선 릴리스입니다.
- 쉽게 말하면, 큰 새 기능보다는 최신 안정화 패치입니다.

### `2.1.166`

- 기본 모델이 과부하이거나 사용할 수 없을 때 순서대로 시도할 fallback 모델을 설정할 수 있게 됐습니다.
- deny 규칙에서 도구 이름 위치에 glob 패턴을 쓸 수 있게 됐고, 알 수 없는 도구 이름은 시작 시 경고합니다.
- 다른 Claude 세션에서 전달된 메시지가 사용자 권한을 대신 갖지 못하도록 cross-session messaging을 더 엄격하게 막았습니다.
- 생각 토큰을 끄는 설정이 기본적으로 thinking을 쓰는 모델에도 더 일관되게 적용됩니다.
- 업데이트 다운로드 전에 목표 버전을 먼저 알려주도록 바뀌었습니다.
- 이미지 처리 실패, 원격 세션 stuck, JetBrains 터미널 flicker, Windows PowerShell 검증 지연, macOS orphan process CPU 사용 등 여러 안정성 문제가 수정됐습니다.
- 쉽게 말하면, 모델 장애 대비, 권한 안전성, 터미널/원격 세션 안정성이 좋아진 업데이트입니다.

## CLI App

- Claude Code CLI도 같은 `2.1.167` 기준으로 추적합니다.
- `2.1.166`의 fallback 모델, deny 규칙, thinking 비활성화, `claude update`, `claude agents`, PowerShell/macOS/터미널 관련 수정은 CLI 사용 흐름에 직접 영향을 줍니다.
- 쉽게 말하면, CLI에서 장애가 났을 때 버티는 힘과 권한·터미널 안정성이 개선됐습니다.
