# jjr-sunmoim — 순모임 주보

매주 순모임(소그룹 모임) 주보. 예배 순서, 나눔 질문, 합심기도, 순헌금 계좌, 한주간 기도제목을 담습니다.

- **주소**: https://cgn210-alt.github.io/jjr-sunmoim/sunmoim.html

## 파일 구성

- `sunmoim.html` — 주보 앱 (단일 파일)
- `og-image.jpg` — 카카오톡 등 링크 공유 시 뜨는 썸네일 이미지

## 사용 방법

- 순장이 "편집" 버튼을 눌러 비밀번호 입력 후 그 주 내용을 수정 → "공유하기"로 순원들에게 링크 전달
- 순원은 "한주간의 기도제목"에 실시간으로 이름/기도제목을 남길 수 있음
- 편집 비밀번호는 `sunmoim.html` 안의 `EDIT_PW` 상수에 설정되어 있음 (필요 시 코드에서 직접 변경)

## 백엔드

자체 Google Apps Script(`APPS_SCRIPT_URL`)를 통해 기도제목 실시간 취합 및 주보 내용 서버 저장.

## 배포

`사이트-올리기.bat` 더블클릭 → `git add / commit / push` 자동 실행 → GitHub Actions가 1~2분 내 자동 배포.
