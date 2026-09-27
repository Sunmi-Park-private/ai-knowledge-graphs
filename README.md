# AI Knowledge Graphs

**보기: https://sunmi-park-private.github.io/ai-knowledge-graphs/**

[graphify](https://pypi.org/project/graphifyy/)로 만든 AI 프로젝트 7개의 코드·문서 지식그래프입니다. 코드는 구문 분석(AST)으로, 설계·운영 문서는 의미 추출로 노드와 엣지를 만들고 커뮤니티를 탐지했습니다.

| 프로젝트 | 구분 | 노드 | 엣지 | 커뮤니티 | 그래프가 보여 준 것 |
|---|---|---:|---:|---:|---|
| [UACOS](uacos/) | 회사 · 사내 AI JAM 1·2등 제품 통합 | 1,030 | 1,477 | 72 | 가장 많이 연결된 문서가 용어집 — 팀이 쌓아 온 용어 정의가 설계 문서 전반을 하나로 잇는 공통 기준이 되고 있음 |
| [ViTag](vitag/) | 회사 · 사내 AI JAM 2등 | 1,314 | 2,275 | 140 | 코드와 배포 설정 두 곳에 흩어져 있던 같은 유형의 문제(설정은 돼 있지만 실제로는 쓰이지 않음)를 한 번에 찾아내 점검 범위를 넓힘 |
| [SceneStealer](scenestealer/) | 회사 · 사내 AI JAM 1등 | 937 | 1,824 | 59 | 기획 문서와 코드 사이의 연결 공백을 찾아내 "스펙마다 구현 파일을 명시한다"는 개선 방향을 도출 |
| [Debut Loop!](debut-loop/) | NHN×AI 해커톤 예선 입상 | 1,108 | 2,910 | 47 | 게임의 여러 기능이 화면을 띄우는 함수 하나(1,460줄)에 몰려 있다는 것을 찾아냄 — 개발자가 "가장 먼저 나눠야 할 코드"로 꼽았던 곳과 정확히 일치 |
| [Red Horse Rescue 2026](red-horse-rescue/) | NHN×AI 해커톤 본선 · 35시간 | 1,313 | 3,436 | 50 | 게임의 주요 기능 20곳이 자동 테스트로 검증되고 있었음 — 35시간 만에 만든 게임이지만 기능마다 자동 테스트로 확인하며 개발 |
| [TravelZip](travel-zip/) | 관광데이터 공모전 웹·앱 개발 부문 | 13,425 | 36,331 | 374 | 수백 개 API가 하나의 공통 오류·응답 규칙을 따르고 있음을 확인 — 두 앱이 함께 쓰는 백엔드의 일관성 |
| [FestaOn](festaon/) | 관광데이터 공모전 웹·앱 구현 부문 | 12,458 | 32,917 | 386 | 교환권·어뷰즈 방지 모듈 사이의 순환 참조를 찾아 다음 정리 대상으로 확정 — 개선 지점을 구조로 짚어냄 |


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
