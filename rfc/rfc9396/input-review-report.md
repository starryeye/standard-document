# Translation QA Review Report

- Status: **PASS**
- Source: ` https://datatracker.ietf.org/doc/html/rfc9396 `
- Screenshots: 2

## Automated required findings

None.

## Warnings

None.

## Preformatted normalization

- Policy: ` prose-reflow-literals-preserved `
- Source SHA256: ` 86dd1023d3957c878c155a1d12a4bb4911c139c2f2f7551823c5e92713550f15 `
- Review SHA256 (canonical): ` 6b879f3ca49dc28b7985421adf9868a95c1184b0ee0905efa798a2ea0dc0001b `
- Projection SHA256: ` 628b9f8fefe867a078fd2aee0e10a641df7c85829e7bae054ee53983eed9e3f4 `
- Translated blocks: 0
- Preserved blocks: 30
- Preserved ` literal-code `: 30
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
| ` zone-002 ` | 1 |
| ` zone-003 ` | 1 |
| ` zone-004 ` | 1 |
| ` zone-005 ` | 1 |
| ` zone-006 ` | 1 |
| ` zone-007 ` | 1 |
| ` zone-008 ` | 0 |

### Section findings

- **` zone-001 `**
  - ` boundary_consistency \| pass \| evidence: No preceding content. Document title, abstract and status opening seg-000085/086 lead into seg-000087's IETF consensus and review statement; title and duplicate sidebar labels agree. `
  - ` naturalness \| pass \| evidence: Korean controls distinguish 나란히 보기/인라인 보기 after retry. Article front matter and abstract use formal plain declarative endings; titles and dates read naturally. `
  - ` protected_content \| pass \| evidence: After retry, all 86 target IDs and exact placeholder sequences checked; both revision selectors retain RFC and all 24 draft choices in source order, along with author links, format labels and fixed numeric values. `
  - ` qualification_preservation \| pass \| evidence: The abstract states what the document specifies, with no added implementation mandate. Proposed Standard and Standards Track are kept as distinct source classifications. `
  - ` semantic_fidelity \| pass \| evidence: seg-000001..086: Verified official title, revision UI, author affiliations, May 2023, standards-track class and abstract. The abstract still identifies the exact OAuth parameter and its purpose as carrying fine-grained authorization data. `
  - ` terminology \| pass \| evidence: Exact RFC 9396, OAuth 2.0, OAuth-RAR, agencies, names, organization names and ISSN retained; '인가' used for authorization in title and abstract. `
- **` zone-002 `**
  - ` boundary_consistency \| pass \| evidence: Seg-000085/086 status into 087 and 165/166 common-field definition into 167/168 agree with neighbors. TOC labels agree with corresponding translated body headings. `
  - ` naturalness \| pass \| evidence: Formal plain declarative prose; examples read as user requests without changing their scope. Aligned four TOC names with actual body headings after review. `
  - ` protected_content \| pass \| evidence: All 80 IDs and ordered placeholders checked after retry, including exact BCP 14 keywords and reference anchors, type identifiers, numbered TOC and 45 Euros amount. `
  - ` qualification_preservation \| pass \| evidence: Preserved all-caps-only BCP 14 condition, REQUIRED type, MAY repeat type, RECOMMENDED copyable and collision-resistant values, and the fact that common fields are reusable but not mandatory. `
  - ` semantic_fidelity \| pass \| evidence: seg-000087..166: Consensus, approval, copyright, RFC links, examples motivating fine-grained data, type-specific fields and AS/RS enforcement responsibilities correspond to source. In seg-000165, the applicable protected API defines allowed values. `
  - ` terminology \| pass \| evidence: Kept exact named RFC terms in seg-000147, AS/RS and client/account identifiers; distinct translatable phrase 상세 인가 정보 is not substituted for the wire parameter. `
- **` zone-003 `**
  - ` boundary_consistency \| pass \| evidence: Seg-000166 term is followed immediately by its 167 definition. Seg-000228 issues reduced-rights token if checks pass; seg-000229/230 constrain example to its API and move to write/read example without treating the comparison as universal. `
  - ` naturalness \| pass \| evidence: Reviewed natural formal declarative prose across definition and protocol steps after retry, kept caption ending 예시 and clear readable wording for the two examples. `
  - ` protected_content \| pass \| evidence: All 62 IDs and ordered placeholders checked after retry, including application/x-www-form-urlencoded, type/data fields, grant identifiers, invalid_authorization_details and numerous section references. `
  - ` qualification_preservation \| pass \| evidence: Preserved independent requirements carried together, AS duties to combine and present merged consent, either error condition with both mandatory abort and response, lowercase should on object comparison, and that reducing a token leaves prior authorization intact. `
  - ` semantic_fidelity \| pass \| evidence: seg-000167..228: Verified common-field Cartesian product vs multiple independent objects, scope/resource processing, absence of authorization-response additions, error and token-request decisions, and field-specific comparison. Corrected the data owners and read/write mappings. `
  - ` terminology \| pass \| evidence: AS/RS, client, resource owner, access token and grant type remain English; exact code forms separated from descriptive Korean 상세 인가 정보. `
- **` zone-004 `**
  - ` boundary_consistency \| pass \| evidence: Seg-000228 success flows into qualifications in 229; seg-000300 ends basic-function list with token availability and seg-000301 moves to customizable representation without changing their force. `
  - ` naturalness \| pass \| evidence: Reviewed formal flow from comparison examples into token response and onward. Rephrased optionality and required return naturally in retry; preserved source vs requested token wording. `
  - ` protected_content \| pass \| evidence: All 72 IDs and ordered placeholders checked after retry; JWT, introspection, registration parameter names, exact cross-references and source example links intact. `
  - ` qualification_preservation \| pass \| evidence: Seg-000240 keeps mandatory output of granted/assigned details, seg-000242 permits omitting some values, seg-000246 distinguishes enrichment permission from the type-definition requirement. Seg-000260/274 keep mandatory AS availability and conditional introspection fields separate from optional transport or filtering. `
  - ` semantic_fidelity \| pass \| evidence: seg-000229..300: Verified API-specific read/write/admin subsumption, audience restriction, return and discretionary assignment, example enrichment, RS data access via JWT/introspection and two metadata flows. `
  - ` terminology \| pass \| evidence: Kept technical actor and claim/metadata terms, as well as recurring 지급 개시 example. Figure 23 retains the source caption's server metadata wording even though context discusses client registration. `
- **` zone-005 `**
  - ` boundary_consistency \| pass \| evidence: Seg-000300 basic production of token/introspection data flows into seg-000301 presentation customization, and seg-000398 starts RFC 8628 citation continued in seg-000399. `
  - ` naturalness \| pass \| evidence: Reviewed formal declarative prose and natural particles after protocol identifiers. No confusion between exact field names and explanatory text; labels remain concise. `
  - ` protected_content \| pass \| evidence: All 98 IDs and ordered placeholders rechecked; signed request object references, metadata and error identifiers, RFCs and DOI strings retained. `
  - ` qualification_preservation \| pass \| evidence: Preserved lower-case advice vs conditional MUST in security, no extra string transformation, prevention of sensitive data disclosure, distinction between end-to-end transport and app-level encryption, and AS local need-to-know policy. `
  - ` semantic_fidelity \| pass \| evidence: seg-000301..398: Verified optional type schema, no dereference assumption, PAR and request URI interplay, protection and comparison rules, privacy sharing, IANA entries and opening citations. `
  - ` terminology \| pass \| evidence: Consistent token endpoint and authorization endpoint, request object, OpenID-related document names, client/AS/RS and exact IANA names; OAuth Dynamic Client Registration heading matches TOC. `
- **` zone-006 `**
  - ` boundary_consistency \| pass \| evidence: Seg-000398/399 finish one bibliographic entry; seg-000487 감사드린다 passes into 488's additional thanks then 489 author contacts. `
  - ` naturalness \| pass \| evidence: Appendix prose now uses the same plain formal style as the rest; revised code particles and signature-algorithm parenthetical. Native definition and figure language is clear. `
  - ` protected_content \| pass \| evidence: All 89 IDs and exact placeholder order checked after retry; data field names, numbers, protected reference links and dates retained. `
  - ` qualification_preservation \| pass \| evidence: OpenID examples are hypothetical and out of scope for defining a type; claims delivery is distinguished from obtaining claims with access token; EHR-only information must be presented, lawful-basis check and conditional example details retain their qualifications. `
  - ` semantic_fidelity \| pass \| evidence: seg-000399..487: Verified complete remaining bibliography, illustrative OpenID Connect types, electronic-signing bindings, tax/access duration and eHealth roles, consent and audit purposes. Requester remains distinct from patient. `
  - ` terminology \| pass \| evidence: References retain their original bibliographic titles/DOIs, and body uses client, access token, ID Token, userinfo endpoint, EHR and OID consistently. `
- **` zone-007 `**
  - ` boundary_consistency \| pass \| evidence: Seg-000487 first list leads into 488's additive thanks; 563/564 contents/HTML conversion labels lead into zone-008 options with same vocabulary. `
  - ` naturalness \| pass \| evidence: Formal article thanks matches preceding paragraph; compact UI labels are clear and remain consistent across main/widened and narrow sidebar copies after retry. `
  - ` protected_content \| pass \| evidence: All 77 IDs and ordered placeholders checked after retry, including exact author link targets, RFC draft names and compared revision choices. `
  - ` qualification_preservation \| pass \| evidence: No added or removed substantive requirement or qualification. Toggles keep default vs selected state and status remains Proposed Standard. `
  - ` semantic_fidelity \| pass \| evidence: seg-000488..564: Acknowledgment, author names/organizations/email routing and full duplicated Datatracker metadata, version selection and preference labels retain their respective functions. `
  - ` terminology \| pass \| evidence: Names, address labels' associated literals, RFC/working group names and HTML/Datatracker product words preserved consistently. `
- **` zone-008 `**
  - ` boundary_consistency \| pass \| evidence: Seg-000563/564 end previous settings zone, and seg-000565/566 expand HTML transformation without a dangling referent. No following segment. `
  - ` naturalness \| pass \| evidence: Short button labels and descriptive Korean attribute text correspond without duplication or ambiguity; mobile preference context is clear. `
  - ` protected_content \| pass \| evidence: All 9 immutable IDs and exact placeholder order validated, including protected settings markup/attributes. `
  - ` qualification_preservation \| pass \| evidence: Network-independent larger pages are distinguished from network-required regular pages; no extra implementation claim or changed constraints. `
  - ` semantic_fidelity \| pass \| evidence: seg-000565..573: Both conversion directions, font-size option, inline or referenced resource choices and two citation-link destinations match their stated functions. `
  - ` terminology \| pass \| evidence: HTML and resource/reference vocabulary consistent with neighboring settings; actual values, conversion directions and links unchanged. `
