# RFC 7523 — 발행본과 한국어판 대조

[IETF Datatracker의 2015년 5월 발행본](https://datatracker.ietf.org/doc/rfc7523/)을 기준으로 번역했습니다. 공개문은 비공식 AI 한국어 번역이며 IETF의 승인·보증을 의미하지 않습니다. [링크가 있는 영문 HTML 표현](https://datatracker.ietf.org/doc/html/rfc7523)도 참고할 수 있습니다.

본문과 표기를 모두 직접 비교해 127개 대응 항목을 확인했습니다. JWT를 authorization grant와 client authentication에 쓰는 두 용도, `assertion`과 `client_assertion`이 각각 필요한 자리, 원래 발행본의 일대일 조건·시간 조건·오류 코드, RS256 구현 의무와 선택적인 replay 보호를 구분했습니다. HTTP·JSON 예제 여섯 개의 글자와 줄바꿈은 원문 그대로입니다. 종이 목차, 발행 정보, 페이지 머리말·꼬리말은 “원문 페이지 표기”에서 확인할 수 있습니다.

1440px·768px·390px에서 한국어판과 원문을 모두 확인했습니다. 좁은 화면에서는 긴 예제만 블록 내부에서 좌우로 스크롤합니다. 출처로 사용한 공식 텍스트 보기의 일부 URL과 URN에는 인쇄 줄바꿈이 그대로 남아 있으므로, 복사하기 전 §8 등록 항목 또는 공식 HTML도 확인하세요.

## 나중에 바뀐 표준

[RFC 10070 §4](https://www.rfc-editor.org/rfc/rfc10070.html#section-4)는 client authentication용 JWT와 authorization grant용 JWT를 구분하여 `aud` 요구사항을 업데이트했습니다. 본문은 2015년의 문구를 유지하고, §3의 별도 안내에 최신 요건을 표시했습니다. 수정된 구현은 해당 공식 표준과 예제를 기준으로 읽으세요.

공개 읽기 화면에는 원본을 바꾸지 않고 §2.1과 §4의 복사용 값, §9.2의 인용판 링크, §4·§5의 RFC 10070 안내, 필요한 예제의 좌우 스크롤 안내를 추가했습니다.
