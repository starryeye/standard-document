# RFC 9101 원문·번역판 검토 및 공개 교정

[IETF 영문 발행본](https://datatracker.ietf.org/doc/html/rfc9101) · [공개 읽기판](index.html) · [블로그](https://starryeye.github.io/rfc/rfc9101/)

2021년 8월 발행본과 한국어 읽기판을 초록부터 저자 연락처까지 직접 비교했다. RFC 9101이 규정하는 `request` / `request_uri`, URI 512자 권고, Request Object의 `client_id` 일치 의무, JWS와 JWE 검증 범위, 개인정보 절의 일회 사용 및 엔트로피 조건을 점검했다. 원문에서 크게 달라진 조건이나 본문 누락은 발견하지 않았다. 컴퓨터 과학 용어와 프로토콜 식별자는 영어 표기를 유지했다.

기존 독립 검토를 바탕으로 공개본에만 다음을 바꿨다.

- §5.2.3의 제목과 두 목차에서 authorization server가 Request Object를 가져오는 주체임을 분명히 했다. 절의 본문은 바꾸지 않았다.
- 원문의 BCP 14 키워드 83곳과 날짜 `datetime` 속성 27개를 대응 위치로 복원했다. 규범 키워드 및 화면의 날짜 문구는 바꾸지 않았다.
- 저자 연락처 세 그룹 사이에 여백을 주었다. HTTP·JSON·JWT·URL 예제 11개는 줄바꿈까지 원문과 같다.

블로그와 독립 읽기판의 변경 지점을 Chromium 1440·768·390px 화면에서 직접 확인했다. 접힌 목차·문서 정보·원문 페이지 표기를 열었고, 목차 링크 이동과 모바일 코드 상자 스크롤을 확인했다. 두 사이트의 본문 조각은 동일하다.

검수 원본 [reviewed.html](reviewed.html) 및 [article.html](article.html)과 해당 [manifest](manifest.json)는 변경하지 않았다. [publication.json](publication.json)은 별도 공개본과 스타일의 해시를 기록한다. 이 문서는 비공식 AI 한국어 번역이며, 해석의 기준은 IETF 공식 영문이다.
