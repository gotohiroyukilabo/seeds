# Executive Summary: Antibody Seed Proposals

調査日: 2026-07-05

## 結論

自己免疫・免疫介在性疾患を中心に、抗体医薬シーズ候補を以下の3件に絞る。

| Rank | Seed proposal | Target | Disease focus | Antibody concept | Recommendation |
|---:|---|---|---|---|---|
| 1 | BAFF-R選択的B細胞制御抗体 | BAFF receptor / TNFRSF13C | Sjogren diseaseを中心とするB-cell-high自己免疫疾患 | Fc-silent blocking antibody、または限定的Fc-enabled antibody | High |
| 2 | IL-36-high皮膚炎症サブセット向けIL-36R抗体 | IL-36 receptor / IL1RL2 | Hidradenitis suppurativa、好中球性/上皮炎症性皮膚疾患 | Fc-silent blocking antibody | Medium-High |
| 3 | 線維化自己免疫疾患向けCCL24中和抗体 | CCL24 / eotaxin-2 | Systemic sclerosis、PSC様線維化疾患 | Neutralizing antibody、またはpH-dependent recycling antibody | Medium-High |

## 選定理由

1. **BAFF-R / Sjogren disease**
   - B細胞病態、自己抗体、BAFF軸が疾患仮説と整合する。
   - BAFF ligand阻害やCD20枯渇と異なる、受容体選択的かつFc調整可能なB細胞制御を提案できる。
   - ただし ianalumab 競合があり、患者選択とFc設計で差別化できない場合は弱い。

2. **IL-36R / HS・好中球性皮膚炎**
   - IL-36Rは抗体で狙いやすく、GPPで臨床的にdrugged targetである。
   - HSではTNF/IL-17後の非奏効、疼痛、排膿、慢性炎症が残る。
   - 最大の課題は、HSの中にIL-36依存サブセットが本当にあるか。

3. **CCL24 / systemic sclerosis・線維化自己免疫**
   - SScなど線維化疾患のunmet needは大きく、競合過密度はB細胞/IL-6軸より低い。
   - 分泌ケモカインで抗体中和に適し、炎症と線維化をつなぐ仮説を置ける。
   - 最大の課題は、CCL24が単なるマーカーではなくドライバーか、またCCL11/CCL26などの冗長性を超えられるか。

## 今回あえて外した候補

| Target | 理由 |
|---|---|
| CD40L | 生物学は強いが、血小板/血栓リスクが歴史的に大きく、競合も活発。安全フォーマットの独自性がないと提案リスクが高い。 |
| OSMR | 差別化仮説は魅力的だが、自己免疫/線維化疾患での因果性と臨床証拠成熟度がまだ弱い。第2波候補として残す。 |

## 共通のGo / No-Go思想

- **Go:** ヒト疾患組織または患者由来細胞で、標的発現、機能依存性、抗体介入による疾患関連readout改善が揃う。
- **No-Go:** 標的発現だけで機能依存性が示せない、既存薬との差別化がex vivoで見えない、安全性またはPK上の実装可能性が低い。

## Next step

最初の3か月は候補を増やすより、3件それぞれについてヒトサンプルベースの検証系を組み、Target Cardのkill criteriaを実験で判定する。
