# Graph Report - ../corpus  (2026-09-27)

## Corpus Check
- 151 files · ~476,808 words
- Verdict: corpus is large enough that graph structure adds value.

## Summary
- 937 nodes · 1824 edges · 59 communities (55 shown, 4 thin omitted)
- Extraction: 91% EXTRACTED · 9% INFERRED · 0% AMBIGUOUS · INFERRED: 156 edges (avg confidence: 0.85)
- Token cost: 695,490 input · 0 output

## Community Hubs (Navigation)
- 런타임 의존성 (AI·FFmpeg SDK)
- 파일 업로드 UI
- 빌드·타입 의존성
- 장면 설명 편집·diff
- 서버 영상 처리 (FFmpeg 유틸)
- 타임라인 에디터·생성 모달
- 배경제거 가이드·구현 (imageUtils)
- Prompts 화면 컴포넌트
- Chat 기능·우선순위 재분배 기획
- 서버 API 핸들러 (Gemini·Veo3)
- TypeScript 설정
- 백엔드 아키텍처 문서
- 에셋 추출 패널
- Video to Asset·추출 프롬프트
- Diff·다이얼로그 UI
- 사이드바 UI 프리미티브
- 세션 저장 (IndexedDB)
- 스크립트 클립·입력 UI
- 앱 내비게이션 (SNB)
- Breadcrumb·리사이즈 패널
- 방향 확정 Sync (Phase1→2)
- Milestone 1 유저 플로우
- 핵심 데이터 모델 (Scene·18필드)
- 사용자 흐름 문서 (StepWizard)
- 에셋 3종 스펙 (배경제거 공통)
- 타임라인 UAC 피드백 스펙
- 프롬프트 스키마 개선 (13→18필드)
- Milestone II·1Pager
- Global Replacement 요구·A/B 피드백
- Upload·Split QA
- 스크린샷: 메인 화면
- 코드 수정 요청 (네이밍·인덱스 정합)
- Kling 영상 생성 리서치
- 스크린샷: 추출 결과
- Sheet UI
- Milestone 1 KPI·Chat 편집
- Upload·Split 스펙 (API 흐름)
- 작업 이력 (Proxy·리팩토링)
- 스크린샷: 병합 결과
- 스크린샷: 분할 결과
- Vercel 배포 설정
- Nano Banana 에셋 추출 PoC
- ViTag 연동·에셋 교체 시나리오
- 1월 회의록·일정
- 스크린샷: 재생성 결과
- Split Scene 스펙 (세그먼트 편집)
- 앱 진입점
- Timeline·Finalization 스펙
- Veo 3.1 vs Sora 2 비교
- Vercel 설치 스크립트
- 프레임 단위 편집 스펙
- A안(SNB) 채택·배포 환경
- Vite 환경 타입
- 영상 생성 도구 리서치
- HTML 진입점
- Prompt Research (빈 문서)
- Video Generate Test Case (빈 문서)

## God Nodes (most connected - your core abstractions)
1. `cn()` - 90 edges
2. `useSceneContext()` - 32 edges
3. `SceneStealer PoC Backend Architecture` - 24 edges
4. `Button()` - 22 edges
5. `SceneStealer PoC Codebase Analysis` - 21 edges
6. `react` - 20 edges
7. `SceneStealer PoC User Action Flow` - 17 edges
8. `Scene` - 16 edges
9. `compilerOptions` - 16 edges
10. `SceneStealer V2 - 1. Upload Scene` - 16 edges

## Surprising Connections (you probably didn't know these)
- `Global Replace (applyInstruction / applyBulkReplace / diff)` --semantically_similar_to--> `Chat-based Contextual Edit Pipeline`  [INFERRED] [semantically similar]
  poc/docs/USER_ACTION_FLOW.md → vault/00-Overview/SceneStealer Milestone 1.md
- `Time Length 4/6/8s toggle` --conceptually_related_to--> `Async Veo3 request_id Polling`  [INFERRED]
  vault/00-Overview/SceneStealer V2 - 1Pager.md → poc/docs/BACKEND_ARCHITECTURE.md
- `SceneStealer Milestone II Function Lists` --references--> `vercel.json rewrites`  [INFERRED]
  vault/00-Overview/[SceneStealer] Milestone II - Function Lists + Ideas.md → poc/docs/BACKEND_ARCHITECTURE.md
- `SceneStealer Milestone II Function Lists` --references--> `Global Replace (applyInstruction / applyBulkReplace / diff)`  [INFERRED]
  vault/00-Overview/[SceneStealer] Milestone II - Function Lists + Ideas.md → poc/docs/USER_ACTION_FLOW.md
- `Asset Decomposition PoC` --conceptually_related_to--> `Asset Extractor feature`  [INFERRED]
  vault/00-Overview/SceneStealer V2 - 1Pager.md → poc/README.md

## Import Cycles
- None detected.

## Hyperedges (group relationships)
- **Upload->Timestamp->Split->Describe->Veo3->Merge pipeline** — poc_docs_backend_architecture_gemini_timestamp_ts, poc_docs_backend_architecture_video_ts, poc_docs_backend_architecture_gemini_extract_ts, poc_docs_backend_architecture_fal_ts, poc_docs_user_action_flow_upload_scene_step, poc_docs_user_action_flow_timeline_editor_step, poc_docs_user_action_flow_finalization_step [EXTRACTED 1.00]
- **Asset extraction background removal flow** — poc_docs_backend_architecture_extract_assets_ts, poc_docs_background_removal_spec_chroma_key_green_background, poc_docs_background_removal_spec_edge_fringe_cleanup, poc_docs_background_removal_spec_connected_components_separation, poc_docs_background_removal_spec_image_to_asset, poc_docs_background_removal_spec_video_to_asset, poc_docs_background_removal_spec_asset_regenerate [EXTRACTED 1.00]
- **Serverless resilience patterns** — poc_docs_backend_architecture_soft_fail_pattern, poc_docs_backend_architecture_hard_fail_pattern, poc_docs_backend_architecture_two_stage_fallback, poc_docs_backend_architecture_async_veo3_polling, poc_docs_backend_architecture_serverless_constraints [INFERRED 0.85]
- **에셋 추출 배경제거 공통 흐름** — vault_02_product_spec_scenestealer_v2_5_image_to_asset_extract_objects_from_images, vault_02_product_spec_scenestealer_v2_6_video_to_asset_frame_capture_extract, vault_02_product_spec_scenestealer_v2_7_asset_re_generate_regenerate_with_custom_prompt, vault_02_product_spec_scenestealer_v2_99_asset_extractor_background_removal_pipeline, vault_02_product_spec_scenestealer_v2_99_asset_extractor_connected_components_separation [EXTRACTED 1.00]
- **Timeline Editor UAC 피드백 기능군** — vault_02_product_spec_scenestealer_v2_3_1_add_uac_feedback_frame_frame_level_editing, vault_02_product_spec_scenestealer_v2_3_2_add_uac_feedback_short_cut_keyboard_shortcuts, vault_02_product_spec_scenestealer_v2_3_3_add_uac_feedback_speed_function_per_scene_playback_speed, vault_02_product_spec_scenestealer_v2_3_4_add_uac_feedback_mass_produce_scenes_track_collapse_expand, vault_02_product_spec_scenestealer_v2_3_0_track_context_menu, vault_02_product_spec_scenestealer_v2_3_timeline_editor_timeline_todo_11_tasks [EXTRACTED 1.00]
- **씬 병렬 배열 정합성 (scenes/timestamps/stealingStates)** — vault_01_planning_code_reorderscenes, vault_01_planning_code_deletescene, vault_01_planning_code_stealingstates, vault_01_planning_code_scene_array_index_invariant, vault_02_product_spec_scenestealer_v2_1_upload_scene_scene_drag_reorder, vault_02_product_spec_scenestealer_v2_1_upload_scene_scene_delete [INFERRED 0.85]
- **씬스틸러 프롬프트 스키마 진화 (설문→1차 개선→코드 반영)** — vault_03_prompt_design_phase2_prompt_survey_result_prompt_survey, vault_03_prompt_design_1_prompt_schema_revision_v1, vault_03_prompt_design_1_style_field, vault_03_prompt_design_1_audio_elements_split, vault_03_prompt_design_phase2_prompt_survey_result_description_types_18_fields, vault_03_prompt_design_phase2_prompt_survey_result_gemini_extract_ts [INFERRED 0.85]
- **Global Replacement 기능과 LLM 재작성 요구** — vault_03_prompt_design_phase2_prompt_survey_result_global_replacement, vault_05_qa_qa_checklist_2_1_global_replacement_local_command_parsing, vault_05_qa_qa_checklist_2_1_global_replacement_diff_modal, vault_05_qa_a_b_test_feedback_replace_limitations, vault_03_prompt_design_phase2_prompt_survey_result_intent_based_llm_rewrite, vault_04_research_video_to_video_workflow_outdated_regenerate_prompts_bulk_replace [INFERRED 0.85]
- **에셋 추출 파이프라인 (캡처→Nano Banana→rembg)** — vault_04_research_custom_nano_banana_build_app_capture_to_asset_flow, vault_04_research_custom_nano_banana_build_app_nano_banana, vault_04_research_custom_nano_banana_build_app_rembg, vault_04_research_poc_asset_decomposition, vault_99_meeting_archive_prep_scene_stealer_meeting_for_milestoneii_asset_decomposition, vault_04_research_video_to_video_workflow_outdated_assets_extractor_step [INFERRED 0.85]
- **Extract -> Edit -> Regenerate scene flow** — poc_public_assets_extract_result_scene_extraction, poc_public_assets_extract_result_scene_description, poc_public_assets_extract_result_regenerate_scene, poc_public_assets_extract_result_veo3 [INFERRED 0.75]
- **Upload -> Steal -> Edit -> Regenerate flow** — poc_public_assets_main_page_file_upload_dropzone, poc_public_assets_main_page_start_scene_stealing, poc_public_assets_main_page_scene_prompt_sections, poc_public_assets_main_page_regenerate_scene, poc_public_assets_main_page_veo3 [INFERRED 0.75]
- **Scene select -> merge -> preview -> download flow** — poc_public_assets_merge_result_scene_timeline, poc_public_assets_merge_result_merge_scenes, poc_public_assets_merge_result_merged_video, poc_public_assets_merge_result_download_scenes [INFERRED 0.75]
- **Structured-prompt scene regeneration flow** — poc_public_assets_regenerate_result_scene_description, poc_public_assets_regenerate_result_character_description, poc_public_assets_regenerate_result_atmosphere, poc_public_assets_regenerate_result_regenerate_scene, poc_public_assets_regenerate_result_veo3 [INFERRED 0.85]
- **Split -> Extract -> Edit -> Regenerate Scene Flow** — poc_public_assets_split_result_scene_splitting, poc_public_assets_split_result_scene_description_schema, poc_public_assets_split_result_scene_editor, poc_public_assets_split_result_regenerate_scene, poc_public_assets_split_result_veo3 [INFERRED 0.75]

## Communities (59 total, 4 thin omitted)

### Community 0 - "런타임 의존성 (AI·FFmpeg SDK)"
Cohesion: 0.04
Nodes (49): axios, class-variance-authority, clsx, @fal-ai/client, @ffmpeg-installer/ffmpeg, @ffprobe-installer/ffprobe, fluent-ffmpeg, @google/genai (+41 more)

### Community 1 - "파일 업로드 UI"
Cohesion: 0.09
Nodes (43): react, createStore(), Direction, DirectionContext, FileState, FileUploadClear(), FileUploadClearProps, FileUploadContext (+35 more)

### Community 2 - "빌드·타입 의존성"
Cohesion: 0.05
Nodes (37): devDependencies, tailwindcss, @tailwindcss/vite, tw-animate-css, @types/node, @types/react, @types/react-dom, @types/uuid (+29 more)

### Community 3 - "장면 설명 편집·diff"
Cohesion: 0.11
Nodes (25): EXAMPLE_DESCRIPTION, DescriptionDiffContent(), getDiffFields(), TODO: Implement setNewDescriptions functionality if needed, DescriptionDiffViewer(), DescriptionGroup(), DescriptionGroupProps, DescriptionTextarea() (+17 more)

### Community 4 - "서버 영상 처리 (FFmpeg 유틸)"
Cohesion: 0.13
Nodes (32): ensureFfmpegConfigured(), require, AudioClip, calcDuration(), clampNumber(), composeVideo(), convertImageToPng(), downloadFontToFile() (+24 more)

### Community 5 - "타임라인 에디터·생성 모달"
Cohesion: 0.13
Nodes (26): GenerationModal(), GenerationModalProps, ImageOverlayEditorProps, ScriptClipEditor(), emptySegment(), Segment, SplitSelection, TimelineEditor() (+18 more)

### Community 6 - "배경제거 가이드·구현 (imageUtils)"
Cohesion: 0.11
Nodes (30): gemini-3-pro-image-preview, Background Removal Context Guide, analyzeScreenshot(), BackgroundRemovalDemo component, Bagel Maker (origin project), base64ToBlob(), refineBackgroundRemoval(), removeBackgroundFromFile() (+22 more)

### Community 7 - "Prompts 화면 컴포넌트"
Cohesion: 0.14
Nodes (20): BulkReplace(), DescriptionEditor(), FileInput(), PromptTextDiffDialog(), SceneCard(), SceneCardProps, SceneEditor(), SceneGrid() (+12 more)

### Community 8 - "Chat 기능·우선순위 재분배 기획"
Cohesion: 0.09
Nodes (31): 우선순위 재분배, 일괄 변경/자동화 기능 (P2), SceneProvider always-on 로그 가드 (NEXT_PUBLIC_DEBUG), 프롬프트 카테고리 추가 (style, Camera Lens, Sound 세분화), 프롬프트 복사/붙여넣기 (P2 Quick Win), 반복 표현 제거 (4k, masterpiece 등), [SceneStealer] New Feature - Chat, /api/smart/preview (plan/preview/apply) (+23 more)

### Community 9 - "서버 API 핸들러 (Gemini·Veo3)"
Cohesion: 0.15
Nodes (21): cors(), handler(), handler(), toFalDuration(), veo3Fast(), fetchGemini(), httpsPost(), isGeminiConfigured() (+13 more)

### Community 10 - "TypeScript 설정"
Cohesion: 0.07
Nodes (27): compilerOptions, allowImportingTsExtensions, allowJs, experimentalDecorators, isolatedModules, jsx, lib, module (+19 more)

### Community 11 - "백엔드 아키텍처 문서"
Cohesion: 0.19
Nodes (25): SceneStealer PoC Backend Architecture, Action-based Routing Pattern, Async Veo3 request_id Polling, _cors.ts CORS helper, Env vars (GEMINI_API_KEY, AI_PROXY_*, FAL_KEY), extract-assets.ts, fal-ai/veo3/fast, fal.ts (Veo3 fast) (+17 more)

### Community 12 - "에셋 추출 패널"
Cohesion: 0.18
Nodes (14): ExtractedAssets1PanelProps, ExtractedAssets2Panel(), ExtractedAssets2PanelProps, GeneratedImagesPanel(), GeneratedImagesPanelProps, ImageToAssetPanel(), ImageToAssetPanelProps, ImageOverlayEditor() (+6 more)

### Community 13 - "Video to Asset·추출 프롬프트"
Cohesion: 0.22
Nodes (12): StyleControlsSectionProps, VideoToAssetPanel(), VideoToAssetPanelProps, EXTRACT_ASSETS_PROMPT, StepWizardAssets(), StepWizardAssetsProps, useAssets1Manager(), useAssets2Manager() (+4 more)

### Community 14 - "Diff·다이얼로그 UI"
Cohesion: 0.21
Nodes (14): DescriptionDiffDialog(), PromptChange, Dialog(), DialogClose(), DialogContent(), DialogDescription(), DialogFooter(), DialogHeader() (+6 more)

### Community 15 - "사이드바 UI 프리미티브"
Cohesion: 0.13
Nodes (17): SidebarContext, SidebarContextProps, SidebarFooter(), SidebarInput(), SidebarMenuAction(), SidebarMenuBadge(), SidebarMenuSkeleton(), SidebarMenuSub() (+9 more)

### Community 16 - "세션 저장 (IndexedDB)"
Cohesion: 0.25
Nodes (16): createSessionActions(), clearAllScenesFromIndexedDB(), deleteSceneFromIndexedDB(), hasScenesInIndexedDB(), loadAllScenesFromIndexedDB(), loadFromIndexedDB(), loadSceneFromIndexedDB(), openDB() (+8 more)

### Community 17 - "스크립트 클립·입력 UI"
Cohesion: 0.17
Nodes (14): OptionSelectorProps, ALIGNMENTS, FONT_FAMILIES, ScriptClipEditorProps, Input(), Select(), SelectContent(), SelectItem() (+6 more)

### Community 18 - "앱 내비게이션 (SNB)"
Cohesion: 0.16
Nodes (14): NavHeader(), Sidebar(), SidebarContent(), SidebarGroup(), SidebarGroupAction(), SidebarGroupContent(), SidebarGroupLabel(), SidebarHeader() (+6 more)

### Community 19 - "Breadcrumb·리사이즈 패널"
Cohesion: 0.20
Nodes (11): BreadcrumbEllipsis(), BreadcrumbItem(), BreadcrumbLink(), BreadcrumbList(), BreadcrumbPage(), BreadcrumbSeparator(), ResizableHandle(), ResizablePanelGroup() (+3 more)

### Community 20 - "방향 확정 Sync (Phase1→2)"
Cohesion: 0.13
Nodes (17): 씬 스틸링 품질 (P1), Toast box 문구 모음, Sync for Scenestealer (Lock the direction), AS-IS(Phase1) vs TO-BE(Phase2) 워크플로우 비교, FFmpeg (fluent-ffmpeg), Kling O1, Logging Management (Splunk, Prompt/Global Replace 로깅), 모델 스택 (Fal.AI Veo 3.1 / Kling O1 / Gemini 3 Pro Image Preview) (+9 more)

### Community 21 - "Milestone 1 유저 플로우"
Cohesion: 0.16
Nodes (17): 프롬프트 Copy/Paste 기능 (#atmosphere 형식), Assets 1/2 (Asset Extractor), Video to Video Workflow (Outdated), Editor Workspace / Timeline 편집, Finalization (Original vs Merged, MP4/ZIP 다운로드), Regenerate Options > Prompts (Bulk Replace), SNB 6단계 유저 플로우 (Upload→Timeline→Prompts→Assets→Regenerate&Review), Upload Scene 단계 (+9 more)

### Community 22 - "핵심 데이터 모델 (Scene·18필드)"
Cohesion: 0.22
Nodes (16): 18-field Scene Description, SceneStealer PoC Codebase Analysis, Description type (18 fields), GeneratedVersion type, Progress enum, scene-context.tsx (SceneProvider), Scene type (src/types/scene.ts), SceneAsset type (+8 more)

### Community 23 - "사용자 흐름 문서 (StepWizard)"
Cohesion: 0.20
Nodes (15): StepWizard component, TimelineEditor (timeline-editor.tsx), SceneStealer PoC User Action Flow, Compare Mode & Version Selection, Step 7: Finalization, Global Replace (applyInstruction / applyBulkReplace / diff), scene-stealer:navigate-step event, Overlay Management (audio/image/script) (+7 more)

### Community 24 - "에셋 3종 스펙 (배경제거 공통)"
Cohesion: 0.26
Nodes (15): gemini-3-pro-image-preview, Workflow 2: Image to Video (에셋 추출), SceneStealer V2 - 5. Image to Asset, Extract Objects from Images, SceneStealer V2 - 6. Video to Asset, 비디오 프레임 캡처 → 에셋 생성, SceneStealer V2 - 7. Asset Re-generate, Regenerate with Custom Prompt (+7 more)

### Community 25 - "타임라인 UAC 피드백 스펙"
Cohesion: 0.17
Nodes (15): SceneStealer V2 - 3-0. 트랙별 우클릭 메뉴, Ripple Delete, 트랙별 우클릭 메뉴, SceneStealer V2 - 3-2. UAC Feedback (Short-cut), 키보드 단축키 체계 (숫자키/Space/J·K·L/C/Del), 씬 넘버 배지, Undo/Redo (최대 50 히스토리), SceneStealer V2 - 3-3. UAC Feedback (Speed function) (+7 more)

### Community 26 - "프롬프트 스키마 개선 (13→18필드)"
Cohesion: 0.25
Nodes (15): Audio Elements 분리 (Dialogue/BGM/Sound Effects), Camera Lens & Settings 필드, 1차 프롬프트 개선 결과, 1차 프롬프트 스키마 개선, gazeDirection·keyColors 필드 제거, Style 프롬프트 필드, types/description.ts 18필드 스키마, [Phase2] Prompt Survey Result (+7 more)

### Community 27 - "Milestone II·1Pager"
Cohesion: 0.24
Nodes (14): SceneStealer Milestone II Function Lists, Cut tool (shortcut C), Extract Objects (Gemini Vision Objects), Logging events & funnel, SceneStealer V2 1Pager, Asset Decomposition PoC, Img -> Video Pipeline, Competitor video -> structure analysis -> rebuild with our assets -> one-click generate (+6 more)

### Community 28 - "Global Replacement 요구·A/B 피드백"
Cohesion: 0.20
Nodes (14): Global Replacement 기능, 의도 기반 LLM 일괄 프롬프트 재작성, Phase2 프롬프트 사용자 설문, 전체 공용 캐릭터/배경 프롬프트, A-B Test Feedback, 정책 위반 자동 필터링/우회, 단어 치환 방식의 한계, 타임라인 단축키 요구 (Undo/Redo/Save/Cut 등, P2) (+6 more)

### Community 29 - "Upload·Split QA"
Cohesion: 0.19
Nodes (13): 씬 분할 기능 문제 (자동 분할 실패/수동 분할 불편), Veo3 4/6/8초 길이 제약, QA Checklist - 1-1. Split Scene, Split 후 Extract Prompts 연계, Split Scene 화면 (수동 구간 분할), AI - Auto Split (타임스탬프 추출 + FFmpeg 분할), QA Checklist - 1. Upload Scene, Fal.ai 업로드 (+5 more)

### Community 30 - "스크린샷: 메인 화면"
Cohesion: 0.21
Nodes (12): Scene Stealer Main Page Screenshot, Aspect Ratio Selector (16:9), Drag & Drop File Upload, Regenerate Scene Action, Scene Editor Tab, Scene Preview Tab, Structured Scene Prompt Sections, Scene Stealer (AI Jam 2025) (+4 more)

### Community 31 - "코드 수정 요청 (네이밍·인덱스 정합)"
Cohesion: 0.21
Nodes (12): Code 수정 요청사항, API 라우팅 폴더 기준 (src/app/api 전용, src/pages/api legacy), deleteScene, 축약 없는 네이밍 규칙 (v2v → video-to-video), Gemini API 정식/폴백 엔드포인트 규칙 (401/403에서만 fallback), Hover/Drag/Drop-target 시각화 우선순위, reorderScenes, scenes/timestamps/stealingStates 인덱스 정합성 불변식 (+4 more)

### Community 32 - "Kling 영상 생성 리서치"
Cohesion: 0.24
Nodes (12): Frame-to-video 방식, Prompt Revision 작업, Kling Camera Movement 제어, KLING AI Guide (Video), KLING AI (Kuaishou 비디오 생성 모델), 효과적 비디오 프롬프트 공통 원칙 (구체적 시각 묘사·현재진행형·외형 묘사), Start and End Frames 기능, Kling Text-to-Video 프롬프트 공식 (주체+움직임+장면+카메라/조명/분위기) (+4 more)

### Community 33 - "스크린샷: 추출 결과"
Cohesion: 0.22
Nodes (11): Scene Stealer Extract Result Screenshot, History View, Regenerate Scene Action, Scene Description (Space & Background, Camera Work), Scene Editor, Scene Extraction (async per-scene), Scene Preview, Scene Stealer (AI Jam 2025) (+3 more)

### Community 34 - "Sheet UI"
Cohesion: 0.18
Nodes (7): Sheet(), SheetContent(), SheetDescription(), SheetFooter(), SheetHeader(), SheetOverlay(), SheetTitle()

### Community 35 - "Milestone 1 KPI·Chat 편집"
Cohesion: 0.25
Nodes (11): [Index] SceneStealer, Product KPIs (Scene Detection success, regen rate, DAU), Milestone II Metrics, SceneStealer Milestone 1, Chat-based Contextual Edit Pipeline, Field Scoping, Prompt Extension (Character Theme / Script / Graphic), PySceneDetect vs Gemini Cut Split PoC (+3 more)

### Community 36 - "Upload·Split 스펙 (API 흐름)"
Cohesion: 0.27
Nodes (11): Apply Split 입력 검증 (end > start), Apply Split (/api/split FFmpeg), SceneStealer V2 - 1. Upload Scene, AI - Auto Split (Gemini 타임스탬프 + FFmpeg 분할), /api/gemini/extract, /api/gemini/timestamp, /api/video?action=split, ensureBaseVideoUrl (Fal.ai 업로드) (+3 more)

### Community 37 - "작업 이력 (Proxy·리팩토링)"
Cohesion: 0.22
Nodes (10): Dual-mode Gemini Client (AI Proxy / Direct), gemini-client.ts, ERR_INVALID_CHAR Authorization header bug, Missing test coverage, Refactoring v1-v3 (~-7,000 lines), SceneStealer Work Log, AB_test_poc branch, AI Proxy Gemini migration (2026-03-11) (+2 more)

### Community 38 - "스크린샷: 병합 결과"
Cohesion: 0.22
Nodes (10): Merge Result Screenshot (Scene Stealer Workspace), Download Scenes Action, History View, Merge Scenes Action, Merged Video, Scene Editor Tab, Scene Preview Tab, Scene Stealer (AI Jam 2025) (+2 more)

### Community 39 - "스크린샷: 분할 결과"
Cohesion: 0.24
Nodes (10): Split Result Screenshot (Scene Stealer Workspace), Regenerate Scene Action, Scene Description Schema (Space & Background, Camera Work, Key Objects, Light & Shadow, Character, Atmosphere), Scene Editor, Scene Preview, Scene Splitting and Attribute Extraction, Scene Stealer (AI Jam 2025), Scene Timeline (+2 more)

### Community 40 - "Vercel 배포 설정"
Cohesion: 0.20
Nodes (9): maxDuration, memory, runtime, buildCommand, devCommand, functions, api/**/*.ts, installCommand (+1 more)

### Community 41 - "Nano Banana 에셋 추출 PoC"
Cohesion: 0.33
Nodes (10): 프레임 캡처→Nano Banana→rembg→다운로드 에셋 추출 플로우, Custom nano banana build app, Nano Banana (Gemini 이미지 모델), rembg (Python 배경 제거 라이브러리), 무기별 투명 PNG 분리 생성 프롬프트, 에셋 구조 분석 및 추출 (Asset Decomposition), 생명체/캐릭터 에셋 추출 프롬프트, 에셋 구조분석 및 추출 구조 PoC (+2 more)

### Community 42 - "ViTag 연동·에셋 교체 시나리오"
Cohesion: 0.27
Nodes (10): Vitag 연동 확장 시나리오, Get ViTag 버튼, Asset Decomposition 단계, 내부 에셋 교체 (Asset Replacement), Cloudinary (텍스트 오버레이 API), 인기 영상 식별 (Competitive Benchmarking), 인기 영상→구조 분석→에셋 추출→내부 에셋 교체→재생성 원클릭 파이프라인, Creatomate (텍스트 오버레이 REST API) (+2 more)

### Community 43 - "1월 회의록·일정"
Cohesion: 0.22
Nodes (10): Asset extraction 일정 산정 (Img/Video to Asset, Re-generate), Dayeon Hyeon (현다연), SceneStealer Meeting Note 2026-01-13, hyunwoo.park, Sunmi Park, Taeyeon Kim (김태연), 코드 리뷰 봇 도입, Scenestealer Meeting Notes 2026-01-19 (+2 more)

### Community 44 - "스크린샷: 재생성 결과"
Cohesion: 0.25
Nodes (9): Regenerate Result Screenshot (Scene Stealer Workspace), Atmosphere, Character Description, Regenerate Scene action, Scene Description (Space & Background, Camera Work, Key Objects, Light & Shadow), Scene Editor, Scene Stealer (AI Jam 2025), Scene Timeline (+1 more)

### Community 45 - "Split Scene 스펙 (세그먼트 편집)"
Cohesion: 0.22
Nodes (9): VideoEditor selectedSegmentIds 재설정 버그, A/B 네비게이션안 (좌측 SNB vs 상단 기능 선택), SceneStealer V2 - 1-1. Split Scene, 최대 10개 세그먼트 제한, 세그먼트 드래그 편집 (최소 0.1초), 선택 세그먼트 루프 재생, splitSelection (Set<number>), Zoom pxPerSec (40~200) (+1 more)

### Community 46 - "앱 진입점"
Cohesion: 0.33
Nodes (5): App(), AppSidebar(), SidebarInset(), SidebarTrigger(), rootElement

### Community 47 - "Timeline·Finalization 스펙"
Cohesion: 0.33
Nodes (7): SceneStealer V2 - 3. Timeline Editor, Regenerate / Extract Prompts, Save Demo, Single / Compare View, SceneStealer V2 - 4. Finalization, Merge → Upload → Compose 파이프라인, 비디오 소스 선택 우선순위 (선택 버전 > 단일 버전 > 원본)

### Community 48 - "Veo 3.1 vs Sora 2 비교"
Cohesion: 0.53
Nodes (6): 자막(caption) 적용 테스트, Image-to-Video with Veo 3 vs. Sora2, 로고 고정 오버레이 테스트, Sora 2 (via ElevenLabs), Veo 3.1, Img to Video 지원 (P1, 로고 유지 테스트)

### Community 49 - "Vercel 설치 스크립트"
Cohesion: 0.40
Nodes (4): args, child, env, projectNpmrc

### Community 50 - "프레임 단위 편집 스펙"
Cohesion: 0.50
Nodes (5): UAC 팀 (대상 사용자), SceneStealer V2 - 3-1. UAC Feedback (Frame), /api/video/split-timestamp, 프레임 단위 정밀 편집 (HH:MM:SS:FF), 1초 버퍼 컷

### Community 51 - "A안(SNB) 채택·배포 환경"
Cohesion: 0.40
Nodes (5): A안 (SNB only) 최종 채택, A/B 설문 결과 A안 채택 결정, 배포 환경 Dev/Alpha(UAC)/Prod 분리, Bi-Weekly Sync 2025-01-12, (1)-(7) 기능별 일정 (Upload/Split/Prompt/Timeline/Asset extractor)

### Community 53 - "영상 생성 도구 리서치"
Cohesion: 0.67
Nodes (3): Phase2 - UI/UX 개선을 위한 Research, Luma Dream Machine, Runway Gen-4

## Knowledge Gaps
- **215 isolated node(s):** `Timestamp`, `SceneTimestamps`, `AudioClip`, `ImageOverlay`, `ScriptClip` (+210 more)
  These have ≤1 connection - possible missing edges or undocumented components.
- **4 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `dependencies` connect `런타임 의존성 (AI·FFmpeg SDK)` to `파일 업로드 UI`, `빌드·타입 의존성`?**
  _High betweenness centrality (0.130) - this node is a cross-community bridge._
- **Why does `react` connect `파일 업로드 UI` to `런타임 의존성 (AI·FFmpeg SDK)`, `앱 내비게이션 (SNB)`, `앱 진입점`, `사이드바 UI 프리미티브`?**
  _High betweenness centrality (0.113) - this node is a cross-community bridge._
- **Why does `cn()` connect `Breadcrumb·리사이즈 패널` to `파일 업로드 UI`, `Sheet UI`, `장면 설명 편집·diff`, `Prompts 화면 컴포넌트`, `에셋 추출 패널`, `Diff·다이얼로그 UI`, `사이드바 UI 프리미티브`, `앱 진입점`, `스크립트 클립·입력 UI`, `앱 내비게이션 (SNB)`?**
  _High betweenness centrality (0.076) - this node is a cross-community bridge._
- **What connects `Timestamp`, `SceneTimestamps`, `AudioClip` to the rest of the system?**
  _215 weakly-connected nodes found - possible documentation gaps or missing edges._
- **Should `런타임 의존성 (AI·FFmpeg SDK)` be split into smaller, more focused modules?**
  _Cohesion score 0.04081632653061224 - nodes in this community are weakly interconnected._
- **Should `파일 업로드 UI` be split into smaller, more focused modules?**
  _Cohesion score 0.08792270531400966 - nodes in this community are weakly interconnected._
- **Should `빌드·타입 의존성` be split into smaller, more focused modules?**
  _Cohesion score 0.05263157894736842 - nodes in this community are weakly interconnected._