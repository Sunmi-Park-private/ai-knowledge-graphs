# AI Knowledge Graphs

**보기: https://sunmi-park-private.github.io/ai-knowledge-graphs/**

[graphify](https://pypi.org/project/graphifyy/)로 만든 AI 프로젝트 7개의 코드·문서 지식그래프입니다. 코드는 구문 분석(AST)으로, 설계·운영 문서는 의미 추출로 노드와 엣지를 만들고 커뮤니티를 탐지했습니다.

| 프로젝트 | 구분 | 노드 | 엣지 | 커뮤니티 | 발견 한 줄 |
|---|---|---:|---:|---:|---|
| [UACOS](uacos/) | 회사 · 사내 AI JAM 1·2등 제품 통합 | 1,030 | 1,477 | 72 | 허브 1위 = 용어집(지식 파이프라인이 중심축) |
| [ViTag](vitag/) | 회사 · 사내 AI JAM 2등 | 1,314 | 2,275 | 140 | "있어 보이지만 배선 안 됨" 패턴을 코드·배포에서 동시에 발견 |
| [SceneStealer](scenestealer/) | 회사 · 사내 AI JAM 1등 | 937 | 1,824 | 59 | 기능 스펙 16개 ↔ 코드 엣지 0개 |
| [Debut Loop!](debut-loop/) | NHN×AI 해커톤 예선 입상 | 1,108 | 2,910 | 47 | 허브 1위 = 따로 진단한 기술 부채 1순위 |
| [Red Horse Rescue 2026](red-horse-rescue/) | NHN×AI 해커톤 본선 · 35시간 | 1,313 | 3,436 | 50 | 허브 1위 = 테스트 러너 |
| [TravelZip](travel-zip/) | 관광데이터 공모전 웹·앱 개발 부문 | 13,425 | 36,331 | 374 | 엔드포인트 전체가 같은 오류·응답 계약 공유 |
| [FestaOn](festaon/) | 관광데이터 공모전 웹·앱 구현 부문 | 12,458 | 32,917 | 386 | 교환권 서비스 3개 순환 의존 발견 |


## 데모 영상

썸네일을 누르면 YouTube에서 재생됩니다. [Pages 첫 화면](https://sunmi-park-private.github.io/ai-knowledge-graphs/)에서는 페이지 안에서 바로 재생됩니다.

| SceneStealer (사내 AI JAM 1등) | Debut Loop! (NHN×AI 해커톤 예선 입상) |
|---|---|
| [![SceneStealer 데모](https://img.youtube.com/vi/3kf9y-sJO7U/hqdefault.jpg)](https://youtu.be/3kf9y-sJO7U) | [![Debut Loop! 게임플레이](https://img.youtube.com/vi/YL6snM3RfzM/hqdefault.jpg)](https://youtu.be/YL6snM3RfzM) |
| **Red Horse Rescue 2026 (NHN×AI 해커톤 본선)** | **Game Hit Hunter (Databricks APJ Hackathon 2026)** |
| [![Red Horse Rescue 게임플레이](https://img.youtube.com/vi/ugOV7KuEAW8/hqdefault.jpg)](https://youtu.be/ugOV7KuEAW8) | [![Game Hit Hunter 데모](https://img.youtube.com/vi/gwZUOpO1z5o/hqdefault.jpg)](https://youtu.be/gwZUOpO1z5o) |

각 폴더: `graph.html`(대화형 그래프, 브라우저로 열기) · `report.md`(허브·커뮤니티·연결 요약)

- 소스 코드는 공개하지 않습니다. 그래프와 요약 리포트만 공개합니다.
- 회사 프로젝트의 사내 인프라 식별자(스토리지 버킷·내부 도메인·권한 역할·티켓 번호)는 공개본에서 일반 표기로 바꿨습니다.
- 노드 5,000개가 넘는 그래프(TravelZip·FestaOn)는 커뮤니티 단위 요약 보기입니다.
- 빌드 2026-09-27 · 박선미 ([github.com/Sunmi-Park-private](https://github.com/Sunmi-Park-private))
