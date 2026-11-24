# RFC 9126 공개 번역판 2차 검수

2026년 11월 25일. [기존 원문 대조 기록](controller-review.md)의 후속 교정이다. [공식 원문](https://datatracker.ietf.org/doc/html/rfc9126), [블로그판](https://starryeye.github.io/rfc/rfc9126/), [보관판](https://starryeye.github.io/standard-document/rfc/rfc9126/)에 대응한다.

- [§7.2](index.html#section-7.2-1)의 한 문장을 교정했다. 인증은 새 redirect URI 수락의 필요조건이며, 인증이 됐다고 모든 새 URI를 수락할 의무가 생기지 않는다. [§2.4](index.html#section-2.4)의 서버 재량과 원문의 `MUST` 표기를 그대로 유지했다.
- 발행일 한 곳과 참고 문헌 날짜 19곳에 원문과 일치하는 `datetime` 값을 복원했다. 한국어 날짜 표시와 나열 순서는 그대로다.
- 가로로 넘치는 예제에만 스크롤 안내를 붙였다. 예제 10개의 텍스트·공백·줄바꿈을 유지했다. §5–6은 긴 식별자 아래에 정의를 두고, §9의 긴 코드 값은 구분자에서 줄을 바꿀 수 있게 했다. 식별자 값이나 링크는 그대로다.
- §2 편집 안내 제목은 JWT audience 규칙을 요약한다는 점을 명시했다. [RFC 10070 §5](https://www.rfc-editor.org/rfc/rfc10070.html#section-5)의 안내 본문과 링크, 2021년 번역 문단은 변경하지 않았다.

배포 전 Chromium에서 두 판을 각각 14개 너비(320–1,440px)에서 검사했다. 예제 스크롤 끝·안내의 표시 조건, 목차 31개, 날짜 값 20개, 정의 배치, 전체 페이지 가로 넘침 및 업데이트 링크를 확인했다. 390·768·1,440px에서 바뀐 문장과 안내, 예제, 정의 및 IANA 식별자를 직접 확인했다.

기존 승인 HTML·검수 기록·공통 스타일시트는 변경하지 않았다. 이 공개 수정본의 해시와 직전 공개본 해시는 [publication.json](publication.json)에 별도로 기록했다.
