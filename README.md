# MINJUN KIM

**Mobile Engineer · iOS Core / React Native Production**

Swift/iOS를 중심으로 React Native 양 플랫폼 제품의 구현, 출시, 테스트와 운영까지 맡는 5년차 모바일 엔지니어입니다. 현재 Personal AI(구 SNPLAB) 앱팀에서 MyD와 TBN교통방송을 유지보수·운영하고 있습니다.

## Featured Open Source

### [ios-production-patterns](https://github.com/minjunkim-dev/ios-production-patterns)

Swift 6 패키지로 정리한 모바일 운영 신뢰성 패턴입니다. 잘못된 원격 정책을 안전하게 통과시키는 version gate, stale 비동기 응답을 차단하는 latest-request gate, bounded timeout을 XCTest와 GitHub Actions로 검증합니다.

## Production Experience

| Product | Scope | Public links |
|---|---|---|
| **MyD · 마이디** | Swift/iOS 중심 · KMC 본인인증·데이터 거래·스크래핑·네이티브 통합 · 현재 운영 | [App Store](https://apps.apple.com/kr/app/id1576612543) · [Google Play](https://play.google.com/store/apps/details?id=io.snplab.myd) |
| **TBN교통방송** | React Native/TypeScript · KMC 본인인증·Kakao/Apple SNS 가입·로그인 · iOS/Android 출시·현재 운영 | [App Store](https://apps.apple.com/kr/app/id969867489) · [Google Play](https://play.google.com/store/apps/details?id=com.mtelo.tbn) |
| **장병e음 모바일 신분증 솔루션** | DID·VC·App Attest·온라인/오프라인 검증 · iOS 중심 구현과 Android 기능 보완 | [App Store](https://apps.apple.com/kr/app/id6744992032) · [Google Play](https://play.google.com/store/apps/details?id=kr.go.mnd.mosp) |

세 제품은 Google Play 공개 기준 각각 **10만+ 다운로드** 제품입니다. 다운로드 수는 제품 공개 지표이며 개인 기여 성과와 직접 연결하지 않습니다.

## Engineering Focus

- **iOS:** Swift, SwiftUI, UIKit, app lifecycle, Keychain, APNs, WebView/native bridge
- **Cross-platform production:** React Native, TypeScript, Kotlin/Android, Flutter/KMP integration
- **Reliability:** async race, cancellation, timeout, fail-open policy, state-machine design
- **Testing:** XCTest, Jest, React Native Testing Library, KMP and build-contract tests
- **Release & operations:** App Store/Google Play review, Jenkins, Fastlane, Firebase App Distribution
- **Mobile identity:** KMC identity verification, Kakao/Apple social sign-in flow, DID/VC, App Attest, biometric and screen security

## How I Use AI

AI는 제한된 구현·탐색·코드 리뷰에 활용하고, 최종 판단은 실제 코드와 시스템 불변식, 자동화 테스트 결과를 기준으로 검증합니다. TBN 백그라운드 편성 동기화에서는 Claude-assisted 구현을 Codex 사후 리뷰로 교차 검증하고, 재시도·취소·stale 응답·GA 귀속 race 제안을 채택 또는 기각한 뒤 확정 항목만 회귀 테스트와 함께 통합했습니다.

## Links

- [Tech Notes](https://minjunkim-dev.github.io/)
- [LinkedIn](https://www.linkedin.com/in/minjun-kim-bene-dev/)
- [Email](mailto:minjunkim.dev@gmail.com)
