# MINJUN KIM

**Mobile Engineer · iOS / React Native · RAG·SDK·CI/CD·인프라**

Swift/iOS를 중심으로 React Native 앱까지 개발, 심사, 출시, 운영을 맡아 온 모바일 엔지니어입니다(경력 4년 4개월). Personal AI(구 SNPLAB) 개발팀(구 앱팀)에서 2022.06부터 2026.10까지 MyD iOS 앱과 tbn교통방송 React Native 앱을 맡았습니다. 장병e음 앱에는 모바일 신분증 모듈을 통합했습니다. 사내 고객 문의 자동 답변(RAG)을 운영에 연결했고, B2B 데이터 수집 SDK와 인증 서버를 설계했습니다. 2026년 7월부터는 앱 업무와 함께 사내 CI/CD·배포·모니터링·사내망을 맡았습니다. 자동 답변·SDK·인프라의 구현은 AI 코딩 에이전트 위주로 하고, 저는 에이전트가 지킬 조건을 정하고 결과를 검증했습니다. 앱 경험을 바탕으로 모바일 플랫폼·인프라로 일의 범위를 넓히고 있습니다.

성공 신호를 그대로 믿지 않고 확인합니다. 응답 코드, 빌드 통과, 도구의 '성공' 보고를 실제 결과로 다시 검증합니다. 대표 글: [HTTP 200은 배포 성공이 아니다](https://minjunkim-dev.github.io/writing/web-deploy-verify-public-sha256/)

## Production Experience

| Work | Scope | Links |
|---|---|---|
| **MyD** | Swift/iOS · 데이터 거래·본인인증 화면 흐름·데이터 연동 · 앱 전체 기준 2022.06 이후 87개 버전 출시, 심사 제출은 대부분 직접 · iOS 앱 crash-free 세션 99.8%(2026년 7~9월, Crashlytics) | [App Store](https://apps.apple.com/kr/app/id1576612543) · [Google Play](https://play.google.com/store/apps/details?id=io.snplab.myd) |
| **tbn교통방송** | React Native/TypeScript · 발주처 실무자와 요구사항·일정 직접 조율 · fail-open 강제 업데이트 · 2026-05-28 iOS·Android 정식 출시 | [App Store](https://apps.apple.com/kr/app/id969867489) · [Google Play](https://play.google.com/store/apps/details?id=com.mtelo.tbn) |
| **장병e음 모바일 신분증** | iOS 모듈 통합 · DID·VC 발급 통합과 온라인 검증 구현, 오프라인 검증 연계, 앱 보안 | [App Store](https://apps.apple.com/kr/app/id6744992032) · [Google Play](https://play.google.com/store/apps/details?id=kr.go.mnd.mosp) |
| **MyD 고객 문의 자동 답변(RAG)** | 사내 · 2026.06–07, 운영 2026.10까지 · Python·FastAPI·bge-m3·ChromaDB·로컬 LLM·n8n · Jira로 들어온 고객 문의에 FAQ 근거로 답하고, 근거가 부족하면 답하지 않고 운영자에게 넘김 · 샘플 FAQ를 실제 FAQ 9개 문서로 바꿔 실제 고객 문의에 적용 · 구현은 AI 코딩 에이전트, 에이전트가 지킬 조건 지정과 결과 검증은 본인 | 비공개 |
| **B2B 데이터 수집 SDK·인증 서버** | 고객사 전달 전 중단 · 설계·검증은 본인, 구현은 AI 코딩 에이전트 위주 · Swift·Kotlin SDK, Node.js·PostgreSQL 인증 서버 · 고객사 영구 API 비밀키가 앱에 들어가지 않는 일회용 토큰 구조 · Android SDK 테스트 간헐 실패 2,400세션 중 15건→0건(실행 순서 경합 규명) | 비공개 |
| **사내 CI/CD·배포** | 2026.07–10, 앱 업무와 병행 · 구현은 대부분 AI 코딩 에이전트, 에이전트가 지킬 조건 지정과 결과 검증은 본인 · 원인 불명 Android CI 실패를 메모리 측정으로 OOM 규명 · CI 서버 디스크 사용률 100%→43%, 디스크가 찰수록 오래된 데이터를 더 일찍 지우는 정리 작업 자동화 · Android CI 빌드 413초→174초(유휴 상태의 이전 Runner vs 캐시 있는 새 Runner) · 웹 프론트 3종 배포를 공개 URL 응답의 SHA-256 일치로 판정, 롤백 추가 · Bitbucket·Jenkins에서 GitLab으로 저장소 8개 이전 | [배포 검증 글](https://minjunkim-dev.github.io/writing/web-deploy-verify-public-sha256/) |
| **사내 모니터링·사내망** | 구현은 대부분 AI 코딩 에이전트 · Prometheus·Grafana로 서버 10대·대상 18개 수집, 알림 16개 · 사내망을 OpenVPN에서 Cloudflare WARP(Zero Trust)로 전환 | 비공개 |
| **마이주식** | Flutter·Firebase · 인턴 프로젝트 기술 지원(보안·배포·서버리스 백엔드) · 1.1.0 출시 당일 1.0.0 앱의 가입 실패를 운영 로그로 추적해 복구 · Firebase Functions 통합 테스트 572건 74.5초→약 20초(로컬, 워커 4개) | [App Store](https://apps.apple.com/kr/app/id6805333415) · [Google Play](https://play.google.com/store/apps/details?id=com.personalai.mytalk) · [ONE store](https://m.onestore.co.kr/v2/ko-kr/app/0001009180) |

## Projects

| Project | What | Highlights |
|---|---|---|
| [Runstir](https://github.com/minjunkim-dev/mobile-runtime) | 앱 개발 환경 준비·실행 도구 (Swift 6.2, alpha). alpha는 버전을 고정한 공개 React Native 앱으로 검증. Native 앱 실행·Flutter SDK 준비·macOS GUI는 main에 병합, alpha 검증 전 | 다른 프로젝트의 개발 서버(Metro)를 재사용해 실패를 성공으로 보고하던 문제 수정 · alpha.4 기준 테스트 482개 · ADR 40건 · Homebrew alpha |
| [smallnext](https://github.com/minjunkim-dev/smallnext) | 큰 목표를 지금 할 수 있는 다음 행동 하나로 바꾸는 플래너 (SwiftUI + Rust API, 미출시) | LLM 생성기·검사기 분리 · 비용 예약·정산 원장 · 생성·검사 전체 시간 중앙값 −16.9%(로컬 CLI, AB/BA 4쌍) |
| [Tech Notes](https://minjunkim-dev.github.io/) | 기술 글 4편. 글 속 코드는 글마다 테스트 파일로 두고 CI에서 실행 ([examples](https://github.com/minjunkim-dev/minjunkim-dev.github.io/tree/main/examples)) | 공개 응답 SHA-256 배포 검증 · fail-open 강제 업데이트 · actor 초기화 공유 · ImageIO 다운샘플링 |

## Focus

- **AI:** RAG(사내, 에이전트 구현): Python·FastAPI, bge-m3, ChromaDB, n8n · Anthropic API, Claude Code·Codex
- **iOS:** Swift, SwiftUI, UIKit, Swift Concurrency, SwiftPM·XCFramework SDK
- **Cross-platform:** React Native, TypeScript, Kotlin/Android, Flutter·KMP 연동
- **Server:** Node.js, TypeScript(Firebase Functions), Rust(axum·sqlx), PostgreSQL, Firestore
- **CI/CD:** GitLab CI, GitHub Actions, Jenkins, Fastlane
- **Infra & ops:** Linux·Docker(GitLab Runner), AWS(CloudFront·S3 배포, ALB·Route 53은 구성 문서화), NGINX, Prometheus·Grafana, Cloudflare Zero Trust
- **Reliability:** race·timeout·fail-open 설계, 측정으로 원인 찾기

## How I Work with AI

스펙, 티켓, 구현, 리뷰, MR을 에이전트로 잇고, AI가 만든 변경도 사람이 쓴 변경과 같은 테스트·리뷰·CI 관문을 통과해야 병합합니다.

## Links

[Tech Notes](https://minjunkim-dev.github.io/) · [LinkedIn](https://www.linkedin.com/in/minjun-kim-bene-dev/) · [Email](mailto:minjunkim.dev@gmail.com)
