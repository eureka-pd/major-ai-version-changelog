# SUMMARY

오늘은 `.version` 파일이 비어 있어 모든 항목을 최초 기준으로 기록했습니다. 다음 실행부터는 아래 버전들이 다시 보고되지 않습니다.

## Claude Code

### GUI App

- 최신 기준: `2.1.165`
- 공개 설명은 버그 수정과 안정성 개선입니다.
- 직전 상세 릴리스 `2.1.163` 기준으로는 Stop 동작, 터미널 표시, 패널 닫힘 후 잔여 표시, 백그라운드 세션 같은 앱 사용 중 불편한 부분이 많이 고쳐졌습니다.
- 쉽게 말하면, 눈에 띄는 새 기능보다 앱이 덜 멈추고 덜 깨지도록 다듬은 업데이트입니다.

### CLI App

- 최신 기준: `2.1.165`
- 조직에서 허용 버전 범위를 강제하는 설정, `/plugin list`, hooks 추가 컨텍스트 전달, resume/Bedrock/Vertex/Foundry/Windows/Bash 관련 수정이 확인됐습니다.
- 쉽게 말하면, 회사 관리자가 버전을 통제하기 쉬워졌고 CLI가 여러 개발 환경에서 더 안정적으로 동작하게 됐습니다.

## Codex

### GUI App

- 최신 기준: Codex app `26.602` (2026-06-04)
- 프로필 활동 인사이트와 공유 카드가 추가됐고, Computer Use 시작 준비, appshot 오류 보고, 브라우저/리뷰/터미널 UI 문제가 개선됐습니다.
- 최근 추가로 Sites 프리뷰와 iOS Codex 잠금/Windows SSH 연결 지원도 확인됐습니다.
- 쉽게 말하면, 앱 안에서 사용 현황을 보기 좋아졌고 화면과 시작 안정성이 좋아졌습니다.

### CLI App

- 이번 최신 changelog에는 CLI 전용 새 버전 번호가 따로 보이지 않았습니다.
- 일반 항목으로 Amazon Bedrock 모델 제공자 지원이 확인됐습니다.
- 쉽게 말하면, CLI 전용 릴리스보다는 로컬 Codex가 쓸 수 있는 모델 제공자 선택지가 늘어난 변화입니다.

## Cursor

### GUI App

- 최신 기준: `3.7` (2026-06-04)
- 캔버스 디자인 모드, 컨텍스트 사용량 보고서, 브라우저 전체 화면 공유 캔버스, 클릭 실행 버튼, 캔버스 오류 수정과 차트/스타일 개선이 추가됐습니다.
- 쉽게 말하면, Cursor가 만든 화면을 직접 찍어 고치고, 토큰이 어디에 쓰이는지 더 쉽게 확인할 수 있습니다.

### CLI App

- 이번 `3.7` changelog에는 CLI 전용 새 버전 변경사항은 따로 보이지 않았습니다.
- 쉽게 말하면, 이번 Cursor 업데이트는 캔버스와 GUI 작업 경험 중심입니다.

## Antigravity

### GUI App

- 최신 기준: Antigravity IDE `2.0.1` (2026-05-19)
- Antigravity 2.0 출시 직후 버그 수정 릴리스입니다.
- CJK 프로젝트 제목 마이그레이션, 1.0 가져오기 중 프로젝트 중복 생성, Google One 크레딧 미적용 문제가 수정됐습니다.
- 쉽게 말하면, 2.0으로 넘어갈 때 프로젝트와 크레딧이 꼬이던 문제를 바로잡은 업데이트입니다.

### CLI App

- CLI는 Antigravity 2.0의 터미널 중심 인터페이스로 안내되어 있습니다.
- 오늘 확인한 changelog 최신 항목은 IDE `2.0.1`이고, CLI 전용 별도 버전 변경사항은 확인되지 않았습니다.
- 쉽게 말하면, CLI는 2.0 플랫폼을 터미널에서 쓰는 가벼운 입구이며 이번 기준 버전은 IDE changelog 기준으로 저장했습니다.

## Sources

- [Claude Code CHANGELOG](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [OpenAI Codex changelog](https://developers.openai.com/codex/changelog)
- [Cursor changelog](https://cursor.com/ko/changelog)
- [Google Antigravity changelog](https://antigravity.google/changelog?app=antigravity-ide)
- [Antigravity CLI product page](https://www.antigravity.google/product/antigravity-cli)
