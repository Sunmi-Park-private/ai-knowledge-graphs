# Graph Report - .  (2026-09-27)

## Corpus Check
- 153 files · ~323,716 words
- Verdict: corpus is large enough that graph structure adds value.

## Summary
- 1030 nodes · 1477 edges · 72 communities (71 shown, 1 thin omitted)
- Extraction: 83% EXTRACTED · 17% INFERRED · 0% AMBIGUOUS · INFERRED: 246 edges (avg confidence: 0.83)
- Token cost: 1,970,095 input · 0 output

## Community Hubs (Navigation)
- Creative Upload & Tagging
- Creative Lifecycle Unification
- Iteration Performance Matching
- Monitoring Dashboard Polish
- Competitive Insights Followups
- Monitoring Campaign Backend
- Creative Library Linking
- UACOS Architecture Overview
- Creative Status Workflow
- Exact Match Search Cleanup
- AppsFlyer Install Correction
- SOV Semantics
- Library Redesign & RBAC
- Jira Sync
- Agent Gateway Plans
- External Data Adapters
- Monitoring AI Actions (UI)
- Competitive Insights Query
- Project-Creative Attach
- Monitoring Custom Views
- Brief Detail Screen
- Channel Activity Monitoring
- Central DB Schema
- New Project Screen
- Idea Library Screen
- Report Degrade Policy
- Review Process Design
- Central Dashboard Tracks
- Vungle Report Design
- Prod OOM & Query Limits
- Human-in-the-Loop Principles
- Glossary Core Concepts
- Creative Edit & Bulk Connect
- Internal Monitoring Pipeline
- Projects List Screen
- AD Idea Screen
- Report Builder Architecture
- pHash Relation Matching
- SceneStealer Porting
- Databricks Decision Engine
- Creative Research Screen
- Competitor Insights Screen
- Dedup Review Components
- Fingerprint Matching Strategy
- Ad Network API Specs
- Monthly Report Pipeline
- Lessons: Security & Ops
- Vungle Report Implementation
- Bug Report
- Upload Duplicate Gate
- SensorTower Usage Alert
- Central Infra Spec
- Creative Fatigue Research
- Iteration Insights
- Network Delivery Clients
- Vungle Report Ops
- Matching Design Specs
- Auto Project Matching
- Agent Gateway Architecture
- Casual Install Correction Plan
- New Game Selection
- Dashboard Period Filter
- Central Asset Match API
- Test Review Metrics
- Casual Campaign Aggregation
- Remote MCP OAuth
- Iteration Cycle Tickets
- Project Lineage
- Docs Cleanup
- SensorTower Alert Icon
- No-Calls Alert Icon
- Casual Correction (orphan)

## God Nodes (most connected - your core abstractions)
1. `GLOSSARY` - 27 edges
2. `Creative Upload Dual (S3+Drive) Spec` - 14 edges
3. `Central DB Schema Draft` - 13 edges
4. `Vungle Creative Performance Review Design` - 12 edges
5. `Iteration Performance Phase 2 Design` - 12 edges
6. `Brief Detail (Proposal) Screen` - 12 edges
7. `drive_creatives Table` - 11 edges
8. `Competitive Insights Followups Design` - 11 edges
9. `SOV Semantics Cleanup Design` - 11 edges
10. `LESSONS_LEARNED` - 11 edges

## Surprising Connections (you probably didn't know these)
- `sensortower_store_keyword_master table` --semantically_similar_to--> `StoreKeywordMaster`  [INFERRED] [semantically similar]
  docs/superpowers/specs/2026-09-04-competitive-insights-followups-design.md → knowledge/1-GLOSSARY.md
- `UACOS User Flow (Real Screens) PDF` --semantically_similar_to--> `UACOS User Flow (Real Screens) HTML`  [INFERRED] [semantically similar]
  docs/UACOS_유저플로우_실제화면.pdf → docs/uacos-user-flow-real.html
- `AP-022 SensorTower ASO keyword 404 hidden by silent fallback` --semantically_similar_to--> `assertOkResponse fetch guard`  [INFERRED] [semantically similar]
  knowledge/4-LESSONS_LEARNED.md → docs/superpowers/specs/2026-09-04-competitive-insights-followups-design.md
- `Keyword Gap Analysis` --conceptually_related_to--> `Keyword Gap Section Removal ([티켓])`  [AMBIGUOUS]
  knowledge/1-GLOSSARY.md → docs/superpowers/specs/2026-09-08-keyword-gap-removal-design.md
- `upload_asset Duplicate Detection (creative_assets)` --semantically_similar_to--> `POST /drive-creatives/duplicate-check`  [INFERRED] [semantically similar]
  docs/superpowers/specs/2026-06-09-exact-match-search-cleanup-design.md → docs/superpowers/specs/2026-06-04-upload-duplicate-gate-design.md

## Import Cycles
- None detected.

## Hyperedges (group relationships)
- **Report Builder Get/Compose/Cache Flow** — docs_report_builder_architecture_getreportusecase, docs_report_builder_architecture_reportstorageport, docs_report_builder_architecture_metricsfetcherport, docs_report_builder_architecture_report_composer, docs_report_builder_architecture_reportdatacacheport, docs_report_builder_architecture_thumbnailresolverport [EXTRACTED 1.00]
- **Internal Monitoring Data Pipeline (Databricks → S3 → sync → Postgres → API)** — docs_architecture_internal_monitoring_architecture_ua_creative_information, docs_architecture_internal_monitoring_architecture_mart_ua_kpi_aggregate, docs_reference_databricks_job_readme_uacos_internal_dump, docs_reference_databricks_job_readme_s3_dump, docs_architecture_internal_monitoring_architecture_sync_internal_data, docs_architecture_internal_monitoring_architecture_internal_tables, docs_architecture_internal_monitoring_architecture_monitoring_backend_v1 [EXTRACTED 1.00]
- **Agent Gateway Core + Adapters** — docs_reference_agent_gateway_uacosclient, docs_reference_agent_gateway_uacos_cli, docs_reference_agent_gateway_stdio_mcp_server, docs_reference_agent_gateway_remote_http_mcp [EXTRACTED 1.00]
- **creative_tag v3 numbering flow** — docs_specs_project_unit_criteria_creative_tag_v3, docs_superpowers_plans_2026_06_01_creative_tag_v3_rework_build_creative_tag, docs_specs_creative_upload_dual_spec_backfill_tags_for_project, docs_specs_creative_upload_dual_spec_try_assign_tag_at_upload, docs_superpowers_plans_2026_06_02_creative_library_part2_register_register_creatives, docs_superpowers_plans_2026_06_02_register_edit_tags_set_creative_tag [INFERRED 0.85]
- **Creative Library ingest-register-catalog pipeline** — docs_superpowers_plans_2026_06_02_creative_library_part1_ingest_ingest_drive_folder, docs_superpowers_plans_2026_06_02_creative_library_part2_register_register_creatives, docs_superpowers_plans_2026_06_02_creative_library_part3_creative_library_page, docs_specs_creative_upload_dual_spec_drive_creatives [EXTRACTED 1.00]
- **Fingerprint-based duplicate detection** — docs_specs_creative_upload_dual_spec_duplicate_cases, docs_superpowers_plans_2026_06_04_upload_duplicate_gate_fingerprint_compute, docs_superpowers_plans_2026_06_04_upload_duplicate_gate_duplicate_check, docs_superpowers_plans_2026_06_05_dedup_review_dedup_candidates, docs_superpowers_plans_2026_06_05_dedup_review_creative_dedup_decisions [INFERRED 0.85]
- **Creative-to-project attach flow** — docs_superpowers_plans_2026_06_11_issue1_edit_attach_patch_project_id_attach, docs_superpowers_plans_2026_06_11_creatives_bulk_connect_attach_endpoint, docs_superpowers_plans_2026_06_11_project_linked_creatives_connectcreativesmodal, docs_superpowers_plans_2026_06_15_auto_project_matching_auto_link, docs_superpowers_plans_2026_06_11_issue1_edit_attach_set_lifecycle [INFERRED 0.85]
- **UACOS MCP gateway evolution (stdio -> bearer HTTP -> Okta)** — docs_superpowers_plans_2026_06_22_uacos_agent_gateway_mcp_server_stdio, docs_superpowers_plans_2026_06_22_uacos_remote_mcp_mcp_mount, docs_superpowers_plans_2026_06_24_uacos_gaia_mcp_app_mcp_server, docs_superpowers_plans_2026_06_22_uacos_agent_gateway_uacosclient [INFERRED 0.85]
- **Creative Library redesign phases** — docs_superpowers_plans_2026_06_15_creative_library_phase1, docs_superpowers_plans_2026_06_15_creative_library_phase2, docs_superpowers_plans_2026_06_15_creative_library_phase3 [EXTRACTED 1.00]
- **drive_creatives SSOT upload->register->library pipeline** — docs_superpowers_specs_2026_06_02_ssot_convergence_phase1_design_a1_upload_unification, docs_superpowers_specs_2026_06_02_ssot_convergence_phase1_design_draft_creative_tag_null, docs_superpowers_specs_2026_06_02_creative_library_design_register_endpoint, docs_superpowers_specs_2026_06_02_creative_library_design_creative_library, docs_superpowers_specs_2026_06_02_ssot_convergence_phase1_design_b2_three_tier_menu [INFERRED 0.85]
- **Campaign list end-to-end data path** — docs_superpowers_plans_2026_07_09_monitoring_campaign_backend_sync_internal_data, docs_superpowers_plans_2026_07_09_monitoring_campaign_backend_internal_creative_tables, docs_superpowers_plans_2026_07_09_monitoring_campaign_backend_pg_internal_data_store, docs_superpowers_plans_2026_07_09_monitoring_campaign_backend_filter_databricks_creatives, docs_superpowers_plans_2026_07_09_monitoring_frontend_integration_campaign_filter_ui [EXTRACTED 1.00]
- **Competitive range-too-large 413 contract chain** — docs_superpowers_plans_2026_08_31_competitive_insights_query_and_state_max_table_rows, docs_superpowers_plans_2026_08_31_competitive_insights_query_and_state_rowlimitexceedederror, docs_superpowers_plans_2026_08_31_competitive_insights_query_and_state_rangetoolargeerror, docs_superpowers_plans_2026_08_31_competitive_insights_query_and_state_userangeguard, docs_superpowers_plans_2026_09_04_competitive_insights_followups_contract_413 [INFERRED 0.85]
- **Fingerprint Dedup/Match Pipeline (F-11, F-12, F-10, F-06)** — docs_superpowers_specs_2026_06_04_upload_duplicate_gate_design_duplicate_check_endpoint, docs_superpowers_specs_2026_06_05_dedup_review_design_dedup_api, docs_superpowers_specs_2026_06_08_unified_fallback_matching_engine_design_matchingengine, docs_superpowers_specs_2026_06_09_exact_match_search_cleanup_design_dead_asset_search_endpoints, docs_superpowers_specs_2026_06_04_upload_duplicate_gate_design_phash_threshold_12 [EXTRACTED 1.00]
- **Creative → Project Linking Paths** — docs_superpowers_specs_2026_06_11_creatives_bulk_connect_design_attach_endpoint, docs_superpowers_specs_2026_06_11_issue1_edit_attach_design_patch_drive_creative_project_id, docs_superpowers_specs_2026_06_11_project_linked_creatives_design_attach_modal, docs_superpowers_specs_2026_06_15_auto_project_matching_design_auto_link_creative [INFERRED 0.85]
- **MCP Access Channel Evolution (stdio → Bearer HTTP → Okta OAuth)** — docs_superpowers_specs_2026_06_22_uacos_agent_gateway_design_mcp_server_stdio, docs_superpowers_specs_2026_06_22_uacos_remote_mcp_design_streamable_http_mount, docs_superpowers_specs_2026_06_24_uacos_gaia_mcp_design_app_mcp_separate_process, docs_superpowers_specs_2026_06_22_uacos_agent_gateway_design_monitoring_tools [EXTRACTED 1.00]
- **performance_links matching & sync pipeline** — docs_superpowers_specs_2026_07_01_iteration_performance_phase2_design_performance_matcher, docs_superpowers_specs_2026_07_01_iteration_performance_phase2_design_rebuild_performance_links, docs_superpowers_specs_2026_07_01_iteration_performance_phase2_design_performance_links, docs_superpowers_specs_2026_07_09_performance_data_sync_design_rebuild_performance_links_script, docs_superpowers_specs_2026_07_09_performance_data_sync_design_batch_chaining, docs_superpowers_specs_2026_07_01_iteration_performance_phase2_design_get_lineage_performance [INFERRED 0.85]
- **JiraAdapter consumers (UC sync + bug report)** — docs_superpowers_specs_2026_07_01_jira_sync_design_jiraadapter, docs_superpowers_specs_2026_07_01_jira_sync_design_sync_jira_graceful, docs_superpowers_specs_2026_07_23_bug_report_design_jiraadapter, docs_superpowers_specs_2026_08_10_bug_report_qa_tabs_design_fetch_statuses, docs_superpowers_specs_2026_08_10_bug_report_qa_tabs_design_reporter_retry [INFERRED 0.85]
- **Competitive Insights load reduction (cap + default range + wizard state)** — docs_superpowers_specs_2026_08_20_competitive_data_query_restructure_design_max_table_rows, docs_superpowers_specs_2026_08_20_competitive_data_query_restructure_design_daterange_helper, docs_superpowers_specs_2026_08_20_competitive_data_query_restructure_design_inflight_coalescing, docs_superpowers_specs_2026_08_31_competitive_insights_wizard_state_design_ciwizardstate, docs_superpowers_specs_2026_08_31_competitive_insights_wizard_state_design_needsselection [INFERRED 0.85]
- **SOV semantic misunderstanding chain (traffic proxy, in-app share, normalized breakdown)** — docs_superpowers_specs_2026_09_08_keyword_gap_removal_design_share_of_voice_traffic_proxy, docs_superpowers_specs_2026_09_14_sov_semantics_cleanup_design_share_is_in_app_ratio, docs_superpowers_specs_2026_09_14_sov_semantics_cleanup_design_breakdown_date_normalized_intensity, docs_superpowers_specs_2026_09_14_sov_semantics_cleanup_design_avg_daily_sov, knowledge_1_glossary_sov [INFERRED 0.85]
- **Central creative tracking model (ID anchor + fingerprints + network/performance mapping)** — knowledge_10_central_db_schema_draft_uacos_id_anchor, knowledge_10_central_db_schema_draft_creatives_table, knowledge_10_central_db_schema_draft_creative_assets_table, knowledge_10_central_db_schema_draft_network_mappings_table, knowledge_10_central_db_schema_draft_performance_links_table, knowledge_11_fingerprint_matching_strategy_three_stage_fallback_matching [INFERRED 0.85]
- **Competitor KPI reverse calculation evolution** — knowledge_7_reverse_calculation_sov_based_impression_reverse_calc, knowledge_7_1_reverse_calculation_data_analysis_creative_level_final_verdict, knowledge_7_2_reverse_calculation_redesign_calibration_coefficient_model, knowledge_7_2_reverse_calculation_redesign_competitor_creative_estimator [INFERRED 0.85]
- **Projects page composition: timeline + filters + table** — docs_assets_user_flow_01_projects_project_timeline, docs_assets_user_flow_01_projects_project_filter_bar, docs_assets_user_flow_01_projects_project_table, docs_assets_user_flow_01_projects_new_project_action [EXTRACTED 1.00]
- **AD Idea Generation Inputs** — docs_assets_user_flow_03_adidea_ad_type_multiselect, docs_assets_user_flow_03_adidea_target_audience_filters, docs_assets_user_flow_03_adidea_keywords_input, docs_assets_user_flow_03_adidea_game_context_library, docs_assets_user_flow_03_adidea_research_library_integration, docs_assets_user_flow_03_adidea_generate_idea_action [EXTRACTED 1.00]
- **Project identity naming chain (App+Year+Abbr -> label -> creative_tag)** — docs_assets_user_flow_06_newproject_basic_info_section, docs_assets_user_flow_06_newproject_project_abbr_identifier, docs_assets_user_flow_06_newproject_project_label_prefix, docs_assets_user_flow_06_newproject_creative_tag [INFERRED 0.85]
- **Creative Research Intake Flow (register or create, then list/filter)** — docs_assets_user_flow_07_research_register_existing_research, docs_assets_user_flow_07_research_new_creative_research, docs_assets_user_flow_07_research_research_document_card, docs_assets_user_flow_07_research_status_filter [INFERRED 0.75]
- **Competitive Insights Analysis Sections** — docs_assets_user_flow_08_competitor_market_overview_section, docs_assets_user_flow_08_competitor_creative_performance_section, docs_assets_user_flow_08_competitor_trend_analysis_section [EXTRACTED 1.00]
- **AI Action Classification Tiers** — docs_assets_user_flow_09_monitoring_ai_action_recommended, docs_assets_user_flow_09_monitoring_ai_action_reference, docs_assets_user_flow_09_monitoring_ai_action_last_chance, docs_assets_user_flow_09_monitoring_ai_action_monitoring [EXTRACTED 1.00]
- **Idea library list filtering dimensions (game, type, status)** — docs_assets_user_flow_10_library_list_idea_filter_bar, docs_assets_user_flow_10_library_list_idea_type, docs_assets_user_flow_10_library_list_idea_status_workflow, docs_assets_user_flow_10_library_list_dream_recipe [INFERRED 0.75]
- **Brief content structure (attributes, scenes, references, concept image)** — docs_assets_user_flow_11_brief_detail_ad_attributes, docs_assets_user_flow_11_brief_detail_scene_breakdown, docs_assets_user_flow_11_brief_detail_reference_creative, docs_assets_user_flow_11_brief_detail_concept_image_generation [INFERRED 0.85]

## Communities (72 total, 1 thin omitted)

### Community 0 - "Creative Upload & Tagging"
Cohesion: 0.05
Nodes (66): Creative Upload Dual (S3+Drive) Spec, backfill_tags_for_project, creative_tag_counter table, drive_creatives table, Duplicate cases A-E (SHA/name/pHash T2-T4), ensure_drive_folder, GoogleDriveAdapter, parseCreativeName (creativeNameParser.ts) (+58 more)

### Community 1 - "Creative Lifecycle Unification"
Cohesion: 0.07
Nodes (46): Creative Lifecycle Unification Phase 1 Plan, CreativeLifecycle single axis, drop_drive_stage_status migration, LIFECYCLE_TRANSITIONS table, lifecycle_mapping.map_to_lifecycle backfill, Transition buttons UI (drive-creatives page), validate_lifecycle_transition / next_lifecycles, Creative Versioning Plan (+38 more)

### Community 2 - "Iteration Performance Matching"
Cohesion: 0.08
Nodes (43): Project-level coverage metric, Iteration Performance Phase 2 Design, drive_creatives table, get_lineage_performance / LineagePerformanceResponse, HIGH band (>=0.70) auto-load only, internal_slots_creative / internal_casual_creative, performance_links table, performance_matcher (code anchor + token Jaccard) (+35 more)

### Community 3 - "Monitoring Dashboard Polish"
Cohesion: 0.09
Nodes (34): ComparePanel multi-series compare, [티켓], Merge Data Analysis into Monitoring, Monitoring Dashboard Polish Design, ExpandedDetail 4-column view, InternalFilterBar (Campaign/OS filters), KpiChart.tsx, useInternalCreatives hook (+26 more)

### Community 4 - "Competitive Insights Followups"
Cohesion: 0.09
Nodes (34): Competitive Insights Followups Design, /aggregate/* before /{table_name} catch-all, assertOkResponse fetch guard, Calendar Midpoint Split for SOV/CPI ([티켓]), Dead Code Cleanup ([티켓]), externalDataAdapter.ts, Keyword Gap Server Aggregation ([티켓]), Modal z-index 1500/1600 fix ([티켓]) (+26 more)

### Community 5 - "Monitoring Campaign Backend"
Cohesion: 0.09
Nodes (33): Monitoring Campaign Filter Backend Plan, campaign_list field (UPPER normalized), databricks_adapter on-demand SQL, filter_databricks_creatives domain filter, internal_slots_creative / internal_casual_creative, pg_internal_data_store, sync_internal_data.py batch, Monitoring Frontend Integration Plan (+25 more)

### Community 6 - "Creative Library Linking"
Cohesion: 0.09
Nodes (32): drive_creatives table, Creatives Bulk Connect Plan, POST /drive-creatives/attach (bulk attach), Creatives multi-select + bulk connect UI, drive-creatives list unlinked filter, Issue 1 Edit Attach Plan, creatives/new ?creative_id= entry (seed + attach-on-select), PATCH /drive-creatives/{id} project_id attach (+24 more)

### Community 7 - "UACOS Architecture Overview"
Cohesion: 0.07
Nodes (31): UACOS Backend Architecture, Clean Architecture Layers (Lv.0-8), Insight API (AI), Creative Design Module Architecture, Brick, Brick-based Assembly, BrickBlock, BriefCanvas (+23 more)

### Community 8 - "Creative Status Workflow"
Cohesion: 0.11
Nodes (29): Creative Status Workflow Design, CreativeLifecycle (8-stage single axis), creative_status_history table, derive_lifecycle / map_to_lifecycle, get_live_periods (Live Seniority), LIFECYCLE_TRANSITIONS graph, Iteration Version / Pattern Version, ROLE_LIFECYCLE_CHANGE_ALLOWED (admin/manager/producer) (+21 more)

### Community 9 - "Exact Match Search Cleanup"
Cohesion: 0.12
Nodes (28): F-06 Exact Match Search Cleanup Plan, Exact Match Search Consolidation to /match-engine, Route Absence Regression Test, search_by_checksum / search_by_phash endpoints (removed), F-10 Unified Fallback Matching Engine Plan, Hash-first Fallback (SHA -> pHash -> exact -> key_match -> none), POST /drive-creatives/match-engine, MatchingEngine usecase (+20 more)

### Community 10 - "AppsFlyer Install Correction"
Cohesion: 0.08
Nodes (28): appsflyer_install (raw audit), appsflyer_ua_kpi_aggregate, campaign_options_fetcher.py, casual_corrected_kpi.py Correction SQL Builder, COALESCE(af, mart) Freshness Fallback, GAME_CORRECTION_MAP, Mart Install Gap (30.8% missing), mart_ua_kpi_aggregate (nebulascope mart) (+20 more)

### Community 11 - "SOV Semantics"
Cohesion: 0.12
Nodes (28): SOV Semantics Cleanup Design, ad_intel/network_analysis app-level market SOV, avg_daily_sov (mean of share_of_voice), breakdown.date is self-normalized intensity (max=1.0), Creative-level daily market SOV not provided, .cursor/rules sensortower-creative-level-metrics.md (wrong premise), [티켓] hardcoded 0 removal, Two-stage decomposition for true market SOV ([티켓]) (+20 more)

### Community 12 - "Library Redesign & RBAC"
Cohesion: 0.09
Nodes (26): Creative Library Redesign (media_buyer) Design, Frontend JSZip Bulk Download, Master-Preview Layout, pickDefaultActive (-01 → first video → first), RBAC / Portal GNB Role Gating (deferred), Core 1 + Adapters 2 Architecture, mcp_server.py (stdio FastMCP), Mock Fallback meta.source Passthrough (+18 more)

### Community 13 - "Jira Sync"
Cohesion: 0.13
Nodes (25): [티켓], [티켓], Project-UC Jira Sync Design, Iteration = original ticket Sub-task, jira_sync_enabled column (js2026jirasync), JiraAdapter (sync httpx, REST v3), JiraSyncPort, render_jira_description (+17 more)

### Community 14 - "Agent Gateway Plans"
Cohesion: 0.15
Nodes (24): UACOS Agent Gateway Plan, Agent Gateway CLI (typer), Agent Gateway MCP server (FastMCP stdio), /backend/v1/monitoring API, UacosClient (httpx sync core), UACOS Remote MCP (HTTP) Plan, Pure ASGI Bearer auth wrapper (hmac.compare_digest), /mcp streamable-HTTP mount + lifespan composition (+16 more)

### Community 15 - "External Data Adapters"
Cohesion: 0.11
Nodes (20): AppMagicAdapter, Competitor API, Creative Research API, SensorTowerAdapter, SensorTower API — Market Analysis, GET /v1/{os}/ad_intel/creatives/top, GET /v1/{os}/ad_intel/top_apps, SensorTower API — Custom Fields & App Metadata (+12 more)

### Community 16 - "Monitoring AI Actions (UI)"
Cohesion: 0.14
Nodes (20): AI Action Criteria Panel, AI Action: Last Chance, AI Action: Monitoring, AI Action: Recommended, AI Action: Reference, AI Iteration Suggestion Banner, AppsFlyer, Bug Report Button (+12 more)

### Community 17 - "Competitive Insights Query"
Cohesion: 0.16
Nodes (19): Competitive Insights Query and Wizard State Plan, ciWizardState sessionStorage helper, dateRange default 30-day helper, Two GameContext types (page vs adapter), MAX_TABLE_ROWS = 50,000, needsSelection response (no unfiltered scan), pg_competitive_data_store.query_table, RangeTooLargeError (FE adapter) (+11 more)

### Community 18 - "Project-Creative Attach"
Cohesion: 0.15
Nodes (16): drive_creatives Table, attach_creatives_to_project (Port+Adapter), POST /drive-creatives/attach, DriveCreativeAttachRequest, HITL Bulk Linking (5,482 CVS creatives), POST /projects/{id}/creatives/register (tag numbering), list_drive_creatives unlinked Filter, Projects LINKED CREATIVES Fix + Attach Design (+8 more)

### Community 19 - "Monitoring Custom Views"
Cohesion: 0.23
Nodes (14): useInternalCreatives hook, Monitoring Custom Views Plan, encodeViewState/decodeViewState (wraps URL codec), MONITORING_DASHBOARD_KEY / MAX_VIEWS_PER_DASHBOARD=30, saved_views CRUD router, savedViews API client + SavedViewError, SaveViewModal component, UserSavedViewModel / user_saved_views table (+6 more)

### Community 20 - "Brief Detail Screen"
Cohesion: 0.22
Nodes (13): Brief Detail (Proposal) Screen, Ad Attributes (Ad Type, 제작, 난이도, 예상 CTR), AD Idea (Creative Planning), Brief Builder, Concept Image Generation, Creative Library (라이브러리), Deliverables (산출물: Figma Link + Planning PDF), Dream Recipe (+5 more)

### Community 21 - "Channel Activity Monitoring"
Cohesion: 0.27
Nodes (13): GET /monitoring/channel-activity, Channel Activity Monitoring Design, get_channel_activity MCP tool, internal_slots_creative / internal_casual_creative, last_date approximation of channel activity, query_channel_activity (pg_internal_data_store), UacosClient.get_channel_activity, MCP Usage Monitoring Design (+5 more)

### Community 22 - "Central DB Schema"
Cohesion: 0.26
Nodes (13): Central DB Schema Draft, creative_assets table, creatives table, Data Disconnection Points D1-D3, network_mappings table, performance_links table, projects table, UACOS ID as single source of truth (CRV-YYYY-NNNN) (+5 more)

### Community 23 - "New Project Screen"
Cohesion: 0.21
Nodes (12): Project Basic Info Form (App, Year, start/end date, fullname, Reviewing team, CP, Designer, Status, Seasonal), creative_tag (label + designer_id-NN assigned at creative registration), Iteration Settings (source project + iteration version), Jira Integration Panel (auto-create ticket / link existing ticket), Jira Ticket Parameters (Theme, Type of Creative, File Format, Video Ratio, Video Length, Proposal link, description preview), New Project Screen (UACOS user flow 06), Pattern / Version (sub-level reskin under iteration), Project Abbr Identifier (1-8 alnum, uppercased label) (+4 more)

### Community 24 - "Idea Library Screen"
Cohesion: 0.23
Nodes (12): AD Idea (Creative Planning), Bug Report Button (header), Club Vegas Slots (game), Creative Library (nav item), Dream Recipe (game), Idea Search & Filter Bar (game/type/status), Idea Library Screen (AD Idea list), Idea Status Workflow (작성중/진행중) (+4 more)

### Community 25 - "Report Degrade Policy"
Cohesion: 0.24
Nodes (12): Prod DB Access Rules, GET /reports/{id} is a Write Path, Failure-as-Default-Value Anti-pattern, source_degraded flag (skip cache write), Degrade Policy (SensorTower/GDrive degrade, Databricks fail), GetReportUseCase, Hybrid Data Strategy (spec + 24h cache + refresh), MetricsFetcherPort (+4 more)

### Community 26 - "Review Process Design"
Cohesion: 0.23
Nodes (12): Review Process & Settings Design, Rejection Templates, Review state DRAFT->REVIEW_REQUESTED->APPROVED, Category-based reviewer auto-assignment, reviews[] multi-reviewer model, SLA reminders & Slack escalation, SensorTower Daily Usage Slack Alert Plan, run-batch.yml cron 01:00 UTC (+4 more)

### Community 27 - "Central Dashboard Tracks"
Cohesion: 0.23
Nodes (12): Central Dashboard Track 1 Plan, Dnipro team 'UAC DP', formatUserDisplay 'English (Korean)', Gantt bar project_name join, Central Dashboard Track 3 Gantt Drag Plan, Assignment PATCH role lock (admin/manager), canEditSchedule helper, computeDraggedDates (UTC day snap) (+4 more)

### Community 28 - "Vungle Report Design"
Cohesion: 0.26
Nodes (12): Vungle Creative Performance Review Design, KPI delta polarity rule, for_master_ua_dashboard_actual table, Hybrid color tokens (Navy+Teal report / Orange chrome), Vungle-dedicated module (Rule of Three), Anthropic LLM insights client (llm_client.py), NEW creative detection (in target not prior), vungle_pdf_renderer (ReportLab) (+4 more)

### Community 29 - "Prod OOM & Query Limits"
Cohesion: 0.24
Nodes (12): [티켓] prod OOM, [티켓], dateRange.ts default 30-day helper, Competitive Data Query Restructure Design, In-flight request coalescing, MAX_TABLE_ROWS 50,000 + HTTP 413 range_too_large, RangeTooLargeError (externalDataAdapter), ciWizardState single sessionStorage key (+4 more)

### Community 30 - "Human-in-the-Loop Principles"
Cohesion: 0.24
Nodes (12): Phased Mapping Strategy (post-registration -> hub -> automation), AgenticWorkflow (Detect-Decide-Approve-Execute-Audit), ApproveRule, AuditRule, Human-in-the-Loop, PI-001 Automation Paradox, DF-002 Human-in-the-Loop scope, Audit Creative Evaluation (+4 more)

### Community 31 - "Glossary Core Concepts"
Cohesion: 0.23
Nodes (12): GLOSSARY, Brick, Creative Planning (UACOS), Creative Tag, Decision Engine, Keyword Gap Analysis, MAINTAIN / OBSERVE / REPLACE statuses, PlanningDoc (+4 more)

### Community 32 - "Creative Edit & Bulk Connect"
Cohesion: 0.22
Nodes (11): Creatives Bulk Connect to Project Design, Issue 1 — Creatives Edit Button Attach Design, DriveCreativeStagePatch, PATCH /drive-creatives/{id} project_id Field, set_lifecycle Repository Method, DELIVERY_NETWORKS SSOT, NetworkMultiSelect (portal top-layer), planned_networks Column (JSONB) (+3 more)

### Community 33 - "Internal Monitoring Pipeline"
Cohesion: 0.27
Nodes (10): Internal Monitoring Dashboard Architecture, nebulascope_mart_prod.mart_ua_kpi_aggregate (Casual), sync_internal_data.py Daily Batch, company_tableau_etl.ua_creative_information (Slots), Databricks Job — Internal Monitoring Data Dump, s3://[운영 버킷] Parquet Dump, uacos_internal_dump Notebook / UACOS_internal_dump_job, Bagel Drive Gateway OAuth Refresh Token (+2 more)

### Community 34 - "Projects List Screen"
Cohesion: 0.24
Nodes (10): Creative Management Section (Dashboard, Projects, Creatives, Creative Library, Network Delivery, Settings), Jira Ticket Link per Project, New Project Action, Project Filter Bar (App, Designer, Reviewing Team, Seasonal, Status, Pattern, Year, Month, Live, Search), Project Status Lifecycle (draft, in_production, delivered, live, archived), Project Table (ID, App, Abbr, Project Name, CP, Jira, Reviewer, Status, Period), Project Timeline (monthly/yearly Gantt), Projects Page (+2 more)

### Community 35 - "AD Idea Screen"
Cohesion: 0.27
Nodes (10): AD Idea Generation Screen (UI Screenshot), Ad Type Multi-Select (Gameplay/Story/Hook/Fake/Playable/UGC), Favorites and History, Game Context Library, Game Tabs (Dream Recipe / Club Vegas Slots), Generate Idea Action, Keyword Input (max 5) and Generation Count, Research Library Competitor Analysis Integration (+2 more)

### Community 36 - "Report Builder Architecture"
Cohesion: 0.22
Nodes (10): docs/ Placement Rules, Document Placement & Deletion Policy, Report Builder Architecture, Figma Injection Points (PDF 20p → 9 components), PermissionGuard (report:view/create/edit/delete via central RBAC), report_composer.compose(), ReportSpec, Report Builder TODO (+2 more)

### Community 37 - "pHash Relation Matching"
Cohesion: 0.24
Nodes (10): pHash Hamming Threshold 12 (bit_count SQL), GET /drive-creatives/{id}/related, Shared bit_count Candidate SQL Helper, central_types pHash Constants (PHASH_BITS, DEFAULT_PHASH_THRESHOLD...), /drive-creatives/match and /match-batch, MatchingEngine Usecase, MatchingRepository Port, MatchQuery (+2 more)

### Community 38 - "SceneStealer Porting"
Cohesion: 0.22
Nodes (10): AI Proxy, Knolling, Style Sync, SceneStealer Porting Design, Asset Gallery, Asset Generator (Image/Video to Asset, Style Sync), gemini-3-pro-image-preview (1K fixed), Grey-background Knolling -> Canvas background removal (+2 more)

### Community 39 - "Databricks Decision Engine"
Cohesion: 0.25
Nodes (9): Databricks as Single Source of Truth (early design), DatabricksClient, MAINTAIN/OBSERVE/REPLACE Decision Engine, Monitoring API (/api/monitoring/*), Planning API, AppsFlyer Install Correction (appsflyer_cost.installs), internal_casual_creative / internal_daily_metrics / internal_slots_creative, /backend/v1/monitoring/* endpoints (+1 more)

### Community 40 - "Creative Research Screen"
Cohesion: 0.31
Nodes (9): Bug Report Button, Creative Research, New Creative Research (Trend Analysis, Insight, Report), Register Existing Research Document (PDF / Drive / URL), Research Document Card (genre, games, creatives, date), Creative Research List Screen (User Flow 07), UACOS Sidebar Navigation (Planning / Monitoring / Production / Management), Research Status Filter (All / Completed / Draft) (+1 more)

### Community 41 - "Competitor Insights Screen"
Cohesion: 0.36
Nodes (9): Floating Compare Performance Action Bar, Competitive Insights Page (Screenshot), Section 2: Creative Performance (Top 10 by Impressions), Explore-Compare-Insights 3-Step Wizard, Section 1: Market Overview (Spend vs Market Share), SensorTower Competitor Data, Step 1 Explore: Competitor vs Own Game Selection, Section 3: Trend Analysis (Impressions SOV Time Series) (+1 more)

### Community 42 - "Dedup Review Components"
Cohesion: 0.22
Nodes (9): DuplicateWarning Component, Append-only Decision History, creative_dedup_decisions Table, Register Creative Page (creatives/new), Dedup API (dedup-candidates / dedup-decisions), DedupReview Component, On-demand Candidates, Project-scoped (Approach A), Attach Joins Existing Register Flow (+1 more)

### Community 43 - "Fingerprint Matching Strategy"
Cohesion: 0.31
Nodes (9): Fingerprint Matching Strategy, asset_storage.py hashing (sha256, imagehash.phash, ffmpeg frame), creative_dedup_decisions audit (F-12), 3-Stage Fallback Matching (SHA-256 -> pHash -> manual), Unified Fallback Matching Engine (F-10, /drive-creatives/match-engine), Checksum (SHA-256), Match Method, Perceptual Hash (+1 more)

### Community 44 - "Ad Network API Specs"
Cohesion: 0.33
Nodes (9): Meta Marketing API Spec, Meta Insights API (async reports, breakdowns), Meta Marketing API v25.0, Meta rate limit tiers (spend-proportional), Google Ads API Spec, Developer Token Tier, Google Ads API (gRPC, GAQL), Immutable Ads / Non-deletable Assets (+1 more)

### Community 45 - "Monthly Report Pipeline"
Cohesion: 0.33
Nodes (9): Monthly Report Data Pipeline, Casual install correction (appsflyer, PR/#149), Game Category Branching (Slots vs Casual install definitions), LayoutOverride / textOverrides system, mart_ua_kpi_aggregate (nebulascope/Adjust, Casual), normalize_creative_id (G-52), Report Builder Extensibility Phase, Slots Creative Review click inflation (unresolved) (+1 more)

### Community 46 - "Lessons: Security & Ops"
Cohesion: 0.22
Nodes (9): AppMagic, Path Traversal Prevention, LESSONS_LEARNED, AP-007 Missing path traversal defense on local file serve, AP-017 Google Ads Developer Token level separate from MCC, AP-021 Same-EC2 workflows missing concurrency, AP-023 AppMagic application-ads needs 2-step call, AP-024 Branch deploy failure was host disk full (+1 more)

### Community 47 - "Vungle Report Implementation"
Cohesion: 0.32
Nodes (8): Vungle Creative Performance Review Plan, LLMClientPort + Anthropic adapter, vungle_insights_llm, vungle_metrics_fetcher (Databricks), vungle_pdf_renderer (ReportLab), MoM delta + NEW detection domain, vungle_reports PG table, Vungle 5-step wizard (Step1-5)

### Community 48 - "Bug Report"
Cohesion: 0.46
Nodes (8): Bug Report Plan, POST /backend/v1/bug-report, BugReport model + br2026bugreport migration, BugReportDialog + Header button, Global error ring buffer (20 entries), error.tsx report CTA, JiraAdapter issue-type creation, slack_notifier.send_slack_via_bot (uacos_bot)

### Community 49 - "Upload Duplicate Gate"
Cohesion: 0.25
Nodes (8): POST /drive-creatives/duplicate-check, Fingerprint Saved at Registration, manual-upload link_creative_tag Parameter, pHash Perceptual Fingerprint (4-frame majority vote), SHA-256 Exact Fingerprint, Warn-not-block Duplicate Policy, auto_confirmable Flag (HITL), MatchEngineResult / BestMatch / MatchCandidate

### Community 50 - "SensorTower Usage Alert"
Cohesion: 0.25
Nodes (8): SensorTower Daily Usage Slack Alert Design, sensortower_daily_usage_alert.py Script, api_counters.json, SENSORTOWER_MONTHLY_CALL_LIMIT (50,000), run-batch.yml Workflow (cron 01:00 UTC), send_slack_via_bot (chat.postMessage), SensorTowerCallCounter (daily extension), slack_bot_token Config (op:// ref)

### Community 51 - "Central Infra Spec"
Cohesion: 0.32
Nodes (8): Central Infra Spec, 50GB gp3 /data volume, S3 storage (pending approval, FileStoragePort swap), EC2 t3.large (vs m6i.large) decision, Local File Storage, Storage Factory, TI-018 Port-Adapter lowers infra swap cost, DS-012 Port-Adapter + Factory to minimize infra swap

### Community 52 - "Creative Fatigue Research"
Cohesion: 0.39
Nodes (8): Creative Fatigue, Reference Research R5 Ideation, Aprimo Agentic DAM (Critic Agent etc.), Focal Creative Boards (Slack/Figma), Segwise fatigue detection, Smartly.io Creative Predictive Potential, To-Be flow: AI evaluation + Human gates + fatigue monitoring, Ziflow sequential stage approval

### Community 53 - "Iteration Insights"
Cohesion: 0.29
Nodes (8): Iteration, TrendStatus, INSIGHT, BI-006 AI should synthesize, not generate, BI-019 Decline detection -> Iteration workflow, TI-005 Single data source limitation, TI-032 SSOT transition cost is boundary noise, TI-034 External API paths need response-structure tests

### Community 54 - "Network Delivery Clients"
Cohesion: 0.33
Nodes (7): AppsFlyer API Investigation (no creative asset URLs), Google Drive Creative Preview, Network Delivery Status, Google Ads Client (gRPC SDK), Meta Ads Client, network_accounts / network_mappings tables, Unity Ads Client

### Community 55 - "Vungle Report Ops"
Cohesion: 0.29
Nodes (7): Vungle Report Ops Notes, gemini_client.fetch_gemini (Insights), Vungle ObjectId 24-hex Suffix Normalization, thumbnail_resolver_pg (drive_creatives), vungle_metrics_fetcher (for_master_ua_dashboard_actual), Vungle PDF Renderer (ReportLab A4 5p), ThumbnailResolverPort

### Community 56 - "Matching Design Specs"
Cohesion: 0.33
Nodes (7): Upload Duplicate Gate (F-11) Design, Dedup Review Workflow (F-12) Design, F-10 Unified Fallback Matching Engine Design, knowledge/11-FINGERPRINT_MATCHING_STRATEGY.md, Hash-first Fallback Chain (SHA → pHash → name → none), F-06 Exact Match Search API Cleanup Design, Phase 2 Iteration Performance Comparison (performance_links)

### Community 57 - "Auto Project Matching"
Cohesion: 0.29
Nodes (7): performance_matcher.find_best_match, Creative ↔ Project Auto Linking Design, GET /creative-link-log, creative_project_link_log Table, scripts/match_creatives_to_projects.py, project_matcher (normalize / match_project), relink_unlinked_for_project

### Community 58 - "Agent Gateway Architecture"
Cohesion: 0.33
Nodes (6): X-API-Key Auth Middleware, UACOS Agent Gateway (CLI · MCP), Remote HTTP MCP (uacos-mcp, Okta OAuth), Local stdio MCP Server, uacos CLI (typer), UacosClient

### Community 59 - "Casual Install Correction Plan"
Cohesion: 0.53
Nodes (6): AppsFlyer Install Correction Plan, casual_corrected_kpi SQL builder, casual_correction contracts (mart code -> appsflyer app_id map), Corrected casual base subquery (mart LEFT JOIN af UNION ALL af-only), Prod SSM docker exec verification, verify_install_correction script

### Community 60 - "New Game Selection"
Cohesion: 0.53
Nodes (6): build_corrected_casual_source allowed_apps whitelist, Casual fetchers per-request threading, [티켓], New Game Selection Design, NewGameSelection (spend_threshold, included_apps), PR (Facebook install correction)

### Community 61 - "Dashboard Period Filter"
Cohesion: 0.80
Nodes (5): Central Dashboard Track 2 Period Filter Plan, cast(col, Date) date comparison, dashboard-stats start_date/end_date, drive-creatives list period filter (source_date), Dashboard period filter (All/7d/14d/30d/90d)

### Community 62 - "Central Asset Match API"
Cohesion: 0.40
Nodes (5): POST /drive-creatives/match-engine, CentralRepositoryPort.find_asset_by_checksum / find_assets_by_phash, creative_assets Corpus, Removed /central/assets/search/checksum & /phash, upload_asset Duplicate Detection (creative_assets)

### Community 63 - "Test Review Metrics"
Cohesion: 0.40
Nodes (5): Creative Test Review Campaign Filter by App Design, PR / [티켓] (fix/report_builder bundle), IPM Metric + Step6 Default Metric Order Design, DEFAULT_METRICS (eCVR, CPI, CTR, CR, Spend, Install), Test Review Status Chip UPDATING + Single Select Design

### Community 64 - "Casual Campaign Aggregation"
Cohesion: 0.83
Nodes (4): Casual Campaign Aggregation Plan, CampaignAggregationGroup / ReportSpec.casualCampaignGroups, CasualReviewTab grouping UI, report_composer group aggregation

### Community 65 - "Remote MCP OAuth"
Cohesion: 0.50
Nodes (4): UACOS Agent Gateway (CLI + MCP) Design, Remote MCP (HTTP, Bearer) Design, UACOS MCP Gaia (Okta) OAuth Design, UAOS PR (Okta MCP reference)

### Community 66 - "Iteration Cycle Tickets"
Cohesion: 0.50
Nodes (4): Creative Stage/Status Lifecycle Unification Design, [티켓], Iteration Cycle (Project-level) Design, [티켓]

### Community 67 - "Project Lineage"
Cohesion: 0.50
Nodes (4): Removed Creative-level Iteration (parent_creative_id, live_since), Explicit Detach (NULL vs unchanged), projects.parent_project_id (self-FK), GET /projects/{id}/lineage

### Community 68 - "Docs Cleanup"
Cohesion: 0.50
Nodes (4): context.md Drive OAuth knowledge absorption, Docs Cleanup Design, Full deletion of Tier 1-4 docs via git rm, architecture/specs/reference folder structure

### Community 69 - "SensorTower Alert Icon"
Cohesion: 0.67
Nodes (3): Broadcast Antenna Motif (teal circular badge), SensorTower Alert Slack Icon, SensorTower Slack Alert Bot

### Community 70 - "No-Calls Alert Icon"
Cohesion: 0.67
Nodes (3): SensorTower No-Calls Alert Icon, Broadcast Antenna Glyph (monochrome signal icon), SensorTower No-Calls Slack Alert

## Ambiguous Edges - Review These
- `Databricks as Single Source of Truth (early design)` → `internal_casual_creative / internal_daily_metrics / internal_slots_creative`  [AMBIGUOUS]
  docs/architecture/BACKEND_ARCHITECTURE.md · relation: conceptually_related_to
- `SLA reminders & Slack escalation` → `send_slack_message (webhook_url override)`  [AMBIGUOUS]
  docs/specs/REVIEW_PROCESS_DESIGN.md · relation: conceptually_related_to
- `HITL Bulk Linking (5,482 CVS creatives)` → `Single-match-only Auto Link + Post Log`  [AMBIGUOUS]
  docs/superpowers/specs/2026-06-15-auto-project-matching-design.md · relation: conceptually_related_to
- `Report CreativeStatus (+UPDATING)` → `Legacy CreativeStage / CreativeStatus (2-axis)`  [AMBIGUOUS]
  docs/superpowers/specs/2026-06-19-status-chip-updating-single-select.md · relation: semantically_similar_to
- `Keyword Gap Section Removal ([티켓])` → `Keyword Gap Analysis`  [AMBIGUOUS]
  knowledge/1-GLOSSARY.md · relation: conceptually_related_to
- `ad_intel/creatives share = in-app ratio (sums to 1.0 per app)` → `SOV-based impression reverse calculation (Y / X%)`  [AMBIGUOUS]
  docs/superpowers/specs/2026-09-14-sov-semantics-cleanup-design.md · relation: conceptually_related_to

## Knowledge Gaps
- **194 isolated node(s):** `docs/ Placement Rules`, `Idea Library (list replaces Kanban)`, `Brief Builder Figma Plugin (standalone zip)`, `Competitive Insights`, `Creative Research / Research Library` (+189 more)
  These have ≤1 connection - possible missing edges or undocumented components.
- **1 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **What is the exact relationship between `Databricks as Single Source of Truth (early design)` and `internal_casual_creative / internal_daily_metrics / internal_slots_creative`?**
  _Edge tagged AMBIGUOUS (relation: conceptually_related_to) - confidence is low._
- **What is the exact relationship between `SLA reminders & Slack escalation` and `send_slack_message (webhook_url override)`?**
  _Edge tagged AMBIGUOUS (relation: conceptually_related_to) - confidence is low._
- **What is the exact relationship between `HITL Bulk Linking (5,482 CVS creatives)` and `Single-match-only Auto Link + Post Log`?**
  _Edge tagged AMBIGUOUS (relation: conceptually_related_to) - confidence is low._
- **What is the exact relationship between `Report CreativeStatus (+UPDATING)` and `Legacy CreativeStage / CreativeStatus (2-axis)`?**
  _Edge tagged AMBIGUOUS (relation: semantically_similar_to) - confidence is low._
- **What is the exact relationship between `Keyword Gap Section Removal ([티켓])` and `Keyword Gap Analysis`?**
  _Edge tagged AMBIGUOUS (relation: conceptually_related_to) - confidence is low._
- **What is the exact relationship between `ad_intel/creatives share = in-app ratio (sums to 1.0 per app)` and `SOV-based impression reverse calculation (Y / X%)`?**
  _Edge tagged AMBIGUOUS (relation: conceptually_related_to) - confidence is low._
- **Why does `GLOSSARY` connect `Glossary Core Concepts` to `SceneStealer Porting`, `Fingerprint Matching Strategy`, `SOV Semantics`, `Lessons: Security & Ops`, `Central Infra Spec`, `Creative Fatigue Research`, `Iteration Insights`, `Human-in-the-Loop Principles`?**
  _High betweenness centrality (0.011) - this node is a cross-community bridge._