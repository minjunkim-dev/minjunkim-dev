# MINJUN KIM

**Mobile Engineer · iOS / React Native**

Swift/iOS를 중심으로 React Native 앱까지 개발, 심사, 출시, 운영을 맡아 온 모바일 엔지니어입니다(경력 4년 4개월). Personal AI(구 SNPLAB) 개발팀(구 앱팀)에서 2022.06부터 2026.10까지 MyD iOS 앱과 tbn교통방송 React Native 앱을 맡았습니다. 장병e음 앱에는 모바일 신분증 모듈을 통합했습니다. 앱이 의존하는 SDK·인증 서버·CI/CD도 직접 구성했습니다.

성공 신호를 그대로 믿지 않고 확인합니다. 응답 코드, 빌드 통과, 도구의 '성공' 보고를 실제 결과로 다시 검증합니다. 대표 글: [HTTP 200은 배포 성공이 아니다](https://minjunkim-dev.github.io/writing/web-deploy-verify-public-sha256/)

## Projects

| Project | What | Highlights |
|---|---|---|
| [Runstir](https://github.com/minjunkim-dev/mobile-runtime) | 앱 개발 환경 준비·실행 도구 (Swift 6.2, alpha). alpha는 버전을 고정한 공개 React Native 앱으로 검증. Native 앱 실행·Flutter SDK 준비·macOS GUI는 main에 병합, alpha 검증 전 | 다른 프로젝트의 개발 서버(Metro)를 재사용해 실패를 성공으로 보고하던 문제 수정 · alpha.4 기준 테스트 482개 · ADR 40건 · Homebrew alpha |
| [smallnext](https://github.com/minjunkim-dev/smallnext) | 큰 목표를 지금 할 수 있는 다음 행동 하나로 바꾸는 플래너 (SwiftUI + Rust API, 미출시) | LLM 생성기·검사기 분리 · 비용 예약·정산 원장 · 생성·검사 전체 시간 중앙값 −16.9%(로컬 CLI, AB/BA 4쌍) |
| [Tech Notes](https://minjunkim-dev.github.io/) | 기술 글 4편. 글 속 코드는 글마다 테스트 파일로 두고 CI에서 실행 ([examples](https://github.com/minjunkim-dev/minjunkim-dev.github.io/tree/main/examples)) | 공개 응답 SHA-256 배포 검증 · fail-open 강제 업데이트 · actor 초기화 공유 · ImageIO 다운샘플링 |

## Production Experience

| Product | Scope | Links |
|---|---|---|
| **MyD** | Swift/iOS · 데이터 거래·본인인증·데이터 연동 · 앱 전체 기준 2022.06 이후 87개 버전 출시, 심사 제출은 대부분 직접 · 앱 전체 crash-free 세션 99.8%(2026년 7~9월) | [App Store](https://apps.apple.com/kr/app/id1576612543) · [Google Play](https://play.google.com/store/apps/details?id=io.snplab.myd) |
| **tbn교통방송** | React Native/TypeScript · 발주처 실무자와 요구사항·일정 직접 조율 · fail-open 강제 업데이트 · 2026-05-28 iOS·Android 정식 출시 | [App Store](https://apps.apple.com/kr/app/id969867489) · [Google Play](https://play.google.com/store/apps/details?id=com.mtelo.tbn) |
| **장병e음 모바일 신분증** | iOS 모듈 통합 · DID·VC 발급 통합과 온라인 검증 구현, 오프라인 검증 연계, 앱 보안 | [App Store](https://apps.apple.com/kr/app/id6744992032) · [Google Play](https://play.google.com/store/apps/details?id=kr.go.mnd.mosp) |
| **사내 인프라·CI/CD** | 2026.07–10, 앱 업무와 병행 · 원인 불명 Android CI 실패를 메모리 측정으로 OOM 규명 · CI 서버 디스크 사용률 100%→43%, 자동 정리기 설치 · Android CI 빌드 413초→174초(유휴 상태의 이전 Runner vs 캐시 있는 새 Runner) · Prometheus·Grafana로 서버 10대 감시, 알림 16개 | [배포 검증 글](https://minjunkim-dev.github.io/writing/web-deploy-verify-public-sha256/) |
| **B2B 데이터 수집 SDK·인증 서버** | 출시 준비 단계 · 설계·구현 혼자 담당 · Swift·Kotlin SDK, Node.js·PostgreSQL 인증 서버 · 고객사 영구 API 비밀키가 앱에 들어가지 않는 일회용 토큰 구조 · Android SDK 테스트 간헐 실패 2,400세션 중 15건→0건(실행 순서 경합 규명) | 비공개 |

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
