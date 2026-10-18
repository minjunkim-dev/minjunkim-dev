# MINJUN KIM

**Mobile Engineer · iOS / React Native**

Swift/iOS를 중심으로 React Native 앱까지 개발, 심사, 출시, 운영을 맡아 온 모바일 엔지니어입니다(경력 4년 4개월). Personal AI(구 SNPLAB) 앱팀에서 2022.06부터 2026.10까지 MyD, tbn교통방송, 장병e음 모바일 신분증을 만들었고, 앱이 의존하는 SDK·인증 서버·CI/CD도 직접 구성했습니다.

성공 신호를 그대로 믿지 않고 확인합니다. 응답 코드, 빌드 통과, 도구의 '성공' 보고를 실제 결과로 다시 검증합니다. 대표 글: [HTTP 200은 배포 성공이 아니다](https://minjunkim-dev.github.io/writing/web-deploy-verify-public-sha256/)

## Projects

| Project | What | Highlights |
|---|---|---|
| [Runstir](https://github.com/minjunkim-dev/mobile-runtime) | `git clone` 후 `mobile up` 한 번으로 React Native 앱을 Simulator·Emulator에서 실행하는 macOS CLI (Swift 6.2) | Metro 정체성 판정으로 거짓 성공 제거 · 테스트 415개 · ADR 37건 · Homebrew alpha |
| [smallnext](https://github.com/minjunkim-dev/smallnext) | 큰 목표를 지금 할 수 있는 다음 행동 하나로 바꾸는 플래너 (SwiftUI + Rust API) | LLM 생성기·검사기 분리 · 비용 예약·정산 원장 · 검사 지연 −39.4% (로컬 실측) |
| [ios-production-patterns](https://github.com/minjunkim-dev/ios-production-patterns) | 운영에서 겪은 문제를 일반화한 Swift 6 패키지 | fail-open version gate · latest-request gate · bounded timeout · actor startup coordinator |

## Production Experience

| Product | Scope | Links |
|---|---|---|
| **MyD** | Swift/iOS · 데이터 거래·본인인증·데이터 연동 · 87개 버전 배포, crash-free 세션 99.8% (2026년 7~9월) | [App Store](https://apps.apple.com/kr/app/id1576612543) · [Google Play](https://play.google.com/store/apps/details?id=io.snplab.myd) |
| **tbn교통방송** | React Native/TypeScript · fail-open 강제 업데이트 · 2026-05-28 iOS·Android 정식 출시 | [App Store](https://apps.apple.com/kr/app/id969867489) · [Google Play](https://play.google.com/store/apps/details?id=com.mtelo.tbn) |
| **장병e음 모바일 신분증** | iOS 모듈 통합 · DID·VC 발급과 온라인 검증 구현, 오프라인 검증 연계, 앱 보안 | [App Store](https://apps.apple.com/kr/app/id6744992032) · [Google Play](https://play.google.com/store/apps/details?id=kr.go.mnd.mosp) |

다운로드 수 같은 제품 지표는 개인 성과와 섞지 않습니다.

## Focus

- **iOS:** Swift, SwiftUI, UIKit, Swift Concurrency, SwiftPM·XCFramework SDK
- **Cross-platform:** React Native, TypeScript, Kotlin/Android, Flutter 연동
- **Server & delivery:** Node.js, Rust(axum), PostgreSQL, GitLab CI, Fastlane
- **Infra & ops:** GitLab Runner(Docker), Prometheus·Grafana, AWS(CloudFront·S3), Cloudflare Zero Trust
- **Reliability:** race·timeout·fail-open 설계, 측정으로 원인 찾기

## How I Work with AI

스펙, 티켓, 구현, 리뷰, MR을 에이전트로 잇고, AI가 만든 변경도 사람이 쓴 변경과 같은 테스트·리뷰·CI 관문을 통과해야 병합합니다.

## Links

[Tech Notes](https://minjunkim-dev.github.io/) · [LinkedIn](https://www.linkedin.com/in/minjun-kim-bene-dev/) · [Email](mailto:minjunkim.dev@gmail.com)
