# Antibody Seed Research

目的:
会社で提案する新規抗体医薬シーズテーマを探索する。

検討対象:
- 標的疾患
- 標的タンパク質
- 抗体モダリティ
- 作用機序
- 競合との差別化
- 開発可能性
- 提案ストーリー

優先疾患領域:
- 免疫分野、特に自己免疫疾患を中心に検討する。
- 必要に応じて、炎症性疾患、線維化、希少免疫疾患など自己免疫疾患と隣接する領域も比較対象として扱う。

最終成果物:
- 3〜5個のシーズ候補
- 各候補の疾患背景、標的妥当性、抗体設計案、リスク、次の検証実験
- 社内提案用の1〜2ページ要約

## Repository Structure Plan

リサーチは以下のフォルダ構成を目安に進める。新しい調査メモ、根拠文献、評価表、提案書ドラフトは、内容に応じて該当する場所に保存する。

```text
antibody_seed_research/
├── README.md
├── INSTRUCTIONS.md
├── criteria/
│   ├── disease_selection_criteria.md
│   ├── target_selection_criteria.md
│   ├── antibody_design_criteria.md
│   └── scoring_rubric.md
├── inputs/
│   ├── company_constraints.md
│   ├── modality_preferences.md
│   ├── excluded_areas.md
│   └── seed_questions.md
├── disease_landscape/
│   ├── autoimmune/
│   ├── oncology/
│   ├── fibrosis/
│   ├── metabolic/
│   └── rare_disease/
├── targets/
│   ├── target_shortlist.tsv
│   ├── target_cards/
│   │   ├── TEMPLATE.md
│   │   └── example_target.md
│   └── rejected_targets.md
├── antibodies/
│   ├── design_options/
│   ├── modality_notes/
│   ├── developability_risks.md
│   └── engineering_strategies.md
├── evidence/
│   ├── papers/
│   ├── clinical_trials/
│   ├── patents/
│   ├── omics/
│   └── competitive_landscape/
├── analysis/
│   ├── disease_target_matrix.tsv
│   ├── scoring_table.tsv
│   ├── ranking_notes.md
│   └── sensitivity_analysis.md
├── outputs/
│   ├── seed_proposal_1.md
│   ├── seed_proposal_2.md
│   ├── executive_summary.md
│   └── slide_outline.md
├── for_me/
│   └── proposal_1_detailed_report.md
└── scripts/
    ├── literature_table_builder.py
    ├── scoring_table_checker.py
    └── citation_checker.py
```
