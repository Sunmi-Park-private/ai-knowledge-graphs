# Graph Report - nhn-2026-game-hackathon  (2026-09-27)

## Corpus Check
- Large corpus: 974 files · ~7,817,790 words. Semantic extraction will be expensive (many Claude tokens). Consider running on a subfolder.

## Summary
- 1313 nodes · 3436 edges · 50 communities (44 shown, 6 thin omitted)
- Extraction: 98% EXTRACTED · 2% INFERRED · 0% AMBIGUOUS · INFERRED: 76 edges (avg confidence: 0.84)
- Token cost: 220,976 input · 0 output

## Community Hubs (Navigation)
- 스테이지 데이터 · 테스트
- 설정 · 아트 페이지 (Pixi)
- 동물 운동회(RACE) · 부스터
- 케이지 아트 맞춤 · 탈출 연출
- 에셋 경로 · 스토리 · 로비 장면
- UI 레이아웃 에디터
- 헥사 슈터 설계 · 계획
- 에디터 저장 서버 · 레이아웃 이력
- 빌드 · 효과음 생성 스크립트
- 타일 파편 물리
- 패키지 · Capacitor 설정
- 당겨 쏘기 조준
- 조준 규칙 · 실패선 · 격자
- 오디오 슬롯 · 볼륨
- 이벤트 · 도감 에셋 슬롯
- 로비 슬롯 · 레이아웃 파서
- 튜토리얼 코치
- 장갑 타일 · 파워 게이지 연출
- RACE 에셋 배선
- 보드 뷰
- 레이아웃 밸런스 스크립트 (Python)
- RACE 에셋 파서
- 게임 규칙 개념 (케이지·금·낙하)
- 동물 정의 · 로비 장면
- 발사 원점 · 첫 반사 제한
- 스테이지 실행 · 클리어 판정
- 확인창 레이아웃
- HUD 뷰
- 천장 하강 연출
- TypeScript 설정
- 아키텍처 원칙 (단방향 의존)
- 컷 순서 · 물리 키워드
- 게임오버 레이아웃
- 코드 규칙 5종 · 제출물
- 인게임 에디터 · 드롭인 에셋
- 레벨 밸런스 · 헤드리스 봇
- 슬롯 터치 영역
- AI 활용 방식 · 검증 게이트
- 난이도 축 · 메타 레이어
- 케이지 금(Crack)
- 안드로이드 빌드 스크립트
- AI 에셋 제작 (Nano Banana)
- 실패선
- 기타 소군집 43
- 기타 소군집 44
- 기타 소군집 45
- 기타 소군집 46
- 기타 소군집 47
- 기타 소군집 48

## God Nodes (most connected - your core abstractions)
1. `vitest` - 57 edges
2. `runStageScreen()` - 56 edges
3. `key()` - 55 edges
4. `pixi.js` - 46 edges
5. `editable()` - 33 edges
6. `fitSprite()` - 32 edges
7. `openRace()` - 29 edges
8. `slot()` - 26 edges
9. `Axial` - 25 edges
10. `main()` - 25 edges

## Surprising Connections (you probably didn't know these)
- `GitHub Pages Deploy Workflow (manual dispatch)` --semantically_similar_to--> `Single-file HTML Build`  [INFERRED] [semantically similar]
  .github/workflows/pages.yml → README.md
- `UI Editor Entry Page (ui.html -> src/tools/uiEditor.ts)` --implements--> `UI Layout & Asset Editor (/ui.html)`  [INFERRED]
  ui.html → docs/ART_SPEC.md
- `Audio Asset Slots README` --conceptually_related_to--> `Miss (Whiff) Consumes a Shot`  [AMBIGUOUS]
  public/assets/audio/README.md → docs/superpowers/specs/2026-09-05-drag-charge-launcher-design.md
- `cellsOf()` --calls--> `key()`  [EXTRACTED]
  tests/hex/cageEdge.test.ts → src/engine/hex/coords.ts
- `clearFace()` --calls--> `key()`  [EXTRACTED]
  tests/hex/cageFaces.test.ts → src/engine/hex/coords.ts

## Import Cycles
- None detected.

## Hyperedges (group relationships)
- **Core Rescue Loop** — docs_gdd_projectile_from_board_colors, docs_gdd_pop_three_or_more, docs_gdd_floating_cluster_drop, docs_gdd_rescue_condition, docs_gdd_cage [EXTRACTED 1.00]
- **Physics Law Keyword Implementation** — docs_gdd_physics_law_keyword, docs_gdd_spectrum_color_order, docs_gdd_floating_cluster_drop, docs_ai_usage_drag_charge_launcher, docs_intro_deck_animal_race [EXTRACTED 1.00]
- **Generative Art Pipeline** — docs_ai_usage_claude_prompt_layer, docs_ai_usage_nano_banana_tool, docs_ai_usage_reference_asset_variation, docs_ai_usage_seedance_stage_video, docs_art_spec_ui_editor [INFERRED 0.85]
- **Shot Resolution Pipeline (snap, merge, gravity, rescue)** — docs_superpowers_plans_2026_09_04_hexa_merge_shooter_2_run_fireat_resolution, docs_superpowers_specs_2026_09_04_hexa_merge_shooter_design_snap_algorithm, docs_superpowers_specs_2026_09_04_hexa_merge_shooter_design_merge_flood_fill, docs_superpowers_specs_2026_09_04_hexa_merge_shooter_design_gravity_floating_clusters, docs_superpowers_specs_2026_09_04_hexa_merge_shooter_design_rescue_judgement [EXTRACTED 1.00]
- **Drag-Charge Launcher Flow** — docs_superpowers_specs_2026_09_05_drag_charge_launcher_design_slingshot_aim, docs_superpowers_specs_2026_09_05_drag_charge_launcher_design_parabolic_shot_physics, docs_superpowers_specs_2026_09_05_drag_charge_launcher_design_right_triangle_power_gauge, docs_superpowers_specs_2026_09_05_drag_charge_launcher_design_horse_sequence_scrub, docs_superpowers_plans_2026_09_04_hexa_merge_shooter_3_screen_launcher_ts [INFERRED 0.85]
- **Stage Difficulty Model** — docs_superpowers_specs_2026_09_05_stage_balance_design_four_difficulty_knobs, docs_superpowers_specs_2026_09_05_stage_balance_design_axes_multiply_not_add, docs_superpowers_specs_2026_09_05_stage_balance_design_color_cost_index, docs_superpowers_specs_2026_09_05_stage_balance_design_cage_as_anchor, docs_superpowers_specs_2026_09_05_stage_balance_design_balance_bot_harness [INFERRED 0.85]

## Communities (50 total, 6 thin omitted)

### Community 0 - "스테이지 데이터 · 테스트"
Cohesion: 0.05
Nodes (110): vitest, stages, src_data_stages_stage_01, src_data_stages_stage_02, src_data_stages_stage_03, src_data_stages_stage_04, src_data_stages_stage_05, src_data_stages_stage_06 (+102 more)

### Community 1 - "설정 · 아트 페이지 (Pixi)"
Cohesion: 0.05
Nodes (104): pixi.js, slot(), DEFAULT_SETTINGS, parseSettings(), serializeSettings(), Settings, ArtButton, Box (+96 more)

### Community 2 - "동물 운동회(RACE) · 부스터"
Cohesion: 0.05
Nodes (72): RACE, RACE_LANE_ORDER, BoosterId, Profile, advanceAi(), aiSpeed(), makeAiPace(), createRace() (+64 more)

### Community 3 - "케이지 아트 맞춤 · 탈출 연출"
Cohesion: 0.05
Nodes (68): CageArtFit, hexArtBox(), measureCageArt(), measureHexRow(), readAlpha(), animate(), animateUntil(), artBox() (+60 more)

### Community 4 - "에셋 경로 · 스토리 · 로비 장면"
Cohesion: 0.06
Nodes (60): hexAssetPaths, VIDEO_SLOT_IDS, videoAssetPaths, sceneCandidates(), Speaker, STORY_BEATS, storyBeat, StoryLine (+52 more)

### Community 5 - "UI 레이아웃 에디터"
Cohesion: 0.06
Nodes (65): normalizeAreas(), sameAreas(), UiArea, UiUpload, actions, adoptAreas(), announce(), applySnapshot() (+57 more)

### Community 6 - "헥사 슈터 설계 · 계획"
Cohesion: 0.06
Nodes (58): Art Spec, GDD, Task 1: Axial Coordinates (coords.ts), Hexa Merge Shooter Plan Part 1: Grid and Judgement, Task 5: Trajectory and Snap (shot.ts) - top project risk, Boosters (boosters.ts), fireAt: Snap -> Merge -> Drop -> Rescue Resolution, Hexa Merge Shooter Plan Part 2: Stage Run (+50 more)

### Community 7 - "에디터 저장 서버 · 레이아웃 이력"
Cohesion: 0.09
Nodes (40): hasEditorServer(), NO_EDITOR_SERVER, readJson(), apply(), applyAll(), applyStyle(), buildRow(), catchUpLayout() (+32 more)

### Community 8 - "빌드 · 효과음 생성 스크립트"
Cohesion: 0.05
Nodes (28): ref_node_child_process, ref_node_fs, ref_node_path, ref_node_url, vite, expRamp(), N, PICKS (+20 more)

### Community 9 - "타일 파편 물리"
Cohesion: 0.08
Nodes (30): collidePieces(), DebrisArena, DebrisBody, DebrisPhase, FADE_MS, FLOOR_BOUNCE, GRAVITY, MAX_LIFE_MS (+22 more)

### Community 10 - "패키지 · Capacitor 설정"
Cohesion: 0.05
Nodes (39): config, dependencies, pixi.js, description, devDependencies, @capacitor/android, @capacitor/cli, @capacitor/core (+31 more)

### Community 11 - "당겨 쏘기 조준"
Cohesion: 0.07
Nodes (16): Aim, AIM_EXPO, applyExpo(), clamp(), createDragAim(), read(), DEAD_ZONE, DragAim (+8 more)

### Community 12 - "조준 규칙 · 실패선 · 격자"
Cohesion: 0.13
Nodes (24): BLOCKED_BAND, FIRST_BOUNCE_LIMIT_Y, BOARD, CELL_W, CENTER_H, CENTER_W, COLS, FIELD_TOP (+16 more)

### Community 13 - "오디오 슬롯 · 볼륨"
Cohesion: 0.11
Nodes (25): audioAssetPaths, AudioSlotId, applyVolume(), AudioId, baseVolume(), bgmVolume(), cueCursor, cuePool (+17 more)

### Community 14 - "이벤트 · 도감 에셋 슬롯"
Cohesion: 0.12
Nodes (19): collectionAssetPaths, EVENT_SLOT_IDS, eventAssetPaths, EventSlotId, frameIndex(), frames(), framesByAnimal(), lobbyAssetPaths (+11 more)

### Community 15 - "로비 슬롯 · 레이아웃 파서"
Cohesion: 0.11
Nodes (16): LOBBY_SLOT_IDS, storyAssetPaths, num(), parseAreas(), slotCenter(), uiAreas, uiAudios, UiSlot (+8 more)

### Community 16 - "튜토리얼 코치"
Cohesion: 0.11
Nodes (9): CoachEvent, CoachStep, createTutorialCoach(), TUTORIAL_STEPS, TutorialCoach, CoachBubble, CoachTargets, createCoachBubble() (+1 more)

### Community 17 - "장갑 타일 · 파워 게이지 연출"
Cohesion: 0.12
Nodes (14): ArmorHit, fallAt(), playArmorHits(), shakeAt(), createFailLine(), createPowerGauge(), FALLBACK, PowerGauge (+6 more)

### Community 18 - "RACE 에셋 배선"
Cohesion: 0.12
Nodes (17): AUDIO_SLOT_IDS, raceAssetPaths, manifest, Box, FALLBACK, RACE_AREAS, RACE_SLOT_IDS, RaceAreaId (+9 more)

### Community 19 - "보드 뷰"
Cohesion: 0.18
Nodes (10): BoardView, createBoardView(), makeView(), TileTextures, drawTileFallback(), hexPoints(), HORSESHOE_COLOR, makeHorseshoeView() (+2 more)

### Community 20 - "레이아웃 밸런스 스크립트 (Python)"
Cohesion: 0.17
Nodes (14): collections, itertools, json, math, random, best(), comps(), dist() (+6 more)

### Community 21 - "RACE 에셋 파서"
Cohesion: 0.17
Nodes (15): BOOSTER_IDS, BoosterAssetId, byAnimal(), frames(), obj(), parseRaceAssets(), pick(), RACE_BG_IDS (+7 more)

### Community 22 - "게임 규칙 개념 (케이지·금·낙하)"
Cohesion: 0.15
Nodes (15): Flat-top Cage Art (2:sqrt3, hollow interior), Multi-cell Cage (7 cells, flat-top), Core Loop (aim-fire-snap-match-pop-drop-rescue), Top-side Crack Progress Indicator (0-5), Floating Cluster Drop (anchors: top row + cage), Hex-grid Merge Shooter Genre, Horseshoe Tile (neutral, collected on drop), Pop 3+ Same-color Cluster (flood fill) (+7 more)

### Community 23 - "동물 정의 · 로비 장면"
Cohesion: 0.22
Nodes (6): AnimalDef, ANIMALS, SCENE_KEYS, sceneFor(), START_KEY, ids

### Community 24 - "발사 원점 · 첫 반사 제한"
Cohesion: 0.22
Nodes (11): horse(), aimBlocked(), firstBounceIndex(), launchOrigin(), launchOriginLocal(), handSlot(), Point, createLauncher() (+3 more)

### Community 25 - "스테이지 실행 · 클리어 판정"
Cohesion: 0.31
Nodes (15): isCleared(), isFailed(), createCageCracks(), cellToScreen(), runStageScreen(), finish(), lowestOccupiedRow(), onDown() (+7 more)

### Community 26 - "확인창 레이아웃"
Cohesion: 0.21
Nodes (8): uiAssetPaths, Box, CONFIRM_AREA, CONFIRM_ASSETS, CONFIRM_FALLBACK, ConfirmSlotId, area, Box

### Community 27 - "HUD 뷰"
Cohesion: 0.25
Nodes (7): box(), centered(), createHudView(), groupFor(), HudTextures, HudView, panel()

### Community 28 - "천장 하강 연출"
Cohesion: 0.35
Nodes (9): SHAKE_AMP, SHAKE_HZ, SHAKE_LEAD_MS, shakeX(), SLIDE_MS, slideDone(), slideY(), applyBoardOffset() (+1 more)

### Community 29 - "TypeScript 설정"
Cohesion: 0.18
Nodes (10): compilerOptions, module, moduleResolution, noUncheckedIndexedAccess, resolveJsonModule, skipLibCheck, strict, target (+2 more)

### Community 30 - "아키텍처 원칙 (단방향 의존)"
Cohesion: 0.29
Nodes (10): Android Capacitor Build (letterboxed 9:16), Latest-dated Spec Is Canonical, One-way Dependency Architecture (data -> engine -> ui), Art Production Spec, Trapezoid Play Area (PEN in geom.ts), Game Design Document (GDD), No In-game Runtime LLM, Game Introduction Deck (+2 more)

### Community 31 - "컷 순서 · 물리 키워드"
Cohesion: 0.20
Nodes (10): Cut Order: FX -> Meta -> Core, AI-written Test Defects, Drag-charge Slingshot Launcher (PR #7), Animal Race Assets, Boosters (Bomb, Rainbow, Horseshoe), Physics Law Keyword (speed, gravity, reflection, light & color), Projectile Color Drawn From Board Colors, Six Colors in Visible-Spectrum Wavelength Order (+2 more)

### Community 32 - "게임오버 레이아웃"
Cohesion: 0.27
Nodes (6): Box, GAMEOVER_AREA, GAMEOVER_ASSETS, GAMEOVER_FALLBACK, area, Box

### Community 33 - "코드 규칙 5종 · 제출물"
Cohesion: 0.22
Nodes (9): New Files Cut at 200 Lines, Code Conventions 5 Rules (new code only), Cheats/Debug Behind devMode Gate, Field-validated JSON Instead of 'as unknown as', New ui/ Files Do Not Import ../data Directly, Screen State in Closure, Not Module-level let, Three Submission Deliverables (prototype, agent design doc, directing spec), Agent Design Document (+1 more)

### Community 34 - "인게임 에디터 · 드롭인 에셋"
Cohesion: 0.32
Nodes (8): Layout Editor Saves Only on Dev Server, Cloudflare Tunnel Designer Workflow, In-game Editor (/?editor=1), UI Layout & Asset Editor (/ui.html), uiLayout.json, Game Entry Page (index.html -> src/main.ts), Drop-in Asset Pipeline with Fallback Rendering, UI Editor Entry Page (ui.html -> src/tools/uiEditor.ts)

### Community 35 - "레벨 밸런스 · 헤드리스 봇"
Cohesion: 0.33
Nodes (7): Ceiling Descent Fail Condition (pushSeconds), Headless Balance Bot (50 runs per stage), Level Balance Design (6 Stages), Pushes Survived Difficulty Unit, Same-color 2-connection on Cage Perimeter, Slack Ratio (given shots / required shots), Stage Balance Design Spec (2026-09-05)

### Community 36 - "슬롯 터치 영역"
Cohesion: 0.43
Nodes (4): slotHitRect(), nodeFor(), project(), rectsFor()

### Community 37 - "AI 활용 방식 · 검증 게이트"
Cohesion: 0.40
Nodes (6): CI Workflow (typecheck + vitest on PR), AI Usage Technical Document, Human Defines, AI Generates, Human Verifies, Skill-based Spec->Plan->Implement->Review Workflow, Verification Gate (tsc + vitest before claiming done), Git Worktree Isolation and Explicit Staging

### Community 38 - "난이도 축 · 메타 레이어"
Cohesion: 0.33
Nodes (6): Meta Layer (Lobby/Ranch, Collection, Level), Six Rescue Animals (rabbit, monkey, deer, sheep, zebra, elephant), Two Difficulty Axes Multiply, Color Cost Index, Four Difficulty Knobs (cage count, pair density, color count, projectile ratio), Six-stage Difficulty Curve

### Community 40 - "안드로이드 빌드 스크립트"
Cohesion: 0.40
Nodes (4): ANDROID_HOME, JAVA_HOME, PATH, android.sh script

### Community 41 - "AI 에셋 제작 (Nano Banana)"
Cohesion: 0.50
Nodes (4): Claude Code as Structured Prompt Layer, Mockup-first Asset Extraction (ChatGPT), Nano Banana Custom Image Tool, Reference Asset Controlled Variation

### Community 43 - "기타 소군집 43"
Cohesion: 0.67
Nodes (3): Kling Idle Video Batch Tool (built with Codex), Seedance 2.5 Start/End-frame Stage Videos, Lobby Scene Videos (cumulative, webm)

### Community 44 - "기타 소군집 44"
Cohesion: 0.67
Nodes (3): Asset Delivery Priority Order, Pointy-top Hex Tile Spec (sqrt3:2, zero canvas margin), tileArtSize Test

### Community 45 - "기타 소군집 45"
Cohesion: 0.67
Nodes (3): Red Horse as Launcher, 2026 Byeong-o Year of the Red Horse, Cool Red Horse Contest Story

## Ambiguous Edges - Review These
- `Audio Asset Slots README` → `Miss (Whiff) Consumes a Shot`  [AMBIGUOUS]
  public/assets/audio/README.md · relation: conceptually_related_to
- `Stage Data Validating Loader (stageLoader.ts)` → `Per-Stage PLACE Override`  [AMBIGUOUS]
  docs/superpowers/specs/2026-09-05-stage-balance-design.md · relation: conceptually_related_to

## Knowledge Gaps
- **256 isolated node(s):** `config`, `name`, `version`, `description`, `type` (+251 more)
  These have ≤1 connection - possible missing edges or undocumented components. (Counts symbols only; 398 node(s) total have ≤1 connection when file, concept and rationale nodes are included.)
- **6 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **What is the exact relationship between `Audio Asset Slots README` and `Miss (Whiff) Consumes a Shot`?**
  _Edge tagged AMBIGUOUS (relation: conceptually_related_to) - confidence is low._
- **What is the exact relationship between `Stage Data Validating Loader (stageLoader.ts)` and `Per-Stage PLACE Override`?**
  _Edge tagged AMBIGUOUS (relation: conceptually_related_to) - confidence is low._
- **Why does `vitest` connect `스테이지 데이터 · 테스트` to `설정 · 아트 페이지 (Pixi)`, `동물 운동회(RACE) · 부스터`, `케이지 아트 맞춤 · 탈출 연출`, `에셋 경로 · 스토리 · 로비 장면`, `UI 레이아웃 에디터`, `에디터 저장 서버 · 레이아웃 이력`, `빌드 · 효과음 생성 스크립트`, `타일 파편 물리`, `패키지 · Capacitor 설정`, `당겨 쏘기 조준`, `조준 규칙 · 실패선 · 격자`, `로비 슬롯 · 레이아웃 파서`, `튜토리얼 코치`, `RACE 에셋 배선`, `동물 정의 · 로비 장면`, `발사 원점 · 첫 반사 제한`, `확인창 레이아웃`, `천장 하강 연출`, `게임오버 레이아웃`, `슬롯 터치 영역`?**
  _High betweenness centrality (0.136) - this node is a cross-community bridge._
- **Why does `pixi.js` connect `설정 · 아트 페이지 (Pixi)` to `동물 운동회(RACE) · 부스터`, `케이지 아트 맞춤 · 탈출 연출`, `에셋 경로 · 스토리 · 로비 장면`, `케이지 금(Crack)`, `에디터 저장 서버 · 레이아웃 이력`, `타일 파편 물리`, `패키지 · Capacitor 설정`, `당겨 쏘기 조준`, `조준 규칙 · 실패선 · 격자`, `튜토리얼 코치`, `장갑 타일 · 파워 게이지 연출`, `보드 뷰`, `발사 원점 · 첫 반사 제한`, `HUD 뷰`?**
  _High betweenness centrality (0.085) - this node is a cross-community bridge._
- **Why does `History` connect `에디터 저장 서버 · 레이아웃 이력` to `UI 레이아웃 에디터`?**
  _High betweenness centrality (0.030) - this node is a cross-community bridge._
- **Are the 3 inferred relationships involving `runStageScreen()` (e.g. with `onDown()` and `onMove()`) actually correct?**
  _`runStageScreen()` has 3 INFERRED edges - model-reasoned connections that need verification._
- **Are the 7 inferred relationships involving `key()` (e.g. with `cageEdge.test.ts` and `cageFaces.test.ts`) actually correct?**
  _`key()` has 7 INFERRED edges - model-reasoned connections that need verification._