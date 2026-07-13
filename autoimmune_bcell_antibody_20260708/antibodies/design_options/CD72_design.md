# 抗体設計案: CD72

## 設計仮説
真のagonismを証明し、B細胞活性化を起こさないことが最重要。

| 設計 | 作用機序 | 期待利点 | 差別化 | 安全性リスク | 初期評価系 | 中止基準 | 優先度 |
|---|---|---|---|---|---|---|---|
| blocking抗体 | ligand/相互作用を阻害 | 弱い | 目的と逆になりうる | 自己免疫悪化 | ligand assay | 活性化増強 | 低 |
| agonist抗体 | CD72 clusterで抑制シグナル | 非除去型tolerance | 中核革新 | 逆活性化/過抑制 | SHP-1、BCR/TLR | 抑制なし | 高 |
| Fc-silent抗体 | FcR架橋を避ける | 安全な機序確認 | 慢性向き | 必要な架橋を失う | Fc有無比較 | Fc依存でしか効かない | 高 |
| Fc強化抗体 | CD72+ B細胞depletion | 強いが凡庸 | CD20と差別化困難 | 感染/低Ig | ADCC | 広範depletion | 低 |
| BsAb | CD72 x IGHV4-34/FCRL4など | context-gated agonism | 強い新規性 | bridging/活性化 | cis/trans assay | monoを超えない | 中-高 |
| ADC | CD72+ B細胞殺傷 | 非推奨 | 意義が消える | payload/B細胞毒性 | internalization | 正常B細胞毒性 | 低 |
| masked抗体 | 病変でagonist化 | 全身抑制低減 | 条件付き | 活性不足 | masked agonism | 選択性なし | 中 |
| pH依存recycling抗体 | receptor sink対策 | 補助的 | 中核でない | occupancy変化 | recycling assay | sinkなし | 低-中 |

## 推奨する初期方針
最初は標的biologyを検証できる最小フォーマットと、差別化を作る本命フォーマットを並行して評価する。流行技術を足すのではなく、単独抗体や2剤併用を超える空間薬理が出るかを最初に確認する。
