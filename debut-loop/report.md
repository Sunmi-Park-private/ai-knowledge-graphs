# Graph Report - debut-loop  (2026-09-27)

## Corpus Check
- Large corpus: 635 files · ~5,222,232 words. Semantic extraction will be expensive (many Claude tokens). Consider running on a subfolder.

## Summary
- 1108 nodes · 2910 edges · 47 communities (37 shown, 10 thin omitted)
- Extraction: 97% EXTRACTED · 3% INFERRED · 0% AMBIGUOUS · INFERRED: 79 edges (avg confidence: 0.82)
- Token cost: 308,606 input · 0 output

## Community Hubs (Navigation)
- 카드 템플릿 · 미니게임 데이터
- 에디터 허브 · 에셋 데이터
- 오디오 · 이징 · 햅틱
- UI 레이아웃 에디터
- 배경 에디터 계획
- 오디션 멤버 시스템 설계
- 빌드 스크립트 (Vite · 싱글파일)
- 모바일 패키징 (Capacitor)
- 2회차 시작 · 리플레이 모드
- 덱 · 멤버 엔진
- 회귀 기억(Recall) 엔진
- 카드 효과 · 관문 · 연습
- 진입점 · BGM 에디터
- 게임 설정 · 치트
- 비트맵 · 비트 에디터
- Pixi 부트 · 로비
- 콘텐츠 JSON 로더 · 테스트
- 엔진 타입 정의
- 게이지 · 진행 · 라우터
- QA 동기화 파이프라인 (/qa-sync)
- 런 화면 그리기
- 에셋 에디터 페이지군
- 캐릭터 에디터
- 게이지 바 UI
- 2회차 시작 설계
- CI · 배포 검증 게이트
- 안드로이드 APK · 에셋 크레딧
- 배경 · UI 스킨 에디터 설계
- 치트 메뉴 · 카드 에디터
- TypeScript 설정
- 메타 UI (설정·출석·앨범)
- 카드 덱빌딩 시스템
- 회귀 루프 설계
- QA 하네스 계획
- 관문 레이아웃 분리
- QA 이슈 파이프라인 설계
- 튜토리얼 · 플로우 에디터
- 기타 소군집 37
- 기타 소군집 38

## God Nodes (most connected - your core abstractions)
1. `mountEngine()` - 51 edges
2. `pos` - 41 edges
3. `startApp()` - 40 edges
4. `editable()` - 36 edges
5. `renderTrainingBoard()` - 32 edges
6. `renderGate()` - 31 edges
7. `pressable()` - 29 edges
8. `skinFit()` - 29 edges
9. `createRunController()` - 27 edges
10. `skinNode()` - 26 edges

## Surprising Connections (you probably didn't know these)
- `QA checklist Google Sheet` --conceptually_related_to--> `Asset QA checklist`  [INFERRED]
  .claude/commands/qa-sync.md → docs/QA-ASSET-CHECKLIST.md
- `CI workflow` --semantically_similar_to--> `Verification gate (typecheck + test)`  [INFERRED] [semantically similar]
  .github/workflows/ci.yml → .claude/commands/qa-work.md
- `Debut Loop! game` --references--> `Android APK workflow`  [INFERRED]
  README.md → .github/workflows/android-apk.yml
- `Content editors` --references--> `Flow editor page`  [EXTRACTED]
  README.md → flow.html
- `Card deckbuilding system` --shares_data_with--> `Gauges (skill, mental, reputation, bond, capital)`  [INFERRED]
  docs/CARD_SYSTEM.md → README.md

## Import Cycles
- None detected.

## Hyperedges (group relationships)
- **QA issue pipeline (sheet -> issue -> fix -> PR)** — _claude_commands_qa_sync_qa_checklist_google_sheet, _claude_commands_qa_sync_qa_sync_command, _claude_commands_qa_sync_debut_loop_qa_private_repo, _claude_commands_qa_work_qa_work_command, docs_qa_readme_qa_process_guide [EXTRACTED 1.00]
- **Asset upload to render flow** — docs_asset_editor_pipeline_assetuploadplugin__vite_dev_endpoints_, docs_asset_editor_pipeline_three_ssot_data_files__uiskins_layout_backgrounds_charskins_, docs_asset_editor_pipeline_asset_updated_ws_push, docs_asset_editor_pipeline_uiskin_ts_slot_helpers, docs_asset_editor_pipeline_layout_editor__pos___editable_ [EXTRACTED 1.00]
- **QA harness automated scan** — docs_qa_harness_plan_qaprobe_ts_slot_instrumentation, docs_qa_harness_plan__goto__deterministic_entry, docs_qa_harness_plan_runcheat___export, docs_qa_harness_plan_qa_scan_mjs_runner, docs_qa_harness_plan_four_machine_checkable_criteria [EXTRACTED 1.00]
- **Dev-only Asset Editor + Upload Plugin + JSON SSOT Pattern** — docs_superpowers_plans_2026_07_28_bg_editor_bg_html_editor_page, docs_superpowers_plans_2026_07_28_bg_editor__bgupload_vite_plugin, docs_superpowers_plans_2026_07_28_bg_editor_backgrounds_json, docs_superpowers_plans_2026_07_28_ui_skin_editor_ui_html_editor_page, docs_superpowers_plans_2026_07_28_ui_skin_editor_imageuploadplugin_factory, docs_superpowers_plans_2026_07_28_ui_skin_editor_uiskins_json [INFERRED 0.85]
- **Flow Editor to Game Live Preview Flow** — src_tools_floweditor, docs_superpowers_plans_2026_08_08_beats_live_preview_beatspreviewplugin, docs_superpowers_plans_2026_08_08_beats_live_preview_in_memory_beats_overlay, docs_superpowers_plans_2026_08_08_beats_live_preview_initbeatspreview, docs_superpowers_plans_2026_08_08_beats_live_preview_triggerredraw [EXTRACTED 1.00]
- **Loop 2 Choice Recording and Replay** — docs_superpowers_plans_2026_07_28_loop2_start_state_choices, docs_superpowers_plans_2026_07_28_loop2_start_triggerregression, docs_superpowers_plans_2026_07_28_loop2_start_runcontroller_choose, docs_superpowers_plans_2026_07_28_loop2_start_fast_mode_replay, docs_superpowers_plans_2026_07_28_loop2_start_swipecard_replay_mode [EXTRACTED 1.00]
- **Dev Asset Editor Upload Pipeline** — docs_superpowers_specs_2026_07_28_bg_editor_design_bg_html_editor, docs_superpowers_specs_2026_07_28_ui_skin_editor_design_ui_html_editor, docs_superpowers_specs_2026_07_28_ui_skin_editor_design_imageuploadplugin_factory, docs_superpowers_specs_2026_07_28_bg_editor_design_bgupload_endpoint, docs_superpowers_specs_2026_07_28_bg_editor_design_backgrounds_json_ssot, docs_superpowers_specs_2026_07_28_ui_skin_editor_design_uiskins_json_ssot [INFERRED 0.85]
- **Live Beat Text Editing Flow** — docs_superpowers_specs_2026_08_08_beats_live_preview_design_beatspreviewplugin, docs_superpowers_specs_2026_08_08_beats_live_preview_design_applyoverlay, docs_superpowers_specs_2026_08_08_beats_live_preview_design_beattextoverlay, docs_superpowers_specs_2026_08_09_flow_editor_loop2_design_beatrecall, docs_superpowers_specs_2026_08_09_flow_editor_loop2_design_recallof [INFERRED 0.85]
- **Hackathon Seed Shims** — docs_superpowers_specs_2026_08_29_hackathon_prep_design_world_step_contract, docs_superpowers_specs_2026_08_29_hackathon_prep_design_runscene_game_loop_shim, docs_superpowers_specs_2026_08_29_hackathon_prep_design_stageprofile_orientation_shim, docs_superpowers_specs_2026_08_29_hackathon_prep_design_demo_scene, docs_superpowers_specs_2026_08_29_hackathon_prep_design_export_seed_script [EXTRACTED 1.00]

## Communities (47 total, 10 thin omitted)

### Community 0 - "카드 템플릿 · 미니게임 데이터"
Cohesion: 0.05
Nodes (112): cardTemplates, buildMatchDeck(), DODGE_COLS, DODGE_E_HEARTS, DODGE_P_HEARTS, DODGE_ROWS, DODGE_SECOND_TILE, DODGE_SPAWN (+104 more)

### Community 1 - "에디터 허브 · 에셋 데이터"
Cohesion: 0.05
Nodes (65): BgSlot, qrcode-generator, src_data_assets, src_data_backgrounds, src_data_charskins, src_data_uiskins, bgSlots, EditorEntry (+57 more)

### Community 2 - "오디오 · 이징 · 햅틱"
Cohesion: 0.07
Nodes (61): applyVolume(), bgmMuted(), bgmVolume(), setBgmMuted(), setBgmVolume(), EASE, easeIn(), easeInOut() (+53 more)

### Community 3 - "UI 레이아웃 에디터"
Cohesion: 0.07
Nodes (66): src_data_layout, applyStoredStyle(), buildMapping(), buildRow(), buildTextInput(), clearHighlight(), clones, cmpPath() (+58 more)

### Community 4 - "배경 에디터 계획"
Cohesion: 0.05
Nodes (53): /__bgupload Vite Plugin, Background Image Editor Plan, Background Slot SSOT, backgrounds.json, bg.html Editor Page, Default Background Fallback, pickBgSlot, Story Background Fade Transition (+45 more)

### Community 5 - "오디션 멤버 시스템 설계"
Cohesion: 0.07
Nodes (48): Audition Member System Design, Audition Ticket Exchange, Candidate Pool, cast_role Flag Exclusive Alternate Beats, droppedCandidates, joinMember Effect, Member Check Board, membersLocked W18 Lock-in (+40 more)

### Community 6 - "빌드 스크립트 (Vite · 싱글파일)"
Cohesion: 0.05
Nodes (31): ref_node_child_process, ref_node_fs, ref_node_path, vite, html, html0, js, m (+23 more)

### Community 7 - "모바일 패키징 (Capacitor)"
Cohesion: 0.04
Nodes (41): config, dependencies, @capacitor/android, @capacitor/core, @capacitor/ios, pixi.js, description, devDependencies (+33 more)

### Community 8 - "2회차 시작 · 리플레이 모드"
Cohesion: 0.08
Nodes (35): Fast Mode (Replay), Loop 2 Start Improvement Plan, Normal Mode, renderEndScreen, RunController.choose, State.choices, swipeCard Replay Mode, triggerRegression (+27 more)

### Community 9 - "덱 · 멤버 엔진"
Cohesion: 0.12
Nodes (33): addCard(), removeCards(), applyGateStat(), applyTrainingStat(), AUDITION_ORDER, AUDITION_ROLES, AUDITION_STAT, auditionRank() (+25 more)

### Community 10 - "회귀 기억(Recall) 엔진"
Cohesion: 0.13
Nodes (30): beatsOfLoop(), pick(), recallIsInherited(), recallOf(), RecallText, BeatRecall, LoopCount, ACT_COLOR (+22 more)

### Community 11 - "카드 효과 · 관문 · 연습"
Cohesion: 0.14
Nodes (25): cardEffect(), GRADE_MULT, makeCards(), templateGauges(), GATE_PICKS, gatePickCount(), resolveGate(), resolveTraining() (+17 more)

### Community 12 - "진입점 · BGM 에디터"
Cohesion: 0.12
Nodes (25): src_data_bgm, main(), EXTS, loadLoadingBg(), loadPrologueBg(), BgmId, bgmPositionMs(), BgmTrack (+17 more)

### Community 13 - "게임 설정 · 치트"
Cohesion: 0.11
Nodes (27): casting, gates, tuning, RhythmJudgeLevel, currentDraw(), initGameCheats(), Cheat, CheatPick (+19 more)

### Community 14 - "비트맵 · 비트 에디터"
Cohesion: 0.08
Nodes (25): beatmaps, Beatmap, BeatmapNote, RhythmMode, audio, commit(), getMap(), head (+17 more)

### Community 15 - "Pixi 부트 · 로비"
Cohesion: 0.21
Nodes (24): pixi.js, currentRunCards(), currentRunInfo(), visibleCards(), center(), LobbyResult, mkText(), playPrologue() (+16 more)

### Community 16 - "콘텐츠 JSON 로더 · 테스트"
Cohesion: 0.09
Nodes (22): vitest, src_data_beatmaps, src_data_beats_demo2_zeroc, src_data_cards, src_data_characters, src_data_config, src_data_gates, beats (+14 more)

### Community 17 - "엔진 타입 정의"
Cohesion: 0.10
Nodes (10): CharacterDef, GateDef, MiniGameGrade, TrainingId, CharAssets, MemberBoardOpts, EngineOpts, RunController (+2 more)

### Community 18 - "게이지 · 진행 · 라우터"
Cohesion: 0.23
Nodes (17): clampGauges(), IDS, isCollapsed(), advance(), AdvanceResult, isFastForward(), resolveRunEnd(), loopOk() (+9 more)

### Community 19 - "QA 동기화 파이프라인 (/qa-sync)"
Cohesion: 0.14
Nodes (20): Approval gate before issue creation, debut-loop-qa private repo, QA checklist Google Sheet, qa-row dedup marker, qa-sync command, Verdict to label mapping, by Claude comment signature, Public visibility rule (no QA numbers in commits) (+12 more)

### Community 20 - "런 화면 그리기"
Cohesion: 0.19
Nodes (16): newRun(), startApp(), draw(), drawHeader(), renderGauges(), pairSpace(), DAYS_PER_WEEK, ddayDays() (+8 more)

### Community 21 - "에셋 에디터 페이지군"
Cohesion: 0.16
Nodes (18): Beat editor page, Background editor page, BGM editor page, Character editor page, Asset editor pipeline, asset-updated ws push, assetUploadPlugin (vite dev endpoints), Display method 3 categories (fill/contain/fit-box) (+10 more)

### Community 22 - "캐릭터 에디터"
Cohesion: 0.22
Nodes (16): animatePreview(), EXTS, LIVE, makeCell(), openLightbox(), SCALABLE, scaleBar(), showUploaded() (+8 more)

### Community 23 - "게이지 바 UI"
Cohesion: 0.15
Nodes (11): Effect, GaugeId, BAR_ORDER, CELL_X, GaugeOpts, GaugePanel, GAUGES, ART (+3 more)

### Community 24 - "2회차 시작 설계"
Cohesion: 0.18
Nodes (15): Fast Mode vs Normal Mode, Loop 2 Opening Beat, Loop 2 Start Improvement Design, State choices Record, swipeCard replay Option, triggerRegression, 10px Snap with Alt Override, Chroma Green Editor Grid (+7 more)

### Community 25 - "CI · 배포 검증 게이트"
Cohesion: 0.16
Nodes (14): Verification gate (typecheck + test), CI workflow, Extended Pages deploy timeout, GitHub Pages workflow, Node version pin (.nvmrc), 40-hour time budget, Cut gate, NAN2026 finals volume back-calculation (+6 more)

### Community 26 - "안드로이드 APK · 에셋 크레딧"
Cohesion: 0.18
Nodes (13): Android APK workflow, Capacitor android sync, All assets AI-generated (GPT + After Effects, Suno), Asset credits, createRunController, Data loader (src/data/index.ts), renderGauges, S0 Pixi boot + swipe plan (+5 more)

### Community 27 - "배경 · UI 스킨 에디터 설계"
Cohesion: 0.28
Nodes (13): Background Image Editor Design, backgrounds.json SSOT, bg.html Editor, __bgupload Endpoint, gateBg, pickBgSlot, 9-slice Skin Mode, imageUploadPlugin Factory (+5 more)

### Community 28 - "치트 메뉴 · 카드 에디터"
Cohesion: 0.33
Nodes (11): inGameCheck(), initCheatMenu(), deckSummary(), effSummary(), render(), renderCardEditor(), renderGauges(), renderJump() (+3 more)

### Community 29 - "TypeScript 설정"
Cohesion: 0.18
Nodes (10): compilerOptions, module, moduleResolution, noUncheckedIndexedAccess, resolveJsonModule, skipLibCheck, strict, target (+2 more)

### Community 30 - "메타 UI (설정·출석·앨범)"
Cohesion: 0.29
Nodes (10): Audio manager (ui/audio.ts), Daily reward stamp board, FE shell scope decision, Meta UI design (settings/shop/daily/album), MetaSave localStorage store, Photo album, Settings menu, Shop (+2 more)

### Community 31 - "카드 덱빌딩 시스템"
Cohesion: 0.31
Nodes (9): addCard / removeCards, Card deckbuilding system, Card grade multiplier (common/rare/epic), cardEffect, Deck sheet UI (A plan + P2 fan picker), GATE_PICKS (gate grade -> picks), Minigame difficulty scaling by act, resolveGate / gatePickCount (+1 more)

### Community 32 - "회귀 루프 설계"
Cohesion: 0.28
Nodes (9): Collect-in-training / spend-at-gate loop, Beat loop filter (router), Fixed endings (loop1 accident / loop2 true), Inheritance rules on regression, loopCount / seenBeats state, Regression acceleration (seen-beat fast skip), Regression loop design, triggerRegression() (+1 more)

### Community 33 - "QA 하네스 계획"
Cohesion: 0.36
Nodes (9): Verdict criteria codes 1-5, ?goto= deterministic entry, Four machine-checkable criteria, isDevMode gate, QA harness plan, qa-scan.mjs runner, qaProbe.ts slot instrumentation, runCheat() export (+1 more)

### Community 34 - "관문 레이아웃 분리"
Cohesion: 0.43
Nodes (8): btnText, centerBtnLabel, Gate Layout Split and Label Centering Plan, gateKeyPrefix, layout.json center Field, registerBtnLabel, renderGate, Shared Key Inheritance

### Community 35 - "QA 이슈 파이프라인 설계"
Cohesion: 0.43
Nodes (8): Input Adapter Normalized Rows, Public Private Repo Split, QA Issue Pipeline Design, qa-row Dedup Marker, qa-sync Command, qa-work Command, QA Work Priority, QA Work-Type Labels

### Community 36 - "튜토리얼 · 플로우 에디터"
Cohesion: 0.33
Nodes (7): Cheat menu, Dependency traps (cheatMenu, flowEditor), guide(id, speaker, text) overlay, Hybrid placement (prologue weave + first-encounter guides), Once-per-device localStorage guard, Tutorial plan, Flow editor page

## Knowledge Gaps
- **234 isolated node(s):** `config`, `name`, `version`, `description`, `type` (+229 more)
  These have ≤1 connection - possible missing edges or undocumented components. (Counts symbols only; 324 node(s) total have ≤1 connection when file, concept and rationale nodes are included.)
- **10 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `pixi.js` connect `Pixi 부트 · 로비` to `카드 템플릿 · 미니게임 데이터`, `에디터 허브 · 에셋 데이터`, `오디오 · 이징 · 햅틱`, `UI 레이아웃 에디터`, `모바일 패키징 (Capacitor)`, `진입점 · BGM 에디터`, `게임 설정 · 치트`, `게이지 바 UI`?**
  _High betweenness centrality (0.101) - this node is a cross-community bridge._
- **Why does `vite` connect `빌드 스크립트 (Vite · 싱글파일)` to `모바일 패키징 (Capacitor)`?**
  _High betweenness centrality (0.065) - this node is a cross-community bridge._
- **Why does `vitest` connect `콘텐츠 JSON 로더 · 테스트` to `카드 템플릿 · 미니게임 데이터`, `에디터 허브 · 에셋 데이터`, `UI 레이아웃 에디터`, `모바일 패키징 (Capacitor)`, `2회차 시작 · 리플레이 모드`, `덱 · 멤버 엔진`, `회귀 기억(Recall) 엔진`, `카드 효과 · 관문 · 연습`, `게이지 · 진행 · 라우터`?**
  _High betweenness centrality (0.030) - this node is a cross-community bridge._
- **What connects `config`, `name`, `version` to the rest of the system?**
  _234 weakly-connected nodes found - possible documentation gaps or missing edges._
- **Should `카드 템플릿 · 미니게임 데이터` be split into smaller, more focused modules?**
  _Cohesion score 0.050137741046831955 - nodes in this community are weakly interconnected._
- **Should `에디터 허브 · 에셋 데이터` be split into smaller, more focused modules?**
  _Cohesion score 0.053946053946053944 - nodes in this community are weakly interconnected._
- **Should `오디오 · 이징 · 햅틱` be split into smaller, more focused modules?**
  _Cohesion score 0.06924882629107981 - nodes in this community are weakly interconnected._