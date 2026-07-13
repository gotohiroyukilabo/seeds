# Antibody Design Options: CCL24 / eotaxin-2

Target Card: `targets/target_cards/CCL24.md`

## Design summary

推奨設計: `blocking antibody` または `pH-dependent recycling antibody`。CCL24は分泌ケモカインなので、中和抗体が最も自然。抗原sinkや慢性投与を考える場合、pH依存リサイクリング設計を比較する。

| Design | Initial fit | Mechanism of action | Expected benefit | Differentiation vs existing drugs | Safety risk | Developability risk | Initial assays | Kill criteria |
|---|---|---|---|---|---|---|---|---|
| Blocking antibody | High | CCL24を中和し、CCR3を介する好酸球/炎症細胞遊走と線維化関連シグナルを抑える。 | 分泌標的で抗体中和に適する。 | IL-6/B-cell/TGF-beta系と異なるchemokine-fibrosis軸。 | 好酸球機能、寄生虫/アレルギー応答、感染防御への影響。 | chemokine redundancy、抗原sink、組織濃度。 | CCL24-CCR3 chemotaxis、SSc skin/lung explant、fibroblast assay。 | CCL24中和でヒト疾患組織readoutが変わらない。 |
| Agonistic antibody | Low | CCL24活性を増強する。 | 自己免疫・線維化では不要。 | なし。 | 炎症/線維化悪化、好酸球増加。 | 意図したagonism困難。 | Chemotaxis enhancement assay。 | 遊走/炎症促進。 |
| Fc-silent antibody | Medium | CCL24中和に限定し、Fc effectorを避ける。 | 免疫複合体やFc依存作用を低減。 | 安全性面の保守設計。 | 中和だけでは不十分な可能性。 | Fc silence、半減期。 | FcγR/C1q binding、chemotaxis blockade。 | Fc-silent化でPK/中和能が劣る。 |
| Fc-enhanced antibody | Low | CCL24発現/結合細胞へのFc effectorを狙う。 | 分泌標的では意義が薄い。 | なし。 | 免疫複合体、オフターゲット炎症。 | 標的が分泌型のため設計合理性が弱い。 | Immune complex/Fc activation assay。 | Fc依存炎症シグナル。 |
| Bispecific antibody | Medium | CCL24 x CCL11/CCL26、またはCCL24 x fibrotic mediatorを同時中和。 | ケモカイン冗長性を超える可能性。 | CCL24単独より深いCCR3軸遮断。 | 広範な好酸球抑制、感染/組織修復リスク。 | CMC複雑化、用量比固定、粘度。 | Multi-chemokine chemotaxis、redundancy assay。 | 単独CCL24との差が小さい、または広範抑制リスク過大。 |
| ADC | Low | CCL24関連細胞へpayload送達。 | 分泌ケモカイン標的では不適。 | なし。 | ADC全身毒性、標的選択性なし。 | Internalization成立しない可能性。 | Not prioritized。 | 標的細胞選択性なし。 |
| Masked antibody | Medium-Low | 線維化/炎症組織でCCL24中和抗体を活性化。 | 全身chemokine blockadeを下げる可能性。 | 安全性差別化。 | 活性化不足、血中活性化、効果不足。 | Mask設計、分泌標的への局所活性化の難しさ。 | Disease tissue cleavage、local chemotaxis blockade。 | 局所活性化で通常抗体並みの中和が得られない。 |
| pH-dependent recycling antibody | High | 中性pHでCCL24を結合し、酸性エンドソームで解離して抗体再利用と抗原クリアランスを狙う。 | 高濃度分泌ケモカイン環境で投与量・持続性を改善できる可能性。 | CM-101型中和抗体との差別化としてPK/PD、投与利便性を狙える。 | 過度/長期のchemokine suppression、予測困難な抗原動態。 | pH依存性と中和potencyの両立、抗原sink modeling。 | pH binding、CCR3 chemotaxis blockade、antigen clearance PK model。 | 通常中和抗体よりPK/PD利点なし。 |

## Initial recommendation

主案は `blocking antibody`、副案は `pH-dependent recycling antibody`。最初のgo/no-goは、SSc/線維化疾患のヒト組織でCCL24が上がっており、中和で線維化・炎症readoutが動くかに置く。
