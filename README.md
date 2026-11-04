# standard-document

원문과 대조·검토한 기술 표준의 비공식 한국어 번역본을 보관합니다. 번역에는 [supertranslator](https://github.com/starryeye/supertranslator)를 사용했습니다.

**[블로그에서 읽기](https://starryeye.github.io/) · [독립 읽기용 보관본](https://starryeye.github.io/standard-document/) · [GitHub 저장소](https://github.com/starryeye/standard-document)**

## 번역 문서

### RFC 6749 — OAuth 2.0 Authorization Framework

[블로그 전문](https://starryeye.github.io/rfc/rfc6749/) · [보관본](https://starryeye.github.io/standard-document/rfc/rfc6749/) · [검토 기록](rfc/rfc6749/controller-review.md) · [공식 원문](https://datatracker.ietf.org/doc/rfc6749/)

### RFC 6750 — OAuth 2.0 Bearer Token Usage

[블로그 전문](https://starryeye.github.io/rfc/rfc6750/) · [보관본](https://starryeye.github.io/standard-document/rfc/rfc6750/) · [검토 기록](rfc/rfc6750/controller-review.md) · [공식 원문](https://datatracker.ietf.org/doc/rfc6750/)

### RFC 9700 — Best Current Practice for OAuth 2.0 Security

[블로그 전문](https://starryeye.github.io/rfc/rfc9700/) · [보관본](https://starryeye.github.io/standard-document/rfc/rfc9700/) · [검토 기록](rfc/rfc9700/controller-review.md) · [공식 원문](https://datatracker.ietf.org/doc/html/rfc9700/)

AI가 직접 번역하고, 전체 원문·번역 대조와 구조·화면 검토를 거친 결과입니다. 코드·도식·URL·프로토콜 식별자는 원문을 유지합니다. 세부적인 보존 범위와 주의점은 문서별 직접 검토 기록을 확인하세요.

RFC 6749·6750의 설명은 2012년 발행본의 맥락을 유지합니다. 이후의 보안 권고는 RFC 9700을 함께 참고하세요. 비공식 번역이므로 해석에 차이가 있으면 IETF의 공식 영문 원문을 기준으로 합니다. IETF의 승인이나 보증을 의미하지 않습니다.

## 읽는 방법

위의 읽기 링크를 누르면 GitHub Pages에서 번역본을 바로 읽을 수 있습니다. 로그인 없이 다른 기기의 브라우저에서도 같은 주소로 접근할 수 있습니다.

오프라인에서 읽으려면 저장소를 내려받고 각 `rfc/rfc번호/index.html`을 브라우저에서 여세요. 같은 폴더의 `assets/`를 함께 유지해야 합니다.

GitHub Pages는 `main` 브랜치의 루트에서 게시됩니다. 저장소에 변경 사항을 푸시하면 GitHub의 기본 Pages 빌드·배포가 실행됩니다. 별도 애플리케이션 서버나 사용자 정의 배포 워크플로는 사용하지 않습니다.

현재 게시본은 설치된 supertranslator 0.10.1로 생성한 읽기용 파생본입니다. 영어 명사를 유지하면서 원문과 대조한 두 문장만 AI가 교정했습니다. 접힌 계층형 목차에서 실제 절로 이동할 수 있으며, 출판 정보와 원래 인쇄 목차는 삭제하지 않고 펼쳐 볼 수 있게 보존했습니다. 본문은 PC 18px·모바일 16px이고, 코드·도식은 원래 줄바꿈과 가로 스크롤을 유지합니다. 새 전면 재번역이나 모든 문장의 새 의미 감수를 했다는 뜻은 아닙니다. 처음 생성한 원문 보존형 HTML과 이전 편집본은 Git 이력과 로컬 실행 기록에 남아 있습니다.

## 공개 범위와 검증 기록

- 완료된 세 RFC의 HTML, 필요한 정적 자산, 검토 보고서와 공개용 `manifest.json`만 포함합니다.
- HTML·본문 조각·스타일과 자산은 검토가 끝난 읽기용 산출물과 바이트가 동일합니다. 렌더링 승인은 HTML·CSS·그림 해시 전체에 결합됩니다. 큰 화면 타일은 저장소에 포함하지 않으며, 원래 증거와 실행 기록은 로컬에 보존합니다.
- `input-*` 보고서는 이전 번역의 검토 기록입니다. 현재 편집 검토와 혼동하지 않도록 별도로 보존합니다. 이번 변경은 새 전면 번역이나 새 의미 검토가 아닙니다.
- 작업 중인 번역, 실패한 실행, 로컬 환경·에이전트 기록, 상용 책 PDF는 포함하지 않습니다.
- RFC 9700까지 번역한 뒤 작업을 중단한 상태입니다. 후속 문서를 자동으로 번역하거나 게시하지 않습니다.

문서와 포함된 자산의 권리는 각각의 원 저작권자에게 있습니다. 이 저장소 전체에 별도 일괄 라이선스를 부여하지 않습니다. [원문 저작권 고지](https://github.com/starryeye/standard-document/blob/main/NOTICE.md)와 각 RFC의 고지를 참고하세요.
