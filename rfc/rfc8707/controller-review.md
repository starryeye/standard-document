# RFC 8707 공개판 교정 검수

[공식 영문](https://datatracker.ietf.org/doc/html/rfc8707) · [독립 읽기판](./) · [블로그 전문](https://starryeye.github.io/rfc/rfc8707/) · [공개판 무결성 기록](publication.json)

2020년 2월 발행본과 승인된 한국어 읽기판으로 공개판 교정 내용을 검수했다. 원문 캡처 SHA-256은 `451bbdc900ca3be74604c98ec8d71e36bd9ffec44d47400229e1a3d9930e6783`, [기존 승인 읽기판](reviewed.html)은 `da8eed2430120b9a20782a642122b455171ed9d7ef57f2af3ace350212ba2a19`이다. 기존 승인본과 검증 기록은 수정하지 않았다.

- [§1](https://datatracker.ietf.org/doc/html/rfc8707#section-1-1): `access token(액세스 토큰)` 풀이를 접힌 원문 목차 항목에서 실제 본문 첫 등장으로 옮겼다. client가 요청 중인 토큰의 사용처를 authorization server에 알린다는 뜻이나 적용 조건은 그대로다.
- [§2](https://datatracker.ietf.org/doc/html/rfc8707#section-2-4): 달리 판단할 구체적인 리소스 정보가 없다면 API 기본 URI를 사용하라는 권고다. 한국어 표현을 다듬고 `SHOULD`와 예외를 그대로 뒀다.
- [§2.1](https://datatracker.ietf.org/doc/html/rfc8707#section-2.1-3): authorization server가 client에게 대상 명시를 요구할 수 있다는 조사만 다듬었다. 생략 시 처리·요구·거부 모두 선택으로 유지했다.
- [§2.2](https://datatracker.ietf.org/doc/html/rfc8707#section-2.2-2): 일부 리소스용 access token과 반환 시 최초 인가 전체에 결부되는 refresh token의 구분을 다시 확인했다. 이 조항은 바꾸지 않았다.
- [RFC Editor 정오표 6810](https://errata.rfc-editor.org/search/?rfc_number=8707)은 §4의 편집상 오타를 정정한다. 번역에서는 이미 올바른 `authorization server`로 표시된다.

원문의 규범어 강조 23곳, HTML 날짜 속성 10개를 복원하고, 저자 세 명의 연락처에 그룹 간 여백을 주었다. 글과 표시 속성의 의도된 변경을 되돌리면 이전 승인 본문과 바이트 단위로 일치한다. 원문 링크와 앵커, 예제 6개의 공백·줄바꿈, 캡션과 숫자는 바뀌지 않았다. 발행본의 영문 저작권 고지와 비공식 번역 표시를 함께 뒀다.

배포 전 독립 읽기판과 기존 Jekyll 테마 미리보기를 1440·768·390px에서 검수했다. 교정 문장, 규범어 굵기, 저자 간격, 목차 점프, 열린 날짜와 원문 표기, 영문 고지를 직접 확인했다. 모바일에서 예제 6개마다 상자 안 가로 스크롤 끝까지 접근할 수 있고 문서 자체에 가로 넘침이 없음을 확인했다. 두 공개판에 같은 교정 본문 SHA-256 `501e306c43844b4bc32e18ae9a601157d4da90054c875c0ff9f9263a523e45ba`를 사용한다.
