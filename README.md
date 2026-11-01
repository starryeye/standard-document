# standard-document

원문과 대조·검토한 기술 표준의 비공식 한국어 번역본을 보관합니다. 번역에는 [supertranslator](https://github.com/starryeye/supertranslator)를 사용했습니다.

## 번역 문서

| 문서 | 번역본 | 검토 결과 | 원문 |
| --- | --- | --- | --- |
| RFC 6749 — OAuth 2.0 Authorization Framework | [HTML](rfc/rfc6749/index.html) | [직접 검토](rfc/rfc6749/controller-review.md) · [QA](rfc/rfc6749/review-report.md) | [IETF](https://datatracker.ietf.org/doc/rfc6749/) |
| RFC 6750 — OAuth 2.0 Bearer Token Usage | [HTML](rfc/rfc6750/index.html) | [직접 검토](rfc/rfc6750/controller-review.md) · [QA](rfc/rfc6750/review-report.md) | [IETF](https://datatracker.ietf.org/doc/rfc6750/) |
| RFC 9700 — Best Current Practice for OAuth 2.0 Security | [HTML](rfc/rfc9700/index.html) | [직접 검토](rfc/rfc9700/controller-review.md) · [QA](rfc/rfc9700/review-report.md) | [IETF](https://datatracker.ietf.org/doc/html/rfc9700/) |

AI가 직접 번역하고, 전체 원문·번역 대조와 구조·화면 검토를 거친 결과입니다. 코드·도식·URL·프로토콜 식별자는 원문을 유지합니다. 세부적인 보존 범위와 주의점은 문서별 직접 검토 기록을 확인하세요.

RFC 6749·6750의 설명은 2012년 발행본의 맥락을 유지합니다. 이후의 보안 권고는 RFC 9700을 함께 참고하세요. 비공식 번역이므로 해석에 차이가 있으면 IETF의 공식 영문 원문을 기준으로 합니다. IETF의 승인이나 보증을 의미하지 않습니다.

## 읽는 방법

현재는 저장소에 파일을 보관하는 단계이며, GitHub Pages는 활성화하지 않았습니다. GitHub의 HTML 링크는 소스 보기로 열립니다. 저장소를 내려받고 각 `rfc/rfc번호/index.html`을 브라우저에서 열면 번역 페이지를 읽을 수 있습니다. 같은 폴더의 `assets/`를 함께 유지해야 합니다.

원본 Datatracker의 RSS, 웹앱 manifest, 사이트 상태 표시 기능은 이 저장소에서 제공하지 않습니다. HTML을 그대로 보존했으므로 해당 원본 사이트 기능의 경로 참조는 남아 있으며, Pages를 연결할 때 점검할 항목입니다. 번역 본문과 필요한 스타일·글꼴·이미지는 포함되어 있습니다.

## 공개 범위와 검증 기록

- 완료된 세 RFC의 HTML, 필요한 정적 자산, 검토 보고서와 공개용 `manifest.json`만 포함합니다.
- HTML·자산·검토 보고서는 검토가 끝난 로컬 산출물과 바이트가 동일합니다. 공개용 manifest에서는 로컬 스크린샷 경로만 제외하고 제외 사유를 표시했습니다. 원래 증거와 실행 기록은 로컬에 보존합니다.
- 작업 중인 번역, 실패한 실행, 로컬 환경·에이전트 기록, 상용 책 PDF는 포함하지 않습니다.
- RFC 9700까지 번역한 뒤 작업을 중단한 상태입니다. 후속 문서를 자동으로 번역하거나 게시하지 않습니다.

문서와 포함된 자산의 권리는 각각의 원 저작권자에게 있습니다. 이 저장소 전체에 별도 일괄 라이선스를 부여하지 않습니다. [원문 저작권 고지](NOTICE.md)와 각 RFC의 고지를 참고하세요.
