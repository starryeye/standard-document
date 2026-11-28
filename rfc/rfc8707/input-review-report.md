# Translation QA Review Report

- Status: **PASS**
- Source: ` https://datatracker.ietf.org/doc/html/rfc8707 `
- Screenshots: 2

## Automated required findings

None.

## Warnings

None.

## Preformatted normalization

- Policy: ` prose-reflow-literals-preserved `
- Source SHA256: ` 451bbdc900ca3be74604c98ec8d71e36bd9ffec44d47400229e1a3d9930e6783 `
- Review SHA256 (canonical): ` c240b0bd17b0d1d052b7e516b2149117476056096c327f5978c29efa0b84c863 `
- Projection SHA256: ` 03b74cdbd05a2757a594832f0ddcbe2d51988c8ea6c44b96c198a1b861059fcc `
- Translated blocks: 0
- Preserved blocks: 6
- Preserved ` literal-code `: 6
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
| ` zone-001 ` | 0 |
| ` zone-002 ` | 1 |
| ` zone-003 ` | 1 |
| ` zone-004 ` | 0 |

### Section findings

- **` zone-001 `**
  - ` boundary_consistency \| pass \| evidence: TOC seg-000080..095 leads to matching article section labels; §1's initial deployment/scope problem at seg-000097 agrees with the protected-resource explanation in seg-000098. Shared sidebar controls align with zone-004. `
  - ` naturalness \| pass \| evidence: Direct English–Korean read of seg-000001..097: interface labels are concise; closing front matter and opening body use formal plain Korean consistently. The introduction splits a long qualifier into its own sentence without dropping it. `
  - ` protected_content \| pass \| evidence: Independent zone validator passed all 97 IDs and protected markers. Both version selectors retain drafts 00–08, normative/reference links, publication numbers, three abbreviated author names and exact email attributes. `
  - ` qualification_preservation \| pass \| evidence: seg-000073 distinguishes consensus, public review and IESG publication approval; seg-000077 states effective-at-publication and retains license/warranty scope; seg-000097 preserves the limitation to some circumstances. `
  - ` semantic_fidelity \| pass \| evidence: seg-000070 retains that the request parameter is an extension to identify the protected resource(s), not an authentication mechanism; seg-000072..077 retain RFC status, links, publication authority and IETF Trust notice. seg-000097 links the need to an applicable deployment example. `
  - ` terminology \| pass \| evidence: Resource Indicators is OAuth 2.0 리소스 식별자 in title and UI; authorization is 인가, not 인증; the first use of authorization server, client and access token is English-first. `
- **` zone-002 `**
  - ` boundary_consistency \| pass \| evidence: The §1 opening completes the zone-001 deployment example. §2.1's code/grant discussion and Figure 2 lead naturally to §2.2 in zone-003. Header labels match the source-layout TOC. `
  - ` naturalness \| pass \| evidence: Read all 28 aligned source/target segments. Clarified query context and placement of the base-URI recommendation in retry 1; protection markers remain in order while surrounding Korean clauses are complete. `
  - ` protected_content \| pass \| evidence: The per-zone validator passed before and after the one retry; BCP 14 markers, RFC numbers, example URIs, resource/aud/error literals and Figure 1–2 references were also directly checked. `
  - ` qualification_preservation \| pass \| evidence: seg-000103 retains all-uppercase-only interpretation; seg-000109 separates absolute URI obligation, fragment prohibition, query recommendation and exceptions; seg-000111 preserves the non-mandatory base URI recommendation; seg-000119..120 distinguish optional default/rejection, conditions and non-BCP-14 lowercase should. `
  - ` semantic_fidelity \| pass \| evidence: seg-000098..101 explain token construction and scope versus destination. seg-000109 correctly places query parameters within the scope of requests made to an application; seg-000115 distinguishes resource identifiers from audience encodings; seg-000117 distinguishes the whole grant from access-token-only use. `
  - ` terminology \| pass \| evidence: Preserved English OAuth nouns, including scope and audience, and distinct resource, authorization grant and authorization code. Aliases in §1.2, SCIM and JWT-SAR remain referentially accurate. `
- **` zone-003 `**
  - ` boundary_consistency \| pass \| evidence: §2.2 follows the approved Figure 2 case, shows calendar after authorization code then contacts after refresh token, and matches Figure 3–6 captions. The closing Acknowledgements heading leads directly to zone-004's credits. `
  - ` naturalness \| pass \| evidence: Read all 63 aligned rows; grant/access/refresh contrast flows across sentences. In the sole retry aligned scope terminology in 128 and clarified grant usage in the IANA registry label in 158. `
  - ` protected_content \| pass \| evidence: Per-zone validation passed, examples' immutable preformatted input stays outside translation, Figure 3–6 links and captions match, and ten bibliography entries preserve source names, RFC labels, dates, DOI and URLs. `
  - ` qualification_preservation \| pass \| evidence: Preserved for-all-grant-types in seg-000126, own-discretion policy and conditional returns in 127, possible downscope and must-return-actual-scope-if-different in 128, non-normative single-resource encouragement in 138, whenever feasible and client responsibility in 139, and possible tracking in 141. `
  - ` semantic_fidelity \| pass \| evidence: seg-000126..129,132 retain per-grant-type requested target, server discretion, requested subset versus any refresh token under the full grant, cartesian product, and downscoping; seg-000136..141 preserve audience, tenant isolation, abstract identifier validation and privacy without strengthening claims. `
  - ` terminology \| pass \| evidence: Kept English access token, refresh token, authorization grant, scope, audience and token introspection consistent with pages and zone-002. IANA OAuth Parameters and OAuth Extensions Error Registry names and exact registry values retain their identity. `
- **` zone-004 `**
  - ` boundary_consistency \| pass \| evidence: seg-000189 follows Acknowledgements and seg-000191 matches TOC. Mirrored sidebar dates, versions, authors, comparison selections and errata labels retain the same translations as zone-001. `
  - ` naturalness \| pass \| evidence: Read all 73 paired rows. Acknowledgments are split into readable Korean without changing the people or attribution. Compact labels and tooltip sentences fit their purposes. `
  - ` protected_content \| pass \| evidence: Zone validator passed. Compared the contributor list, all three author organizations/emails, mirrored draft versions 00–08, IETF alt text, mailto and other protected links/labels. `
  - ` qualification_preservation \| pass \| evidence: Preserved attribution and assistance rather than authorship in the credits; UI text keeps conditions (offline availability versus connection required) and alternate citation destinations. `
  - ` semantic_fidelity \| pass \| evidence: seg-000189..203 differentiate both chairs, three Security Area Directors, individual contributors and published bylines. seg-000253..261 distinguish HTML/plain text conversion, offline embedding and different citation link behaviors. `
  - ` terminology \| pass \| evidence: OAuth 작업반, 제안 표준, Datatracker, other UI terms and identifiers agree with zone-001; organization and author names remain exact. `
