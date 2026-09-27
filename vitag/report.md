# Graph Report - vitag  (2026-09-27)

## Corpus Check
- 209 files · ~135,867 words
- Verdict: corpus is large enough that graph structure adds value.

## Summary
- 1314 nodes · 2275 edges · 140 communities (66 shown, 74 thin omitted)
- Extraction: 94% EXTRACTED · 5% INFERRED · 0% AMBIGUOUS · INFERRED: 125 edges (avg confidence: 0.78)
- Token cost: 443,878 input · 0 output

## Community Hubs (Navigation)
- 태그 탐색기 UI
- 태그 연관 그래프 · API 클라이언트
- 공용 UI 프리미티브
- 크리에이티브 갤러리 검색·필터
- 영상 태그 검색 서비스
- 태그 추출 화면·진행 표시
- FastAPI 앱 진입점·시간 유틸
- 태그 키워드 조회 서비스
- 프론트엔드 빌드 의존성
- 히스토리 화면·한글 폰트 등록
- 설계·계획 문서와 Helm 차트
- S3 업로드·썸네일 생성
- TypeScript 컴파일 설정
- 태그 상관 서비스·캐시
- Redis 작업 추적기(JobTracker)
- 레포 문서 지도
- 태그 추출 엔드포인트·Lambda 호출
- Google Drive 수집
- 태그 추출 스키마
- 크리에이티브 카드·상세 모달
- 환경별 Helm values
- 태그 히스토리 서비스
- 배포 함정 기록(빌드타임 인라인·이미지 스킵)
- 크리에이티브 스키마
- shadcn 컴포넌트 설정
- 영상 검색 화면·페이지네이션
- 트렌드 지표 서비스
- 태그 히스토리 스키마
- 크리에이티브 서비스
- 태그 상관 스키마
- 운영 배포 잡 · prod values 이중화
- 파일명 안전 변환·CloudFront URL
- SQLAlchemy 모델
- 대시보드 사이드바
- UACOS 연동 계약·검색 보안 결함
- 프론트엔드 런타임 의존성
- Aurora 덤프 적재 배치
- Lambda 호출 서비스
- 규칙 파일(5법칙·시크릿·커밋)
- Aurora 스키마·적재 파이프라인
- 크리에이티브 API
- 트렌드 API
- DB 연결·시크릿 조회
- 트렌드 스키마
- dev 배포 잡
- 히스토리 API
- 헬스체크·페이지 라우트
- Next.js 루트 레이아웃
- 토글 컴포넌트
- Tableau 임베드·토큰
- 태그 히스토리 모델
- ESLint 설정
- 워드클라우드 차트 타입
- Tableau 타입 선언
- Tableau JWT 발급 라우트
- .unregister_sse_client()
- WordCloud.tsx
- middleware.ts
- chartjs-chart-wordcloud
- chartjs-plugin-zoom
- class-variance-authority
- clsx
- d3
- @gaia-portal/gnb
- @gaia-ui/core
- redis_prod_deploy Job
- hangul-romanization
- jose
- Unidirectional grep misses cross-repo de
- Reviewer/controller-provided citations a
- next
- next-themes
- @radix-ui/react-accordion
- @radix-ui/react-checkbox
- @radix-ui/react-collapsible
- @radix-ui/react-dialog
- @radix-ui/react-label
- @radix-ui/react-navigation-menu
- @radix-ui/react-popover
- @radix-ui/react-progress
- @radix-ui/react-scroll-area
- @radix-ui/react-select
- @radix-ui/react-separator
- @radix-ui/react-slider
- @radix-ui/react-slot
- @radix-ui/react-switch
- @radix-ui/react-toggle
- @radix-ui/react-toggle-group
- react
- react-day-picker
- react-dom
- server-only
- sonner
- @tableau/embedding-api
- tailwind-merge
- @types/d3
- endpoints/__init__.py
- router.py
- config.py
- core/__init__.py
- services/__init__.py
- utils/__init__.py
- next.config.ts
- zustand
- postcss.config.mjs
- dev/sensortower_ad_creative_details.sql
- dev/tag_all_creative_keywords.sql
- dev/tag_explorer_ranked_data.sql
- dev/tag_monthly_trends_metrics.sql
- dev/tag_weekly_trends_metrics.sql
- dev/vitag_tag_history.sql
- prod/sensortower_ad_creative_details.sql
- prod/tag_all_creative_keywords.sql
- prod/tag_explorer_ranked_data.sql
- prod/tag_monthly_trends_metrics.sql
- prod/tag_weekly_trends_metrics.sql
- prod/vitag_tag_history.sql
- Check Pod Log Workflow
- Pluto K8s API Check Workflow
- prod_check_k8s_api Job
- build_only Job
- release_build_and_push Job
- Diff and Deploy Workflow
- Dimension
- Genre
- Share of Voice (SoV)
- Tag Insight
- Duplicated rule files always drift

## God Nodes (most connected - your core abstractions)
1. `cn()` - 93 edges
2. `Button()` - 19 edges
3. `JobTracker` - 18 edges
4. `compilerOptions` - 17 edges
5. `TagSearchService` - 14 edges
6. `TrendService` - 14 edges
7. `TagCorrelationGraph()` - 13 edges
8. `Tag Co-occurrence Graph 실데이터 연동 — 설계` - 12 edges
9. `upload_video()` - 11 edges
10. `get_s3_client()` - 11 edges

## Surprising Connections (you probably didn't know these)
- `Vault-Data vs Vault-Data-Deploy Duplication Trap` --semantically_similar_to--> `NEXT_PUBLIC_* Build-Time Inlining`  [INFERRED] [semantically similar]
  context.md → docs/ENVIRONMENT.md
- `Redis JobTracker Pattern` --shares_data_with--> `Redis Diff and Deploy Workflow`  [INFERRED]
  docs/ARCHITECTURE.md → .github/workflows/redis_deploy.yaml
- `aurora_databricks_db_dump Loading Pipeline` --shares_data_with--> `vitag-airflow-db-dump Build and Push Workflow`  [INFERRED]
  docs/DATABASE.md → .github/workflows/vitag-airflow-db-dump.yaml
- `Next.js Dual-Cluster Deployment` --shares_data_with--> `web_dev_deploy_data Job`  [INFERRED]
  docs/DEPLOYMENT.md → .github/workflows/workflow.yaml
- `Image Tag Build-Skip Behavior` --shares_data_with--> `api_dev_build Job`  [INFERRED]
  docs/DEPLOYMENT.md → .github/workflows/workflow.yaml

## Import Cycles
- None detected.

## Hyperedges (group relationships)
- **REDIS_PASSWORD 1Password Secret Shared Across Workflows** — github_workflows_pluto, github_workflows_redis_deploy, github_workflows_workflow_api_dev_deploy, docs_environment, redis_job_tracker [INFERRED 0.85]
- **NEXT_PUBLIC_* Build-Time Env Inlining Pattern** — next_public_build_time_inlining, github_workflows_workflow_web_dev_build, github_workflows_workflow_web_prod_build, company_k8s_values_dev, company_k8s_values_prod, docs_environment [INFERRED 0.90]
- **Next.js Dual-Cluster (company EKS + data EKS) Deployment Pattern** — nextjs_dual_deployment, github_workflows_workflow_web_dev_deploy, github_workflows_workflow_web_dev_deploy_data, company_k8s_values_dev, docs_deployment [INFERRED 0.90]
- **UACOS-ViTag 연동 4종 (UI 임베드, API 소비, 딥링크, 데이터 공유)** — docs_uacos_integration_ui_embed, docs_uacos_integration_api_consumption, docs_uacos_integration_deep_link, docs_uacos_integration_data_sharing [EXTRACTED 1.00]
- **동일 4개 원시값(N, cA, cB, pair)에서 파생되는 다섯 지표 — 라디오 전환 시 재요청 없음** — docs_superpowers_specs_2026_08_19_tag_cooccurrence_graph_design_metric_count, docs_superpowers_specs_2026_08_19_tag_cooccurrence_graph_design_metric_jaccard, docs_superpowers_specs_2026_08_19_tag_cooccurrence_graph_design_metric_cosine, docs_superpowers_specs_2026_08_19_tag_cooccurrence_graph_design_metric_pmi, docs_superpowers_specs_2026_08_19_tag_cooccurrence_graph_design_metric_confidence [EXTRACTED 1.00]
- **fastapi-app Helm 차트 — Chart/values/deployment/service/ingress/hpa/pvc가 함께 배포 단위를 구성** — k8s_charts_fastapi_app_chart, k8s_charts_fastapi_app_values, k8s_charts_fastapi_app_templates_deployment, k8s_charts_fastapi_app_templates_service, k8s_charts_fastapi_app_templates_ingress, k8s_charts_fastapi_app_templates_hpa, k8s_charts_fastapi_app_templates_pvc [EXTRACTED 1.00]
- **Dev environment: nextjs + fastapi + redis values wired by env vars** — k8s_values_nextjs_app_values_dev, k8s_values_fastapi_app_values_dev, k8s_values_redis_values_dev [INFERRED 0.85]
- **Two competing nextjs prod values files; only one is actually applied** — k8s_values_nextjs_app_values_prod, company_k8s_values_prod, knowledge_3_insight_values_prod_dual_files_issue [INFERRED 0.85]
- **nextjs-app Helm chart: deployment + service + ingress + values work as one template set** — k8s_charts_nextjs_app_templates_deployment, k8s_charts_nextjs_app_templates_service, k8s_charts_nextjs_app_templates_ingress, k8s_charts_nextjs_app_values [INFERRED 0.95]

## Communities (140 total, 74 thin omitted)

### Community 0 - "태그 탐색기 UI"
Cohesion: 0.06
Nodes (50): TableauViz, TableauViz, menuConfig, MenuType, AnalysisOptions(), AnalysisOptionsProps, CASINO_COLUMNS, CASUAL_COLUMNS (+42 more)

### Community 1 - "태그 연관 그래프 · API 클라이언트"
Cohesion: 0.06
Nodes (58): Home(), WordCloud, HotKeywordsProps, SortDropdownProps, Props, TagCorrelationAnalysis(), TagCorrelationGraph(), Props (+50 more)

### Community 2 - "공용 UI 프리미티브"
Cohesion: 0.07
Nodes (35): Navbar(), Alert(), AlertDescription(), AlertTitle(), alertVariants, Checkbox(), DialogContent(), DialogDescription() (+27 more)

### Community 3 - "크리에이티브 갤러리 검색·필터"
Cohesion: 0.08
Nodes (41): CreativeGalleryContent(), INITIAL_FILTERS, isSortOption(), CreativeFilters(), CreativeFiltersProps, FilterState, INITIAL_FILTERS, shouldDropUp() (+33 more)

### Community 4 - "영상 태그 검색 서비스"
Cohesion: 0.06
Nodes (33): get_available_genres_api(), get_available_tag_categories_api(), AsyncSession, get, API endpoints for tag search video functionality., Search videos based on tag queries and filters., Get list of available genres for filtering., Get list of available tag categories. (+25 more)

### Community 5 - "태그 추출 화면·진행 표시"
Cohesion: 0.10
Nodes (29): FileStatus, FileProgressDisplay(), FileProgressDisplayProps, FileStatus, FileUploadCards(), FileUploadCardsProps, Window, TagHistory (+21 more)

### Community 6 - "FastAPI 앱 진입점·시간 유틸"
Cohesion: 0.06
Nodes (38): exception_handler, on_event, scheduled_job, StarletteHTTPException, general_exception_handler(), http_exception_handler(), Exception, Request (+30 more)

### Community 7 - "태그 키워드 조회 서비스"
Cohesion: 0.08
Nodes (32): TagCategoryResponse, TagValueResponse, get_all_tag_categories_with_values_api(), get_chart_data_by_category_api(), get_tag_categories_api(), get_tag_correlation_api(), get_tag_detail_with_creatives_api(), get_tag_pair_creatives_api() (+24 more)

### Community 8 - "프론트엔드 빌드 의존성"
Cohesion: 0.05
Nodes (38): eslint, eslint-config-next, @eslint/eslintrc, tailwindcss, @tailwindcss/postcss, tw-animate-css, @types/jspdf, @types/node (+30 more)

### Community 9 - "히스토리 화면·한글 폰트 등록"
Cohesion: 0.09
Nodes (31): jspdf, jspdf, xlsx, History(), INITIAL_FILTERS, TagExtraction(), HistoryCardGrid, HistoryCardGridProps (+23 more)

### Community 10 - "설계·계획 문서와 Helm 차트"
Cohesion: 0.08
Nodes (35): docs/archive README, 문서 수명 관리 — docs/ 루트는 현재 참인 문서만, 작업 로그는 archive/YYYY-MM으로, ViTag 레포 문서 기반 구축 Implementation Plan, Tag Co-occurrence Graph 실데이터 연동 Implementation Plan, 카테고리 다중선택 필터 — 백엔드 categories 파라미터로 선택 카테고리 내 재랭킹, 링크 없음 안내 문구 — 카테고리 1개 선택 시 구조적으로 0건인 경우와 구분, 힘 파라미터 노드 반지름 비례 교정 + spacing 배율 슬라이더, 링크 밀도 슬라이더 — 백분위 기반 topLinksByValue, 노드는 유지하고 링크만 필터 (+27 more)

### Community 11 - "S3 업로드·썸네일 생성"
Cohesion: 0.10
Nodes (28): BinaryIO, UploadFile, Upload video file to S3 and return filename and S3 URL., upload_video(), copy_file_to_history(), copy_file_to_history_with_filename(), download_file(), generate_presigned_url() (+20 more)

### Community 12 - "TypeScript 컴파일 설정"
Cohesion: 0.06
Nodes (30): dom, dom.iterable, esnext, next-env.d.ts, .next/types/**/*.ts, node_modules, node_modules/@types, ./src/types (+22 more)

### Community 13 - "태그 상관 서비스·캐시"
Cohesion: 0.12
Nodes (20): date_type, cache_get(), cache_key(), cache_set(), _get_client(), Any, Async Redis cache for expensive aggregate queries. tag_extract.py의 JobTracker와…, Get a Redis client from the shared async pool. (+12 more)

### Community 14 - "Redis 작업 추적기(JobTracker)"
Cohesion: 0.13
Nodes (17): get_extraction_status(), JobTracker, Any, Generate Redis key for job time., Create a new job in Redis., Mark job as completed in Redis., Mark job as failed in Redis., Get job data from Redis. (+9 more)

### Community 15 - "레포 문서 지도"
Cohesion: 0.14
Nodes (23): No Test Suite Policy, router.py try/except Registration Pattern, Tableau Embed Integration, Tag Analysis Query Flow, Tag Extraction Data Flow, tag_history Table (vitag_tag_history), src/lib/api.ts (12 Functions), CreativeFilters.tsx Component (+15 more)

### Community 16 - "태그 추출 엔드포인트·Lambda 호출"
Cohesion: 0.11
Nodes (25): AbstractEventLoop, post, Redis, download_drive_video(), extract_tags(), get_saved_video(), get_thumbnail(), process_video_analysis_lambda() (+17 more)

### Community 17 - "Google Drive 수집"
Cohesion: 0.11
Nodes (24): BytesIO, uuid, authenticate_drive(), download_and_save_video(), download_video_stream(), extract_folder_id(), find_deepest_folder_with_videos(), generate_download_url() (+16 more)

### Community 18 - "태그 추출 스키마"
Cohesion: 0.13
Nodes (21): AnalysisResult, DriveVideoRequest, FolderInfo, FolderListResponse, BaseModel, Tag extraction schemas for request/response validation., Google Drive video request schema., S3 folder request schema. (+13 more)

### Community 19 - "크리에이티브 카드·상세 모달"
Cohesion: 0.16
Nodes (13): AdDetailModal(), AdDetailModalProps, CreativeCard(), CreativeCardProps, CreativeGrid(), CreativeGridProps, ScrollArea(), ScrollBar() (+5 more)

### Community 20 - "환경별 Helm values"
Cohesion: 0.17
Nodes (20): Nextjs App Deployment Template, Nextjs App Ingress Template, Nextjs App Service Template, Nextjs App Helm Chart Default Values, FastAPI App Dev Values ([S3 IAM 역할]), FastAPI App Prod Values ([S3 IAM 역할]), Nextjs App Dev Values ([사내 도메인]), Nextjs App Prod Values ([사내 도메인], believed unused by real deploy) (+12 more)

### Community 21 - "태그 히스토리 서비스"
Cohesion: 0.14
Nodes (14): TagHistory, convert_json_to_markdown(), Any, AsyncSession, PaginationParams, History management service for Aurora DB., Get tag history by UUID., Delete tag history by UUID. (+6 more)

### Community 22 - "배포 함정 기록(빌드타임 인라인·이미지 스킵)"
Cohesion: 0.22
Nodes (15): company-k8s values.dev.yaml, Dead Environment Variables (LLM_AGENT etc.), check_web_log Job, Redis Diff and Deploy Workflow, web_dev_build Job, web_dev_build_data Job, web_dev_deploy Job, web_dev_deploy_data Job (+7 more)

### Community 23 - "크리에이티브 스키마"
Cohesion: 0.15
Nodes (17): Config, Creative, CreativeBase, CreativeFilters, CreativeListResponse, DimensionResponse, PaginationParams, BaseModel (+9 more)

### Community 24 - "shadcn 컴포넌트 설정"
Cohesion: 0.11
Nodes (17): aliases, components, hooks, lib, ui, utils, iconLibrary, rsc (+9 more)

### Community 25 - "영상 검색 화면·페이지네이션"
Cohesion: 0.22
Nodes (14): PaginationControlsProps, DropdownMenu(), DropdownMenuRadioGroup(), DropdownMenuTrigger(), Input(), Pagination(), PaginationContent, PaginationEllipsis() (+6 more)

### Community 26 - "트렌드 지표 서비스"
Cohesion: 0.18
Nodes (10): Config, Schema for monthly trend metrics., Schema for weekly trend metrics., TagMonthlyTrendsMetricsSchema, TagWeeklyTrendsMetricsSchema, AsyncSession, 특정 태그에 대한 관련 썸네일 URL들을 랜덤하게 가져옵니다., 썸네일 URL들에 매핑되는 크리에이티브 URL들을 가져옵니다. (+2 more)

### Community 27 - "태그 히스토리 스키마"
Cohesion: 0.17
Nodes (15): Config, PaginationParams, BaseModel, Pydantic schemas for tag history., Base schema for tag history., Schema for creating tag history., Schema for tag history response., Schema for paginated tag history list response. (+7 more)

### Community 28 - "크리에이티브 서비스"
Cohesion: 0.15
Nodes (12): CreativeFilters, SortOption, AdCreativeDetails, Base, Model for vitag_ad_creative_details table., CreativeService, AsyncSession, PaginationParams (+4 more)

### Community 29 - "태그 상관 스키마"
Cohesion: 0.20
Nodes (14): CalculationWindow, CorrelationLink, CorrelationNode, PairCreative, PeriodNodeCount, PeriodSlice, BaseModel, Pydantic schemas for the tag co-occurrence graph. 이 계열 엔드포인트는 UACOS의 외부 소비 계약이… (+6 more)

### Community 30 - "운영 배포 잡 · prod values 이중화"
Cohesion: 0.19
Nodes (14): company-k8s values.prod.yaml, api_prod_build Job, api_prod_deploy Job, api_prod_diff Job, static_checks Job, web_prod_build Job, web_prod_build_data Job, web_prod_deploy Job (+6 more)

### Community 31 - "파일명 안전 변환·CloudFront URL"
Cohesion: 0.15
Nodes (12): slugify, build_safe_cloudfront_history_url(), build_safe_cloudfront_temp_url(), build_safe_s3_temp_url(), Return S3 temp URL with ASCII-safe filename (for URL building only)., Return CloudFront history URL with ASCII-safe filename (for URL building only)., Return CloudFront temp URL with ASCII-safe filename (for URL building only)., ascii_safe_filename() (+4 more)

### Community 32 - "SQLAlchemy 모델"
Cohesion: 0.22
Nodes (7): SQLAlchemy models for creative gallery., Base, SQLAlchemy models for hot keyword., TagAllCreativeKeywords, TagExplorerRankedData, TagMonthlyTrendsMetrics, TagWeeklyTrendsMetrics

### Community 33 - "대시보드 사이드바"
Cohesion: 0.19
Nodes (11): categoryIcons, DashboardMenuItem(), DashboardMenuItemProps, DashboardSidebar(), DashboardSidebarProps, DashboardSidebarProvider(), DashboardSidebarProviderProps, SidebarContext (+3 more)

### Community 34 - "UACOS 연동 계약·검색 보안 결함"
Cohesion: 0.24
Nodes (11): Creative Gallery 검색 개선 Implementation Plan, Creative Gallery 검색 개선 설계, 이중 입력 제한 — 프론트 화이트리스트 + 백엔드 문자 제거가 검색을 막음, 한/영 자판 오타 자동 변환(hangulToLatin) — 0건일 때만 재검색, 하이라이트 결함 — 정규식 주입 + dangerouslySetInnerHTML XSS, 결합 생성 컬럼(search_text) + 트라이그램 GIN — 다중 컬럼·다중 토큰 검색, API 소비 계약(예정) — TagInsight/ThemeKeywordAnalysis mock, 데이터 공유 — vitag_prod_sensortower_ad_creative_details 미러링 (+3 more)

### Community 35 - "프론트엔드 런타임 의존성"
Cohesion: 0.18
Nodes (11): chart.js, date-fns, lucide-react, @next/third-parties, @radix-ui/react-dropdown-menu, dependencies, chart.js, date-fns (+3 more)

### Community 36 - "Aurora 덤프 적재 배치"
Cohesion: 0.31
Nodes (10): Namespace, _column_list(), _copy_csv_into_table(), _fetch_aurora_password(), _list_csv_keys(), main(), parse_args(), vitag-airflow-db-dump entrypoint. Streams CSV objects under an S3 prefix into a… (+2 more)

### Community 37 - "Lambda 호출 서비스"
Cohesion: 0.18
Nodes (8): DriveVideoPayload, BaseModel, LambdaService, Any, Invoke Lambda function via HTTP POST request for tag extraction. Args: job_id:…, MaxFileSizeExceeded, Exception, Raised when a file exceeds the maximum allowed size while streaming upload.

### Community 38 - "규칙 파일(5법칙·시크릿·커밋)"
Cohesion: 0.25
Nodes (7): Absolute Rules (5 Laws), Atomic Commits Rule, PR Size Convention (Hotfix/Small/Medium/Large), NEXT_PUBLIC_ Secret Exposure Rule, Pre-commit Configuration, black Hook, ruff Hook

### Community 39 - "Aurora 스키마·적재 파이프라인"
Cohesion: 0.42
Nodes (8): sensortower_ad_creative_details Table, tag_all_creative_keywords Table, tag_explorer_ranked_data Table, tag_monthly_trends_metrics Table, tag_weekly_trends_metrics Table, Generated Column COPY Limitation, vitag-airflow-db-dump Build and Push Workflow, aurora_databricks_db_dump Loading Pipeline

### Community 40 - "크리에이티브 API"
Cohesion: 0.31
Nodes (8): get_creatives(), get_dimensions(), AsyncSession, datetime, get, Creative gallery related API endpoints., Get filtered and paginated creatives., Get all unique dimensions from the database.

### Community 41 - "트렌드 API"
Cohesion: 0.39
Nodes (7): get_database_info(), get_monthly_trends_api(), get_weekly_trends_api(), AsyncSession, get, Get monthly trend metrics., Get weekly trend metrics.

### Community 42 - "DB 연결·시크릿 조회"
Cohesion: 0.29
Nodes (7): get_database(), get_database_password(), get_database_url(), Database connection and session management., Get database password from AWS Secrets Manager., Create database URL for async connection., Dependency for getting database session.

### Community 43 - "트렌드 스키마"
Cohesion: 0.36
Nodes (6): Pydantic schemas for API request and response validation., BaseModel, Schema for weekly trend list response., Schema for monthly trend list response., TagMonthlyTrendsListResponse, TagWeeklyTrendsListResponse

### Community 44 - "dev 배포 잡"
Cohesion: 0.29
Nodes (7): check_api_log Job, dev_check_k8s_api Job, redis_dev_deploy Job, redis_dev_diff Job, api_dev_build Job, api_dev_deploy Job, api_dev_diff Job

### Community 45 - "히스토리 API"
Cohesion: 0.33
Nodes (6): get_tag_history(), AsyncSession, datetime, get, History related API endpoints using Aurora DB., Fetch paginated and filtered tag history from Aurora DB.

### Community 46 - "헬스체크·페이지 라우트"
Cohesion: 0.33
Nodes (6): health_check(), index_page(), get, Request, Page routing endpoints., Health check endpoint for Kubernetes probes.

### Community 47 - "Next.js 루트 레이아웃"
Cohesion: 0.33
Nodes (4): geistMono, geistSans, metadata, Toaster()

### Community 48 - "토글 컴포넌트"
Cohesion: 0.43
Nodes (5): ToggleGroup(), ToggleGroupContext, ToggleGroupItem(), Toggle(), toggleVariants

### Community 49 - "Tableau 임베드·토큰"
Cohesion: 0.47
Nodes (4): TableauViz(), TableauVizProps, TokenStore, useTokenStore

### Community 50 - "태그 히스토리 모델"
Cohesion: 0.40
Nodes (4): Base, SQLAlchemy models for tag history., Model for vitag_tag_history table., TagHistory

### Community 51 - "ESLint 설정"
Cohesion: 0.40
Nodes (4): compat, __dirname, eslintConfig, __filename

### Community 52 - "워드클라우드 차트 타입"
Cohesion: 0.40
Nodes (4): chart.js, chartjs-chart-wordcloud, WordCloudController, WordElement

### Community 53 - "Tableau 타입 선언"
Cohesion: 0.40
Nodes (4): IntrinsicElements, JSX, react, VizParameter

## Ambiguous Edges - Review These
- `nextjs-app Chart.yaml` → `prod 배포 호스트 이원화 — k8s/values vs company-k8s/values 불일치`  [AMBIGUOUS]
  docs/superpowers/specs/2026-07-30-repo-documentation-design.md · relation: conceptually_related_to
- `nextjs-app Chart.yaml` → `values.yaml 주석이 'nextjs-app' 기준으로 복사됨 — fastapi-app 차트와 불일치(포트 3000 등)`  [AMBIGUOUS]
  k8s/charts/fastapi-app/values.yaml · relation: conceptually_related_to
- `FastAPI App Prod Values ([S3 IAM 역할])` → `Redis Prod Values (bitnamilegacy/redis standalone)`  [AMBIGUOUS]
  k8s/values/fastapi-app/values.prod.yaml · relation: shares_data_with

## Knowledge Gaps
- **245 isolated node(s):** `Config`, `Config`, `Config`, `$schema`, `style` (+240 more)
  These have ≤1 connection - possible missing edges or undocumented components.
- **74 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **What is the exact relationship between `nextjs-app Chart.yaml` and `prod 배포 호스트 이원화 — k8s/values vs company-k8s/values 불일치`?**
  _Edge tagged AMBIGUOUS (relation: conceptually_related_to) - confidence is low._
- **What is the exact relationship between `nextjs-app Chart.yaml` and `values.yaml 주석이 'nextjs-app' 기준으로 복사됨 — fastapi-app 차트와 불일치(포트 3000 등)`?**
  _Edge tagged AMBIGUOUS (relation: conceptually_related_to) - confidence is low._
- **What is the exact relationship between `FastAPI App Prod Values ([S3 IAM 역할])` and `Redis Prod Values (bitnamilegacy/redis standalone)`?**
  _Edge tagged AMBIGUOUS (relation: shares_data_with) - confidence is low._
- **Why does `dependencies` connect `프론트엔드 런타임 의존성` to `프론트엔드 빌드 의존성`, `히스토리 화면·한글 폰트 등록`, `Google Drive 수집`, `파일명 안전 변환·CloudFront URL`, `chartjs-chart-wordcloud`, `chartjs-plugin-zoom`, `class-variance-authority`, `clsx`, `d3`, `@gaia-portal/gnb`, `@gaia-ui/core`, `hangul-romanization`, `jose`, `next`, `next-themes`, `@radix-ui/react-accordion`, `@radix-ui/react-checkbox`, `@radix-ui/react-collapsible`, `@radix-ui/react-dialog`, `@radix-ui/react-label`, `@radix-ui/react-navigation-menu`, `@radix-ui/react-popover`, `@radix-ui/react-progress`, `@radix-ui/react-scroll-area`, `@radix-ui/react-select`, `@radix-ui/react-separator`, `@radix-ui/react-slider`, `@radix-ui/react-slot`, `@radix-ui/react-switch`, `@radix-ui/react-toggle`, `@radix-ui/react-toggle-group`, `react`, `react-day-picker`, `react-dom`, `server-only`, `sonner`, `@tableau/embedding-api`, `tailwind-merge`, `@types/d3`, `zustand`?**
  _High betweenness centrality (0.347) - this node is a cross-community bridge._
- **Why does `uuid` connect `Google Drive 수집` to `태그 추출 엔드포인트·Lambda 호출`?**
  _High betweenness centrality (0.280) - this node is a cross-community bridge._
- **Why does `uuid` connect `Google Drive 수집` to `프론트엔드 런타임 의존성`?**
  _High betweenness centrality (0.273) - this node is a cross-community bridge._
- **Are the 4 inferred relationships involving `JobTracker` (e.g. with `UnifiedTagExtractRequest` and `TagHistoryService`) actually correct?**
  _`JobTracker` has 4 INFERRED edges - model-reasoned connections that need verification._