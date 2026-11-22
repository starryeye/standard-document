# 규정과 경계 사례 대응표 — RFC 10070 (2026년 11월)

절 번호는 IETF 원문과 한국어 읽기판에 공통이다. OLD는 과거 규칙 인용이고, NEW와 추가 규칙은 이번 발행본이다. 아래 한국어는 짧은 확인용 발췌 또는 해당 문장의 요지이며 정확한 쌍과 앵커는 실제 DOM 대응표에 있다. `equal`은 규정의 적용 범위·강도·경계가 같다는 뜻이다.

| 위치 | 원문 규칙: 주체, 동작, 강도와 조건 | 한국어판 규칙 및 경계 사례 | 판정 |
|---|---|---|---|
| 초록, §1 | JWT 토큰인 경우 의도된 수신자 값은 `aud`; RFC 8414 §3.3은 메타데이터를 가져온 client에게 반환된 issuer의 검증을 요구한다. client 인증용 JWT에는 단 하나의 audience로 issuer identifier를 요구하며 서버가 다른 것을 거부한다. | metadata를 가져오지 않은 actor로 확대하지 않는다. 다른 endpoint 메타데이터 값의 직접 검증 불가와 공격 가능성을 별개로 설명한다. 서론의 단일값 범위는 JWT client 인증이며 grant에 일반화하지 않는다. | equal |
| §1.1–1.2 | BCP 14의 대문자 키워드는 전부 대문자일 때에만 규범적 의미로 해석. 용어 정의의 출처는 RFC 6749·7521·7519. | 대문자 `MAY`에는 적용하고 본문의 일반 소문자 *may*에는 적용하지 않는다. 세 정의 출처를 모두 보존한다. | equal |
| §2 OLD | assertion의 하나 이상 예정 처리자를 식별. RFC 6749 token endpoint URL 사용 가능; 별도 application profile이 없으면 준수 앱이 Simple String Comparison을 사용해야 한다. | 하나와 복수 모두 해당; 다른 비교법을 정한 프로파일이 있는 경우 기존 문자열 비교 의무를 일률 적용하지 않는다. | equal |
| §2 NEW | 예정된 처리자를 식별. RFC 8414 issuer identifier로 해당 서버를 유효한 audience로 표시할 수 있다. | 과거의 다중 수신자 표현과 token endpoint 설명을 이 정의에 넣지 않았고, 해당 issuer identifier 사용은 가능 표현을 유지한다. | equal |
| §3 OLD 1 | client 인증 SAML `client_assertion_type` 값 고정, `client_assertion` SAML 2.0 Assertion 정확히 하나, RFC 4648 §5 base64url과 zero padding bits 의무; 인코딩 데이터 줄바꿈과 실제 pad 문자 둘 다 비권고. | 두 assertion은 불가, 값 하나는 개수 조건 충족; 0 padding bits와 뒤에 붙는 `=` 문자는 같은 요구가 아니다. 줄바꿈·pad 문자에 MUST NOT을 추가하지 않는다. HTTP 예제의 추가 줄바꿈은 표시용이다. | equal |
| §3 NEW 1 | 모든 새 애플리케이션은 SAML Bearer Assertion을 client 인증에 사용하면 안 됨. 기존에 인용 방식으로 사용하는 앱의 이전·audience 강화는 구현·배포자 판단. | 신규 구현에는 금지, 이미 같은 방식으로 운영하던 앱에는 이전과 강화 중 하나/둘 다의 재량이 남음. SAML grant 전체를 금지하지 않는다. | equal |
| §3 OLD 2 | SAML XML 세 계층 필수, token endpoint URL은 추가 허용, 자기 identity가 없는 assertion은 서버가 거부, 예외 프로파일이 없으면 Simple String Comparison, 정확한 문자열은 서버와 issuer가 out of band에서 설정. | XML 요소 이름·중첩 유지. 프로파일이 다른 비교법을 정하는 경우 예외를 살렸고, URL이 값을 가리키는지와 문자열의 사전 설정을 분리했다. | equal |
| §3 NEW 2 | 동일 XML 세 계층, client가 대상 적합성 책임. 서버 issuer identifier, token endpoint URL, SAML Entity ID 중 적합한 것은 허용; 서버 자체 identity가 의도된 audience에 없으면 거부 의무. | 수신 서버에 적합한 SAML Entity ID를 선택할 수 있다. 다른 서버의 Entity ID만 넣으면 거부한다. JWT client 인증과 달리 issuer identifier 유일 조건을 새로 붙이지 않는다. | equal |
| §4 OLD | JWT `aud` 포함 의무, token endpoint URL 사용 가능, 자기 identity가 없으면 거부; 별도 프로파일 없으면 단순 문자열 비교, issuer와 서버가 정확한 문자열을 out of band에서 설정. | token endpoint 허용은 OLD에만 남아 있으며, 별도 프로파일 예외와 거부 주체·정확한 문자열을 설정하는 두 당사자가 같다. | equal |
| §4 NEW 공통과 A | `aud`가 의도된 서버를 식별해야 한다. authorization grant에서 client가 수신 서버에 맞는 값을 보장할 책임, 서버 issuer identifier 또는 token endpoint URL 사용 가능. | 적합한 token endpoint URL은 JWT grant에서는 허용된다. 이를 JWT client 인증에서도 허용한다고 읽히지 않도록 A/B 구분을 유지한다. | equal |
| §4 NEW B | client 인증의 JWT는 해당 authorization server의 issuer identifier만; 서버에 issuer identifier 의무; endpoint URL을 audience로 사용 금지; sole value가 아니면 서버가 거부. | issuer만 있는 경우 이 요건 충족, 발급자와 다른 값을 함께 넣거나 token endpoint만 넣으면 실패. 배열과 JSON 문자열 표현에 대한 추가 제약은 번역에 추가하지 않는다. | equal |
| §4 NEW 비교 | 달리 규정하는 application profile이 없을 때만 RFC 3986 §6.2.1 Simple String Comparison 의무. | URL을 마음대로 정규화하도록 허용하지 않는다. 다르게 명시한 application profile의 예외를 양쪽에서 확인했다. | equal |
| §4 추가 타이핑 | client 인증 JWT에는 `typ`으로 `client-authentication+jwt` 또는 프로파일 명세의 더 구체적 explicit type 권고. 강화된 audience가 주된 보호; 명시적 타입이 없는 JWT를 그것만으로 거부하는 것은 NOT RECOMMENDED. | 올바른 audience와 타입 없음은 타입 누락만으로 거부 비권고. 올바른 타입과 틀린 audience는 위 규칙대로 거부한다. 더 구체적인 값은 프로파일이 정해야 한다. | equal |
| §4 예제·§4.1와 합의 | OLD와 NEW의 grant audience·claim set 교체. client 인증 JWT에서는 audience identifier의 별도 합의 불필요. 예제의 JWT를 발급/서명한 client 및 audience는 token endpoint 주소와 다르며 HTTP 블록 줄바꿈은 예시 표시용. | OLD와 NEW JSON, 발급자·token endpoint 주소·`ES256`과 key ID `16`은 보존. 사전 합의 제거가 grant까지 적용된다고 추가하지 않았다. 예제는 예제이고 배포 값에 대한 규범이 아니다. | equal |
| §5 PAR OLD | issuer URL 사용 SHOULD; receiver가 issuer identifier, token endpoint 또는 PAR endpoint URL 모두 자기 audience로 수락해야 한다. | 구 규칙에서 적합한 PAR endpoint URL 입력은 수락 의무가 있었다. 이를 NEW로 오인하지 않도록 별도의 OLD 인용으로 유지했다. | equal |
| §5 PAR NEW | RFC 8414 issuer URL만을 audience로 사용 MUST, 다른 경우 서버 거부 MUST. 동일한 `typ` SHOULD와 거부 비권고. | PAR endpoint URL만 혹은 issuer+추가 값은 수락하지 않는다. 타입 하나로 audience 위반을 덮을 수 없으며 §4와 동일하게 처리한다. | equal |
| §6 | 새 client는 이전 및 새 서버와 상호운용; 일부 이전 client는 엄격한 새 서버와 호환되지 않을 수 있음. 계획에 비대칭을 고려하고 필요하면 client 먼저 또는 서버와 조율하여 갱신. | 어떤 이전 client도 항상 실패한다고 하지 않는다. 서버 우선이라는 새 권고를 만들지 않는다. 소문자 should의 운영상 고려와 BCP 14 의무를 구분한다. | equal |
| §7 | 인용한 여섯 명세의 고려 사항 모두 적용. 이전 audience의 모호함에서 가능한 문제를 막기 위해 검사를 강화. | 인용한 여섯 명세 모두 유지. 타입 지정만으로 문제가 해결된다는 주장을 더하지 않는다. | equal |
| §8.1.1 | application 하위 타입 client-authentication+jwt. base64url 값들이 점으로 구분되며 값의 일부는 빈 문자열 가능; 필수/선택 parameter 등은 N/A; 용도 COMMON, 제한 없음, 가등록이 아님. | 연속된 점 사이의 빈 값이 가능하다는 원문 등록 문구를 막지 않는다. N/A·COMMON·IETF 및 §4·§7 참조가 일치한다. | equal |
| §8.2–8.3 | 두 인증 방식 private_key_jwt/client_secret_jwt의 change controller는 IESG, OpenID.Core §9·RFC 10070 참조; 4개의 OAuth URI에 RFC 10070이 추가 참고. | 2가지 방식과 JWT/SAML × grant/client assertion 4개 등록값을 그대로 둔다. 등록 참조 추가를 값 자체의 변경으로 옮기지 않는다. | equal |
