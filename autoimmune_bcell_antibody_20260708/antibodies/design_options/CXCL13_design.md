# 抗体設計案: CXCL13

## 設計仮説
可溶性B細胞ニッチ標的であり、pH-dependent recyclingが最も理にかなう。

| 設計 | 作用機序 | 期待利点 | 差別化 | 安全性リスク | 初期評価系 | 中止基準 | 優先度 |
|---|---|---|---|---|---|---|---|
| blocking抗体 | CXCL13-CXCR5を中和 | B細胞/Tfh migration阻害 | niche blockade | リンパ組織/感染 | chemotaxis/explant | migration抑制なし | 高 |
| agonist抗体 | 該当しない | なし | なし | chemokine刺激 | 実施しない | agonismが出る | 低 |
| Fc-silent抗体 | Fc炎症なしで中和 | 安全性 | 補助的 | 免疫複合体 | FcR/complement | PK悪化 | 中 |
| Fc強化抗体 | 該当しない | なし | なし | 免疫複合体 | 実施しない | 炎症活性化 | 低 |
| BsAb | CXCL13 + 冗長経路/albumin | 冗長性対策/半減期 | 必要時のみ | 広い免疫抑制 | combo explant | 単剤超えず | 中-低 |
| ADC | 該当しない | なし | なし | payload毒性 | 実施しない | 選択的uptakeなし | 低 |
| masked抗体 | 病変で活性化 | 全身リンパ影響低減 | 条件付き有用 | 不十分な活性 | protease panel | 選択性なし | 中 |
| pH依存recycling抗体 | 中性で結合、endosomeで解離 | 抗原clearance/投与量改善 | 最重要工学 | 過剰抑制 | pH affinity、PK/PD | 通常IgG超えず | 高 |

## 推奨する初期方針
最初は標的biologyを検証できる最小フォーマットと、差別化を作る本命フォーマットを並行して評価する。流行技術を足すのではなく、単独抗体や2剤併用を超える空間薬理が出るかを最初に確認する。
