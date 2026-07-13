# Antibody Design Options: BAFF receptor / TNFRSF13C

Target Card: `targets/target_cards/BAFFR_TNFRSF13C.md`

## Design summary

推奨設計: `blocking antibody` または `Fc-silent blocking antibody`。疾患・患者層によっては、限定的なB細胞除去を狙う `Fc-enhanced antibody` も検討余地あり。

| Design | Initial fit | Mechanism of action | Expected benefit | Differentiation vs existing drugs | Safety risk | Developability risk | Initial assays | Kill criteria |
|---|---|---|---|---|---|---|---|---|
| Blocking antibody | High | BAFF-RへのBAFF結合を阻害し、BAFF依存性B細胞生存を抑える。 | BAFF ligand blockadeより受容体選択的。B細胞サブセットへの作用を調整しやすい。 | BelimumabなどBAFF ligand阻害と異なり、BAFF-R陽性B細胞へ直接作用する点。 | 感染、低IgG、ワクチン応答低下。 | 受容体占有率、内在化、遊離BAFF濃度による薬効変動。 | BAFF依存B細胞生存 assay、受容体占有率、自己免疫患者PBMC assay。 | BAFF-R blockadeがBAFF ligand阻害より優位性を示さない。 |
| Agonistic antibody | Low | BAFF-Rを架橋/刺激する。 | 免疫賦活が目的なら理論上可能。 | 自己免疫では既存薬との差別化以前に病態悪化リスクが高い。 | B細胞活性化、自己抗体増加、疾患悪化。 | アゴニズム制御が難しい。 | B細胞活性化、Ig産生、NF-kB readout。 | B細胞活性化または自己抗体産生が上昇。 |
| Fc-silent antibody | High | BAFF-R blockadeに限定し、ADCC/CDCを抑える。 | 慢性自己免疫で安全域を広げやすい。 | Ianalumab型のdepleting設計と比較して、安全性・慢性投与性で差別化可能。 | 免疫抑制は残る。十分なB細胞制御が得られない可能性。 | Fc silence、半減期、免疫原性。 | FcγR binding、CDC/ADCC陰性確認、BAFF blockade。 | Fc-silent化で薬効が不十分、または受容体占有に高用量が必要。 |
| Fc-enhanced antibody | Medium | BAFF-R陽性B細胞をADCC/ADCPで除去しつつBAFF-Rを阻害。 | 自己反応性B細胞除去が必要な患者で強い薬効を狙える。 | CD20より成熟B細胞選択性が異なる可能性。 | 過度なB細胞減少、感染、低IgG。 | Fc effectorのばらつき、標的発現量依存、組織B細胞到達性。 | ADCC/ADCP、B細胞サブセット別殺傷、IgG低下予測。 | CD20/CD19枯渇療法と安全性・有効性で差別化できない。 |
| Bispecific antibody | Medium-Low | BAFF-R x 別標的でB細胞選択性や抑制シグナルを追加する。 | B細胞活性化high患者で精密制御できる可能性。 | BAFF-R単独より患者選択・作用選択性を高められる仮説。 | 予期せぬB細胞活性化、過剰免疫抑制。 | CMC複雑化、鎖ミスマッチ、安定性、免疫原性。 | Dual binding、B-cell functional assay、cytokine release。 | 単抗体より明確な機能差がない、またはCMCが重い。 |
| ADC | Low | BAFF-R陽性細胞へ毒素を送達。 | B細胞腫瘍なら検討余地。自己免疫では過剰。 | 自己免疫治療では既存B細胞枯渇薬より安全性で劣る可能性。 | 骨髄抑制、肝毒性、オフターゲット毒性、長期免疫不全。 | DAR、リンカー安定性、payload毒性。 | 細胞内移行、payload killing、正常B細胞毒性。 | 正常B細胞への強い毒性、治療域が狭い。 |
| Masked antibody | Medium | 炎症組織プロテアーゼなどでBAFF-R結合を局所活性化。 | 全身B細胞抑制を下げる可能性。 | 慢性自己免疫で安全性差別化が可能な仮説。 | 活性化部位の不確実性、組織外活性化。 | Mask cleavage設計、活性化率、製造複雑性。 | 疾患組織プロテアーゼ切断、masked/unmasked affinity、ex vivo tissue assay。 | 疾患組織で選択的活性化しない。 |
| pH-dependent recycling antibody | Medium | 中性pHでBAFF-R/BAFFに結合し、酸性エンドソームで解離して再利用または抗原クリアランスを改善。 | 投与間隔延長、抗原sink対策。 | 高BAFF環境や慢性投与でPK/PD差別化可能。 | 長期B細胞抑制、予測困難なターゲット占有。 | pH選択性と中性pH affinityの両立。 | pH-dependent binding、FcRn binding、receptor occupancy PK/PD model。 | pH依存性が薬効または投与量に寄与しない。 |

## Initial recommendation

最初は `Fc-silent blocking antibody` と `moderately Fc-enabled blocking/depleting antibody` の2案を比較する。自己免疫での慢性投与を考えると、安全性重視のFc-silent案を主案、B細胞除去が必要な高活動性患者向けにFc-enabled案を副案とする。
