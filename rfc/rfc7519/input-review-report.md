# Translation QA Review Report

- Status: **PASS**
- Source: ` https://datatracker.ietf.org/doc/rfc7519/ `
- Screenshots: 2

## Automated required findings

None.

## Warnings

None.

## Preformatted normalization

- Policy: ` prose-reflow-literals-preserved `
- Source SHA256: ` 11c1fec1dbaf27a05cace76b79f9eb759b7864ff9fbe50c3720d4de1044a01ad `
- Review SHA256 (canonical): ` 278997a29c22ceb7ef6e74a9f2c1d0caa2c96341279e4740e0434c05f61bf71d `
- Projection SHA256: ` d757a2e54a27e10238ffd3970eff8ad90a407898e7fabb183d10989992e1fa44 `
- Translated blocks: 271
- Preserved blocks: 416
- Preserved ` blank `: 302
- Preserved ` literal-code `: 20
- Preserved ` literal-layout `: 68
- Preserved ` literal-table `: 26
- Generated critical asset: ` assets/wt-preformatted-14edac915a1f0158.css ` SHA256 ` 14edac915a1f01585baf87d8c22fec54e261a42cf370c2e5afe244b1f9b07072 `

## Browser evidence

| Viewport | Horizontal overflow | Broken images | Clipped text |
| --- | ---: | ---: | ---: |
| ` desktop-1440x900 ` | false | 0 | 0 |
| ` narrow-390x844 ` | false | 0 | 0 |

## Master semantic review

### Unresolved required items

None.

### Translation retries

| Zone | Retries |
| --- | ---: |
| ` zone-001 ` | 2 |
| ` zone-002 ` | 1 |
| ` zone-003 ` | 0 |
| ` zone-004 ` | 1 |
| ` zone-005 ` | 1 |

### Section findings

- **` zone-001 `**
  - ` boundary_consistency \| pass \| evidence: §1의 JWT 발음 설명에서 다음 구역의 표기법으로 자연스럽게 이어진다. `
  - ` naturalness \| pass \| evidence: 사이트 메뉴와 발행 정보의 의미를 확인하고 이메일 수신자 목록·발행 월 표기를 수정했다. `
  - ` protected_content \| pass \| evidence: 139개 ID와 보호 마커를 재검증했다. seg-000135의 법적 고지 URL 뒤에는 조사를 붙이지 않고 원문 주소를 정확히 보존했다. `
  - ` qualification_preservation \| pass \| evidence: 서명·암호화의 and/or, 날짜와 라이선스 범위를 그대로 유지했다. `
  - ` semantic_fidelity \| pass \| evidence: §1 JWT가 JWS 페이로드 또는 JWE 평문으로 쓰인다는 구분, 서명/MAC과 암호화의 관계, 발행 시점 BCP 78 및 코드 라이선스의 범위를 대조했다. `
  - ` terminology \| pass \| evidence: JWT, JWS, JWE, Claim 및 Compact Serialization의 원래 기술 명칭을 유지했다. `
- **` zone-002 `**
  - ` boundary_consistency \| pass \| evidence: §1 다음의 표기법부터 jti 제목까지 이어지며 다음 구역은 jti 본문으로 시작한다. `
  - ` naturalness \| pass \| evidence: 용어 정의와 시간 조건은 한국어로 풀고 예제 설명과 구분했다. `
  - ` protected_content \| pass \| evidence: 52개 대상 및 보호 마커 검증을 통과했다. JSON·JWT·바이트 예시는 번역 대상 밖의 원문 리터럴이다. `
  - ` qualification_preservation \| pass \| evidence: exp는 지정 시각 미만, nbf는 지정 시각 이상이며 유예 시간은 선택 사항이다. aud의 단일 문자열 예외도 남았다. `
  - ` semantic_fidelity \| pass \| evidence: §2–4.1에서 StringOrURI의 콜론 조건, NumericDate의 윤초 제외/실수 가능성, 중복 Claim 처리 두 선택지와 aud 불일치 거부를 대조했다. `
  - ` terminology \| pass \| evidence: Claim Name 세 분류의 명칭을 인접 구역과 맞췄다. `
- **` zone-003 `**
  - ` boundary_consistency \| pass \| evidence: 이전 구역의 jti 제목에 이어 본문을 열고, §7.3의 예외는 다음 구역에서 이어진다. Public/Claim Names는 원문 페이지 경계에서 분리되어 있다. `
  - ` naturalness \| pass \| evidence: 번호가 붙은 검증 절차 및 JWS/JWE 하위 사례를 구별한다. `
  - ` protected_content \| pass \| evidence: 57개 대상·보호 마커가 유효하다. §7.2는 정오표와 구분하여 발행 판본대로 번역했다. `
  - ` qualification_preservation \| pass \| evidence: typ/cty의 선택성과 Nested JWT에서 cty가 JWT여야 하는 요구, 외부 보호 수단과 Unsecured JWT의 관계, 검증 단계의 실패 조건을 유지했다. `
  - ` semantic_fidelity \| pass \| evidence: §4.1.7–7.3의 발급자별 jti 충돌 방지, JOSE 헤더와 복제 Claim의 조건, 생성·검증 절차를 발행 원문과 대조했다. `
  - ` terminology \| pass \| evidence: JOSE Header, Nested JWT, Public/Private Claim Names를 구역 간 동일하게 사용했다. `
- **` zone-004 `**
  - ` boundary_consistency \| pass \| evidence: §7.3의 DNS 대소문자 예외를 이어받고, §11.2는 다음 구역의 그 결과를 암호화한다는 말로 연결된다. `
  - ` naturalness \| pass \| evidence: 추가 등록 정보 내 세 필드가 붙어 보이지 않게 구분했다. `
  - ` protected_content \| pass \| evidence: 105개 대상·보호 마커와 등록 참조 문서 형식이 유효하다. `
  - ` qualification_preservation \| pass \| evidence: 3주와 21일, 8자 권고 및 대소문자 예외의 충분히 설득력 있는 사유, 외부 적용 맥락에 따른 검증 제약을 유지했다. `
  - ` semantic_fidelity \| pass \| evidence: §8–11에서 구현 필수와 사용 여부, JWE 선택과 조건부 요구, IANA 등록 절차·필드, 발급자에 대한 키 결합 및 검증 조건을 대조했다. `
  - ` terminology \| pass \| evidence: nbf의 등록 설명은 §4.1.5와 일관된 처리 개시 시각으로, JWS/JWE 구별과 Designated Expert 명칭을 유지했다. `
- **` zone-005 `**
  - ` boundary_consistency \| pass \| evidence: §11.2 앞 구역의 서명한 메시지를 암호화한다는 문장을 완성하고, 참고문헌·부록·감사·저자 연락처 순서를 유지했다. `
  - ` naturalness \| pass \| evidence: 서명자의 privacy를 프라이버시로 구별하고, SAML 비교에서 작은 크기를 자연스럽게 표현했다. `
  - ` protected_content \| pass \| evidence: 58개 대상·보호 마커 검증 통과. 458 옥텟, 알고리즘 이름, 예제 및 저자 이름을 보존했다. `
  - ` qualification_preservation \| pass \| evidence: 서명 선행을 절대 규칙으로 바꾸지 않고, §12의 공개 방지 요구 및 수신자·엔드포인트 인증 조건을 보존했다. `
  - ` semantic_fidelity \| pass \| evidence: §11.2–부록 C까지 서명 선행의 일반적 관행과 이유, 사생활 관련 조치, 두 암호화 예제, SAML과 SWT의 관계를 대조했다. `
  - ` terminology \| pass \| evidence: Content Encryption Key, JWE Ciphertext, SAML Assertion, SWT 및 규격 참조를 일관되게 유지했다. `
