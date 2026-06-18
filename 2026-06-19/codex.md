# Codex

오늘 Codex는 CLI 안정 버전이 `0.141.0`으로 올라갔습니다. Codex app `26.609`와 ChatGPT for iOS `1.2026.160`은 기존 저장 기준과 같습니다.

## GUI App

- 최신 앱 버전 저장 기준: `26.609`
- 새 GUI 앱 버전 번호는 확인되지 않았습니다.
- 2026-06-16 지역 제공 범위 공지는 기존 기준과 같습니다.
- EEA, UK, Switzerland의 Computer Use, Chrome extension, Memories, Chronicle 제공 범위도 이미 반영된 상태입니다.

## CLI App

- 최신 저장 기준: `0.141.0`
- npm `@openai/codex`의 `latest` 태그가 `0.141.0`으로 올라갔고, GitHub release도 `0.141.0`을 latest로 표시합니다.
- remote executor 통신에 인증된 end-to-end encrypted Noise relay channel이 적용됐습니다. 원격 실행 연결을 더 안전하게 다루기 위한 변경입니다.
- cross-platform remote execution에서 executor 쪽 working directory, shell, filesystem permission path를 더 정확히 보존합니다.
- 선택한 executor plugin이 thread별 stdio MCP server를 활성화할 수 있고, plugin discovery에는 내가 만든 marketplace와 인증 방식별 curated catalog가 추가됐습니다.
- app-server client는 즉시 하위 thread를 조회하고, 외부 agent import 결과와 rate-limit reset credit을 다룰 수 있습니다.
- realtime client는 speech append와 response 주입 방식을 더 명시적으로 제어할 수 있습니다.
- TUI input prompt는 일정 시간 입력이 없으면 countdown 뒤 자동 resolve할 수 있습니다.
- Windows sandbox, hook trust, plugin capability routing, idle relay, SQLite WAL reset, enterprise proxy TLS 관련 버그가 수정됐습니다.

## Mobile

- 최신 저장 기준: ChatGPT for iOS `1.2026.160`
- 새 모바일 버전 번호는 확인되지 않았습니다.
- workspace file browser, directory picker, diff expand/collapse, MCP approval 선택지는 기존 기준과 같습니다.

## Sources

- [OpenAI Codex changelog](https://developers.openai.com/codex/changelog)
- [OpenAI Codex GitHub releases](https://github.com/openai/codex/releases)
- [npm @openai/codex](https://www.npmjs.com/package/@openai/codex)
