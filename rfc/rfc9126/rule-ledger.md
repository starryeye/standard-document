# RFC 9126 규범·예외 대조

기준은 [RFC 9126의 2021년 9월 발행본](https://datatracker.ietf.org/doc/html/rfc9126)이다. 아래는 실제 번역판에 남은 규칙과 경계를 요약한 것으로, 구현용 규범 문구는 링크된 공식 문서가 우선한다.

| 위치 | 원문과 번역판에서 확인한 내용 |
| --- | --- |
| §1–1.2 | 인가 데이터를 먼저 직접 보내고, 뒤이어 user agent를 통한 요청에서 참조를 사용한다. PAR는 JAR를 보완한다. BCP 14 키워드의 대문자 조건과 2021년의 문헌 인용을 유지했다. |
| §2 | HTTPS는 필수다. API는 UTF-8 폼을 담은 POST를 받고, 지원 서버에는 PAR URL 메타데이터를 게시하는 것이 권장된다. Request Object 지원 가능성은 선택이다. 2021년 본문에는 issuer URL 권장과 함께 issuer identifier·token endpoint URL·PAR endpoint URL의 수락 의무가 그대로 남아 있다. |
| §2.1 | PAR POST에 `request_uri`를 제공하면 거부한다. 인증 규칙은 token endpoint와 같고, 추가 인증 매개변수는 인증에만 사용한다. 당시 본문의 `client_id` 요구를 보존했다. 조기 수행이 불가능한 검증만 미룰 수 있고, 미룬 검증은 authorization endpoint에서 해야 한다. |
| §2.2 | 성공 응답은 HTTP 201, 최상위 JSON 멤버는 `request_uri`와 `expires_in`이다. 기간은 초 단위 양의 정수이며 5–600초는 예시다. URI에는 암호학적으로 강한 난수 부분이 있어야 하고, 보낸 client에 바인딩되어야 한다. |
| §2.3 | 자동 리디렉션이 금지되고 오류 코드가 정의되지 않는 경우의 기본 `invalid_request`는 선택이다. 사용자 상호작용 오류는 반환하지 않는다. 서명된 Request Object를 요구하는 정책이 적용될 때 비준수 요청에는 400/`invalid_request`를 반환한다. 405는 POST가 아닐 때, 413은 크기 한도를 넘을 때, 429는 기간 내 횟수 한도를 넘을 때다. |
| §2.4·§7.2 | PAR에서 redirect URI 정확 일치의 완화는 인증 자격 증명이 설정된 client에 대한 서버 재량이다. 새 URI를 받아들일 수는 있으나 인증된 client에 한하며, 새 URI만 받아야 한다는 뜻은 아니다. |
| §3 | 폼 본문의 `request` 및 client 인증 매개변수와 JWT에 담는 인가 매개변수를 구분했다. 복호화는 해당하는 경우, 서명 검증은 필수다. 인증된 `client_id`와 JWT의 `client_id`가 다르면 거부하고, `iss`도 일치하도록 요구하는 것은 서버의 재량이다. 원문 첫 문단에 대해 보고된 정오표는 반영하지 않았다. |
| §4 | client의 일회 사용은 의무, 서버의 일회 취급은 권고다. 사용자 새로고침으로 생긴 중복을 허용할 수 있지만 만료된 값은 거부해야 한다. 생략 가능한 검증은 이미 수행한 것에 한하며, 요청과 서버 정책 모두에 결과를 바꿀 변경이 없어야 한다. PAR를 유일한 수단으로 정하는 정책은 전체 또는 client별로 적용할 수 있다. |
| §5–6 | 서버와 client의 `require_pushed_authorization_requests`는 적용 대상이 다르고, 각각 생략 시 기본값은 `false`다. client는 PAR endpoint 메타데이터가 있다는 것만으로 사용 가능 여부를 판단할 수 있으며, 발급된 참조의 사용을 다른 메타데이터가 막지 않는다. |
| §7–8 | §7의 난수·새 redirect URI·일회 사용·client 정책 변경 검증·바꿔치기 대응 권고를 각각 확인했다. §8의 개인정보 보호 개선은 정보가 우발적으로 노출될 가능성을 줄일 수 있다는 설명이며 OAuth 전반의 개인정보 보호 보장이 아니다. |
| §9–10 | IANA 등록 문자열·값·섹션 링크와 규범/참고 문헌의 구분을 보존했다. 발행 당시 초안 번호·날짜는 후속 RFC나 최신 초안으로 바꾸지 않았다. |

§2에서만 별도 편집 안내를 붙였다. [RFC 10070 §5](https://www.rfc-editor.org/rfc/rfc10070.html#section-5)가 갱신한 PAR의 JWT client authentication에서는 authorization server의 issuer identifier URL만 audience로 사용하며, 이를 유일한 값으로 담지 않은 JWT는 거부한다. 2021년 문단 자체는 바꾸지 않았다.
