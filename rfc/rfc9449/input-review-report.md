# Translation QA Review Report

- Status: **PASS**
- Source: ` https://datatracker.ietf.org/doc/html/rfc9449 `
- Screenshots: 2

## Automated required findings

None.

## Warnings

None.

## Preformatted normalization

- Policy: ` prose-reflow-literals-preserved `
- Source SHA256: ` 4df872c8cd5491e7cd45557a6d22414908df2e63c416e4bdae095c6e44b99c12 `
- Review SHA256 (canonical): ` 35d5c25951dfd571db7f998a423c2753b81fdcad36593627420ec5db27b40ed5 `
- Projection SHA256: ` a19af38d13a545f0ed7f8a256a09ee48a5abbcf3affd5c425c4847bc35468642 `
- Translated blocks: 0
- Preserved blocks: 25
- Preserved ` literal-code `: 24
- Preserved ` literal-diagram `: 1
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
| ` zone-003 ` | 0 |
| ` zone-004 ` | 0 |
| ` zone-005 ` | 1 |
| ` zone-006 ` | 0 |
| ` zone-007 ` | 1 |
| ` zone-008 ` | 1 |
| ` zone-009 ` | 0 |
| ` zone-010 ` | 1 |
| ` zone-011 ` | 0 |

### Section findings

- **` zone-001 `**
  - ` boundary_consistency \| pass \| evidence: No preceding neighbor. Copyright reservation at 90 continues immediately into applicable legal terms at 91. `
  - ` naturalness \| pass \| evidence: Natural Korean status and concise UI labels; article starts with a declarative technical abstract. `
  - ` protected_content \| pass \| evidence: Validated IDs, exact tokens, locations and DOM shape, including URLs, emails, numbers and version selectors. `
  - ` qualification_preservation \| pass \| evidence: 00–16 and September 2023 are exact; the abstract does not claim all replay is prevented. `
  - ` semantic_fidelity \| pass \| evidence: Datatracker sidebars and duplicate tooltips, author/ISSN/print metadata, title, abstract, status and reservation checked; proof detects replay for both token types. `
  - ` terminology \| pass \| evidence: English-first DPoP, proof of possession, sender-constrained and token terms, with exact author and standards identifiers. `
- **` zone-002 `**
  - ` boundary_consistency \| pass \| evidence: Follows rights reservation at 90; 161 sender constraint leads to browser/XSS section at 162. `
  - ` naturalness \| pass \| evidence: Removed redundant title exposition, and exact TOC/native heading matches restored across all zones. `
  - ` protected_content \| pass \| evidence: One same-agent retry validated under exact placeholders and DOM preflight; TOC titles all match destinations. `
  - ` qualification_preservation \| pass \| evidence: Uppercase-only BCP 14; illustrative wrapping chars are excluded; HTTPS always mandatory; audience restriction applies differently from sender constraint. `
  - ` semantic_fidelity \| pass \| evidence: Reviewed legal notices, original TOC and first sections; DPoP key binding imposes sender constraint, not client authentication. `
  - ` terminology \| pass \| evidence: Retains English-first nouns and literal quotation data, license name, citation names and HTTP variants. `
- **` zone-003 `**
  - ` boundary_consistency \| pass \| evidence: 161 introduces replay constraint; 220 decoded-caption is followed by 221 request coverage. `
  - ` naturalness \| pass \| evidence: Follows native prose and A–D flow; no client authentication versus proof ambiguity. `
  - ` protected_content \| pass \| evidence: All code, capitalization, translation placeholders, literal examples and links validated; DOM shape passed. `
  - ` qualification_preservation \| pass \| evidence: None and MAC prohibited under alg; private jwk key forbidden; negligible jti collision, at least 96 bits; ath and nonce only in respective cases. Erratum source wording faithfully translated and separately explained. `
  - ` semantic_fidelity \| pass \| evidence: 162–220: XSS context and non-extractable keys, A–D flow, TLS vs DPoP, header encoding, JOSE fields and claims. `
  - ` terminology \| pass \| evidence: DPoP proof JWT, header, JOSE, access token, private/public keys and nonce distinct. `
- **` zone-004 `**
  - ` boundary_consistency \| pass \| evidence: 220 to 221 from example to coverage; 265 JWK-thumbprint heading to 266 JWT representation. Targeted direct review of seg-000247: Figure 7: the original places the refresh token in the request, not in the key binding. The new sentence explicitly attaches it to requesting the DPoP-bound token. Cross-checked the same placement, normative scope, English identifiers and protected tokens. `
  - ` naturalness \| pass \| evidence: Checklist grouping, distinctions between condition and action, and formatting-relative details readable. Targeted direct review of seg-000247: Figure 7: the original places the refresh token in the request, not in the key binding. The new sentence explicitly attaches it to requesting the DPoP-bound token. Cross-checked the same placement, normative scope, English identifiers and protected tokens. `
  - ` protected_content \| pass \| evidence: Validated source-anchored references, JWT claims and literal BCP 14 text; DOM preflight passed. Targeted direct review of seg-000247: Figure 7: the original places the refresh token in the request, not in the key binding. The new sentence explicitly attaches it to requesting the DPoP-bound token. Cross-checked the same placement, normative scope, English identifiers and protected tokens. `
  - ` qualification_preservation \| pass \| evidence: Proof checks mandatory, URI normalization recommended, no cross-key use of public refresh, conditional discard and metadata false default retained. Targeted direct review of seg-000247: Figure 7: the original places the refresh token in the request, not in the key binding. The new sentence explicitly attaches it to requesting the DPoP-bound token. Cross-checked the same placement, normative scope, English identifiers and protected tokens. `
  - ` semantic_fidelity \| pass \| evidence: 221–265: request coverage and proof validation, issuance/refresh rules, Bearer alternative, metadata and key confirmation. Targeted direct review of seg-000247: Figure 7: the original places the refresh token in the request, not in the key binding. The new sentence explicitly attaches it to requesting the DPoP-bound token. Cross-checked the same placement, normative scope, English identifiers and protected tokens. `
  - ` terminology \| pass \| evidence: Client, grant types, token_type, metadata identifiers and public key retained. Targeted direct review of seg-000247: Figure 7: the original places the refresh token in the request, not in the key binding. The new sentence explicitly attaches it to requesting the DPoP-bound token. Cross-checked the same placement, normative scope, English identifiers and protected tokens. `
- **` zone-005 `**
  - ` boundary_consistency \| pass \| evidence: Heading 265 defines subject for 266; 306 origin-only, 307 explains Bearer-compatible credential syntax. `
  - ` naturalness \| pass \| evidence: Clarified qualifier attachment in 275, distinguishing schema choice from mandatory value. `
  - ` protected_content \| pass \| evidence: Corrected file and exact token sequences and DOM markup validated. `
  - ` qualification_preservation \| pass \| evidence: Introspection token_type optional but when present must be DPoP; native dual-token condition, all checks and challenge parameter force maintained. `
  - ` semantic_fidelity \| pass \| evidence: 266–306: jkt JWK hash in JWT and introspection, local resource validation, protected access and HTTP challenges. `
  - ` terminology \| pass \| evidence: Keeps jkt vs ath, introspection endpoint vs protected resource, DPoP vs Authorization names. `
- **` zone-006 `**
  - ` boundary_consistency \| pass \| evidence: 306 origin-only contrasts 307 credential syntax; 349 resource example precedes 350 per-issuer nonce guidance. `
  - ` naturalness \| pass \| evidence: Separate AS/RS chronology, local definitions and examples; request versus response paragraphs clear. `
  - ` protected_content \| pass \| evidence: Exact endpoints, MUST/SHOULD/MAY keywords, example and RFC links passed validator/DOM shape. `
  - ` qualification_preservation \| pass \| evidence: Reject DPoP-as-Bearer only at resource supporting both; three distinct challenge cases; nonce randomness and match; AS 400 vs RS 401; new nonce use until another. `
  - ` semantic_fidelity \| pass \| evidence: 307–349: Bearer compatibility boundaries, retries, AS and resource nonce challenge paths, default access to headers. `
  - ` terminology \| pass \| evidence: Same names for token/DPoP/challenge and CORS, HTTP header and error identifiers exact. `
- **` zone-007 `**
  - ` boundary_consistency \| pass \| evidence: Follows resource nonce example; ends with compromised client scenario flowing into 382 CSP defense. Targeted direct review of seg-000381: Section 11.4: the source refers to cryptographic APIs, not only encryption APIs. The correction retains the broader class and leaves the rest of the paragraph unchanged. Cross-checked the same placement, normative scope, English identifiers and protected tokens. `
  - ` naturalness \| pass \| evidence: Used complete conditional sentences and rerendered ordinary vs formal recommendation without force drift. Targeted direct review of seg-000381: Section 11.4: the source refers to cryptographic APIs, not only encryption APIs. The correction retains the broader class and leaves the rest of the paragraph unchanged. Cross-checked the same placement, normative scope, English identifiers and protected tokens. `
  - ` protected_content \| pass \| evidence: One same-agent retry exact token validation and DOM preflight; protected and structural values preserved. Targeted direct review of seg-000381: Section 11.4: the source refers to cryptographic APIs, not only encryption APIs. The correction retains the broader class and leaves the rest of the paragraph unchanged. Cross-checked the same placement, normative scope, English identifiers and protected tokens. `
  - ` qualification_preservation \| pass \| evidence: Issuer-only accepted fact and ordinary recommendation separated; both PAR methods when supported, mismatch rejection, time windows and same nonce reuse conditional on jti; short lifetime scoped to access token. Targeted direct review of seg-000381: Section 11.4: the source refers to cryptographic APIs, not only encryption APIs. The correction retains the broader class and leaves the rest of the paragraph unchanged. Cross-checked the same placement, normative scope, English identifiers and protected tokens. `
  - ` semantic_fidelity \| pass \| evidence: 350–381: per-server and OIDC nonce distinction, authorization-code key binding with PKCE/PAR, limitations, replay and pre-generation. Targeted direct review of seg-000381: Section 11.4: the source refers to cryptographic APIs, not only encryption APIs. The correction retains the broader class and leaves the rest of the paragraph unchanged. Cross-checked the same placement, normative scope, English identifiers and protected tokens. `
  - ` terminology \| pass \| evidence: Keeps nonce, ath, jti, iat, dpop_jkt, PKCE, PAR, proof terms and exact endpoints. Targeted direct review of seg-000381: Section 11.4: the source refers to cryptographic APIs, not only encryption APIs. The correction retains the broader class and leaves the rest of the paragraph unchanged. Cross-checked the same placement, normative scope, English identifiers and protected tokens. `
- **` zone-008 `**
  - ` boundary_consistency \| pass \| evidence: 381 compromised client followed by 382 defenses; 503 claim registry heading to 504 registration details. `
  - ` naturalness \| pass \| evidence: Repositioned readable normative annotations; repeated registration fields retain consistent labels and original values. `
  - ` protected_content \| pass \| evidence: Same-agent retry revalidated, DOM shape passed. `
  - ` qualification_preservation \| pass \| evidence: MUST reject nonsecure algorithms/none; current SHA-256 not generally selectable; future updated spec optional, not current alternatives. Request body not covered; transport is separate. `
  - ` semantic_fidelity \| pass \| evidence: 382–503: type confusion prevention, asymmetric algorithm rules, request integrity/TLS scope, hash collision vs second-preimage, code binding, IANA registrations through jkt. `
  - ` terminology \| pass \| evidence: Matches native headings and printed TOC; exact IANA, media type and registry payload identifiers. `
- **` zone-009 `**
  - ` boundary_consistency \| pass \| evidence: 503 heading completes clause at 504; 633 citation key followed by its matching citation 634. `
  - ` naturalness \| pass \| evidence: Parallel labels and Korean field descriptions; bibliographic data preserved with exact titles. `
  - ` protected_content \| pass \| evidence: Validated exact token, link and registry fields, all references and DOM. `
  - ` qualification_preservation \| pass \| evidence: htu omits query and fragment; ath ASCII→SHA-256→base64url; JWT nonce registration allows use in other JWT contexts, does not impose that use. `
  - ` semantic_fidelity \| pass \| evidence: 504–633: registered claims and descriptions, updated nonce definition, header names and statuses, metadata, normative/informative references. `
  - ` terminology \| pass \| evidence: Maintains OpenID nonce distinction, RFC numbers, English bibliography and IANA period/status values. `
- **` zone-010 `**
  - ` boundary_consistency \| pass \| evidence: 634 belongs to 633 RFC2046 key; 722 revision 09 leads into 723 revision 10. `
  - ` naturalness \| pass \| evidence: Exact citation convention through whole bibliography; concise Korean acknowledgments and matching duplicate error action label. `
  - ` protected_content \| pass \| evidence: Same-agent retry revalidated; source citation records exact, linked technical atoms and contact information preserved. `
  - ` qualification_preservation \| pass \| evidence: Dates, DOI/URI, draft recency and 4th workshop preserved without changing bibliography provenance. `
  - ` semantic_fidelity \| pass \| evidence: 634–722: remaining references, named contributors, Stuttgart workshop, six authors' contacts, and chrome controls. `
  - ` terminology \| pass \| evidence: Author spellings, proper organizations, RFC numbers, English titles and metadata retained. `
- **` zone-011 `**
  - ` boundary_consistency \| pass \| evidence: Finishes earlier revision list, no later neighbor. Site chrome does not enter complete RFC reader. `
  - ` naturalness \| pass \| evidence: Concise Korean labels/tooltip register with identical counterpart semantics. `
  - ` protected_content \| pass \| evidence: Validated exact IDs, protected URLs, email, version labels and DOM preflight. `
  - ` qualification_preservation \| pass \| evidence: Unchanged revision values 10–16; inline option is larger and network independent; direct citation vs section destination remains separate. `
  - ` semantic_fidelity \| pass \| evidence: 723–773: closing Datatracker revisions, metadata, link labels, accessibility and rendering/citation preferences. `
  - ` terminology \| pass \| evidence: Proper names, Datatracker, RFC, format literals and author affiliations unchanged. `
