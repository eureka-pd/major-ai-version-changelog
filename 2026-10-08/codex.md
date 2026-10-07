# Codex 변경사항

기준일: 2026-10-08 (Asia/Seoul). CLI 안정판과 모바일 릴리스 각 1건을 새로 확인했습니다.

## GUI App

- `26.924` (공식 표시일 2026-09-25); 변경 없음.

## CLI App

### 0.161.0

- 이전 기록: `0.160.1`.
- 공식 공개: 2026-10-07 15:58:45 UTC, 한국 시간 2026-10-08 00:58:45.
- 기본 모델을 GPT-6.1 Sol로 변경했습니다. 지원하는 Bedrock 모델에서는 다중 에이전트 V2와 Ultra 추론을 사용할 수 있습니다.
- 실행 중인 터미널에서 `/mcp login <name>`으로 MCP 서버에 로그인하고, 음성 대화의 마이크·스피커·입력 채널을 선택할 수 있습니다.
- Daybreak는 `--enable cli_daybreak` 또는 `features.cli_daybreak=true`로 명시적으로 켜야 합니다. 기존 `daybreak=true`만으로는 활성화되지 않습니다.
- 백그라운드 작업의 권한 유지, 재연결 후 설정 유지, 대화 재개 시 최신 기록 복원, 과부하 재시도와 Windows 실행 안정성을 개선했습니다.

## General / Mobile

### iOS 1.2026.272

- 이전 기록: `1.2026.267`. 공식 표시일: 2026-10-07.
- 응답 안에 페이지 미리보기가 표시되고, iOS에서 Codex 작업 링크를 바로 열 수 있습니다.
- 권한 선택창을 알기 쉽게 정리하고 플러그인 메뉴를 통합했습니다.
- 긴 대화의 응답 표시, 연결 후 작업 목록, 오프라인 컴퓨터 선택 유지와 작업 트리 처리를 개선했습니다.
- 공식 통합 변경 로그의 ChatGPT for iOS 항목을 기존 모바일 분류로 기록합니다.

### General

- 최신 일반 공지는 2026-09-29 GPT-6.1 Sol로 유지됩니다. 이미 기록한 공지는 재집계하지 않습니다.

## 확인 기준

- 지정 URL은 현재 ChatGPT Learn 통합 변경 로그로 연결됩니다.
- CLI는 GitHub 최신 안정판 기준이며 알파판은 제외합니다. 모바일 표시일에는 시각·시간대가 없어 임의 변환하지 않았습니다.

## Sources

- [OpenAI Codex changelog](https://developers.openai.com/codex/changelog)
- [현재 공식 통합 변경 로그](https://learn.chatgpt.com/docs/changelog)
- [Codex CLI 0.161.0 공식 릴리스](https://github.com/openai/codex/releases/tag/rust-v0.161.0)
