# Translation QA Review Report

- Status: **PASS**
- Source: ` https://datatracker.ietf.org/doc/html/rfc9068 `
- Screenshots: 2

## Automated required findings

None.

## Warnings

None.

## Preformatted normalization

- Policy: ` prose-reflow-literals-preserved `
- Source SHA256: ` d1bc81c5cdb6f0f76122a62f4c5d9fe4a4232adf1112d0ecfe780003b768c184 `
- Review SHA256 (canonical): ` 7b908c9e7bcaff318957b6f5ecc7f8d61fefd6fa85eadf30711b1c6bf48f03c2 `
- Projection SHA256: ` d79e78f6423ebb730a0976744156aea0a8393f90e7ae243d57db636dc6c0ad52 `
- Translated blocks: 0
- Preserved blocks: 1
- Preserved ` literal-code `: 1
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
| ` zone-001 ` | 1 |
| ` zone-002 ` | 2 |
| ` zone-003 ` | 2 |
| ` zone-004 ` | 2 |
| ` zone-005 ` | 0 |
| ` zone-006 ` | 0 |

### Section findings

- **` zone-001 `**
  - ` boundary_consistency \| pass \| evidence: 목차 §1–§8 및 감사의 글을 본문 제목과 맞췄다. 이어지는 zone-002 첫 항목 저자 연락처가 마지막 목차 링크다. `
  - ` naturalness \| pass \| evidence: 문서의 초록 및 고지 말투를 §1 이하와 일치시키고 메뉴 항목의 동작 의미를 확인했다. `
  - ` protected_content \| pass \| evidence: 104개 결과 검증 통과. 원문 URL/DOM 마커·숫자만 보호 대상으로 유지했다. `
  - ` qualification_preservation \| pass \| evidence: 발행일 유효 규정, 코드 구성요소 추출 시 라이선스 의무, 2021년 10월과 RFC 번호 보존. `
  - ` semantic_fidelity \| pass \| evidence: 문서 표제/발행 메타데이터와 초록의 서버 간 상호운용성 및 고지의 BSD 적용/무보증 내용을 대조했다. `
  - ` terminology \| pass \| evidence: OAuth 2.0, JWT, authorization server, resource server, access token 및 Claim 구분 일치. `
- **` zone-002 `**
  - ` boundary_consistency \| pass \| evidence: 저자 연락처 목차가 앞 구역에 이어지고, 마지막 §2.2.2 첫 문단의 resource owner 속성 설명이 다음 문단의 Claim 직접 요청 미제공과 이어진다. `
  - ` naturalness \| pass \| evidence: 정중체 유지, RS256 문장 및 영문 Claim 조사 수정. 본문과 목차 용어 일치. `
  - ` protected_content \| pass \| evidence: 45개 결과 및 2차 수정 검증 통과. RFC 번호, 규범 마커, Claim 이름/서명 알고리즘과 숫자 보존. `
  - ` qualification_preservation \| pass \| evidence: 서명 필수, 비대칭 권고, none 금지, RS256은 지원 목록에 포함할 의무와 sub 대상이 grant에 따라 달라지는 조건. 인증 값은 같은 응답에서 파생시 변하지 않는다. `
  - ` semantic_fidelity \| pass \| evidence: §1의 포맷 미지정과 RFC7523 목적 차이, §2의 일곱 필수 Claim과 인증 정보 선택 Claim을 원문과 대조했다. `
  - ` terminology \| pass \| evidence: authorization server와 원문이 사용한 authentication server의 역할을 구분했다. 기술용어 JWT, Claim, entitlements, grant, endpoints의 영어를 보존했다. `
- **` zone-003 `**
  - ` boundary_consistency \| pass \| evidence: 앞 §2.2.2 주체 속성 설명을 이어받고, §5.1 토큰 명시 구분 다음의 §5.2 sub 혼동 예방으로 이어진다. `
  - ` naturalness \| pass \| evidence: 요청 설명·캡션·서명 검사 흐름을 자연스럽게 표현하고 §3 첫 문장에서 authorization grant의 범위를 구체적으로 연결했다. `
  - ` protected_content \| pass \| evidence: 36개 결과를 재검증했다. 152/155/159/160/170/173/180/182의 링크·규범 표지 순서를 원문 그대로 복원한 뒤 의미와 조건을 직접 재검토했다. 두 HTTP/JSON 본문 예시는 보호 리터럴이다. `
  - ` qualification_preservation \| pass \| evidence: 형식/iss/aud/서명/exp의 의무, 암호화 사전 협의 후 평문 시 거부 권고, scope에 따라 묶인 기본값의 invalid_scope 권고와 검증 실패 시 invalid_token 필수. 원문 AS/RS 주체 변화는 변경하지 않았다. `
  - ` semantic_fidelity \| pass \| evidence: §2.2.2–§5.1의 발급, resource/scope, 기본 audience, 발견 메타데이터와 resource server의 전체 검증단계, 정확한 오류 코드를 대조했다. `
  - ` terminology \| pass \| evidence: 프로파일·Claim 및 기술 식별어를 앞 구역과 맞추고 ID Token과 access token을 혼동하지 않았다. `
- **` zone-004 `**
  - ` boundary_consistency \| pass \| evidence: §5.1 명시적 구분에서 §5.2 sub 혼동으로 연결된다. 마지막 RFC6838 표제의 서지 설명을 다음 구역이 이어받는다. `
  - ` naturalness \| pass \| evidence: MUST, MUST NOT이 자연스러운 한국어 의무 표현과 함께 배치되며 ‘각 scope와 특정 resource’ 연결을 명확히 했다. `
  - ` protected_content \| pass \| evidence: 97개 결과를 재검증했다. 186/187/200/251/260/269의 링크 계층과 순서를 고쳐 원래 링크와 문구 의미를 대조했고, IANA 값·연락처·참조 번호·서지 정보를 유지했다. `
  - ` qualification_preservation \| pass \| evidence: 모호한 요청에 대한 일반 권고와 자원별 aud 필수, client 내용 검사 금지, 서버 간/동일 자원 내 연결 방지 조건의 서로 다른 정책을 구분했다. `
  - ` semantic_fidelity \| pass \| evidence: §5.2–8.1의 sub 및 audience 구분, 키 분리 한계, 클라이언트 토큰 불투명성과 개인정보 대책, 세 IANA Claim 등록 및 참고문헌을 대조했다. `
  - ` terminology \| pass \| evidence: Claim/프로파일/개인정보 표기와 Roles/Groups/Entitlements 제목을 앞 구역 목차와 맞췄다. `
- **` zone-005 `**
  - ` boundary_consistency \| pass \| evidence: 이전 구역에서 시작한 RFC6838의 서지 설명을 완성하고, 마지막 비교 보기 옵션은 다음 구역의 비교 기준/대상 버전으로 이어진다. `
  - ` naturalness \| pass \| evidence: 이름과 조직을 그대로 보존하면서 감사의 글의 역할과 문장 연결을 한국어로 정리했다. `
  - ` protected_content \| pass \| evidence: 67개 결과 검증 통과. 상세 출처 링크·DOI 및 원문의 중복 인명도 임의로 변경하지 않았다. `
  - ` qualification_preservation \| pass \| evidence: 기존 참고문헌의 표준명·개정판·날짜와 ‘Work in Progress’를 원문대로 둔다. 2019년 워크숍·IIW 28에서의 언급과 두 명의 초기 피드백을 보존했다. `
  - ` semantic_fidelity \| pass \| evidence: 규범적·정보 제공용 참고문헌, 감사의 글과 저자 연락처, 이어지는 Datatracker 메뉴의 내용을 대조했다. `
  - ` terminology \| pass \| evidence: OpenID 및 OAuth 표준·저자·워크숍 고유 이름 유지; 정보 제공용 참고문헌과 감사 제목 목차와 일치. `
- **` zone-006 `**
  - ` boundary_consistency \| pass \| evidence: 앞 구역에서 선택한 비교 방식에 이어 비교 대상 revision이 나오며, 문서 마지막 설정 항목 둘을 모두 확인했다. `
  - ` naturalness \| pass \| evidence: 메뉴·도움말과 레이블의 간결한 문체를 유지했다. `
  - ` protected_content \| pass \| evidence: 30개 결과 검증 통과. 입력/옵션 마커, 버전 00–13 및 모든 링크의 소유 범위 불변. `
  - ` qualification_preservation \| pass \| evidence: 인라인 페이지는 네트워크 불필요, 외부 참조 페이지는 표시 시 네트워크 필요, 링크 이동 대상 두 가지를 구분했다. `
  - ` semantic_fidelity \| pass \| evidence: 비교 기준과 대상 옵션, 연락처, 사이드바·문서 형식·참조 링크의 동작을 한 항목씩 대조했다. `
  - ` terminology \| pass \| evidence: Datatracker·RFC·HTML·문서 ID 및 날짜/번호는 원문대로 두었다. `
