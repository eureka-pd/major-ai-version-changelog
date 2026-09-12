# Antigravity 변경사항

## GUI App

- 버전: `2.13.0` (이전: `2.12.2`, 2026-09-09)
- Documents 섹션과 조직·제어 UX를 중심으로 개선 16건·수정 16건입니다. 새 버전은 점진 배포라 모든 사용자에게 바로 오지 않을 수 있습니다.
- Google Drive·PDF·Office 같은 외부 파일이 Artifacts 위 Documents 섹션에 모이고, Scratch Files는 접을 수 있는 전용 섹션으로 분리됩니다.
- Review Changes·파일 diff에 “Hide Whitespace Changes”, SQL·JSONL 등 코드·데이터 아티팩트용 가상화 뷰어(구문 강조·줄 번호·인라인 댓글)를 넣었습니다.
- 샌드박스 실행 명령에 문서 링크 shield 배지, 설정 파싱 실패 시 경로·복사 버튼 경고, side question을 작곡기 툴바 버튼으로 최소화·복원·삭제할 수 있습니다.
- 대화형 질문 Cancel과 단축키(macOS Ctrl+C, Linux/Windows Ctrl+D), 선택 텍스트를 채팅에 인용·추가(Cmd/Ctrl+L·I), 명령 팔레트에서 대화 pin/unpin·rename·archive(archive 시 홈으로 이동)를 지원합니다.
- 리뷰 댓글은 전송 시 입력·diff에서 바로 지우고 실패 시 복원합니다. 토스트 기본 8초, 모델 쿼터 패널 여백·높이, 작업 완료음 볼륨을 조정했습니다.
- 반복 미닫힘 HTML로 대화 크래시, 모델 셀렉터 빈 그룹 크래시, 스크린 리더 빠른 상태·반복 알림 누락, 권한 거절 단계 삭제(Rejected로 유지), 타 프로젝트 아티팩트 재승인 요청을 고쳤습니다.
- Enterprise/Business 모델 셀렉터 usage 패널 제거, 입력 위 카드 여백, 경로·picker 자동수정 끄기, hover 카드 잔존, 하단 근처 autoscroll, 인용 줄바꿈, scroll-to-bottom·툴팁, 보조 패널 너비 기억, 실패 턴 복사, `.ico` 미리보기, 보조 패널 정렬을 고쳤습니다.

## IDE App

- 버전: `2.5.5`
- 이전 기록 이후 새 IDE 버전은 확인되지 않았습니다.

## CLI App

- 제품 탭: `2.0`, 바이너리: `1.2.0`
- 이전 기록 이후 새 CLI 버전은 확인되지 않았습니다. 최신 바이너리는 2026-09-10 `1.2.0`입니다.

## Sources

- [Google Antigravity changelog](https://antigravity.google/changelog)
