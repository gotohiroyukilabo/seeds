# 抗体設計案: CD38 x BCMA

## 設計仮説
plain oncology薬の転用ではなく、gated/finite自己免疫用resetでなければならない。

| 設計 | 作用機序 | 期待利点 | 差別化 | 安全性リスク | 初期評価系 | 中止基準 | 優先度 |
|---|---|---|---|---|---|---|---|
| blocking抗体 | CD38 enzyme/BCMA survivalを阻害 | 弱いが安全寄り | depletionより弱い | 効果不足 | survival assay | 自己抗体低下なし | 低-中 |
| agonist抗体 | 不適切 | なし | なし | 形質細胞生存促進 | 実施しない | survival増強 | 低 |
| Fc-silent抗体 | effectorなしbinding/blocking | 安全性probe | 単独では弱い | 効力不足 | autoantibody assay | depletion必須 | 低-中 |
| Fc強化抗体 | ADCC/ADCPでPC depletion | 深い自己抗体低下 | CD20より直接的 | 低Ig/感染 | ADCC/ADCP | 防御抗体喪失 | 中 |
| BsAb | CD38 x BCMA dual-gated/TCE | co-expressionで安全域仮説 | gatingなら新規 | CRS/ICANS | co-expression/cytokine | TIなし | 中-高 |
| ADC | CD38/BCMA payload | 有限reset | T細胞を避ける | marrow/payload毒性 | internalization | payload毒性 | 中-低 |
| masked抗体 | 病変/骨髄ニッチで活性化 | 全身毒性低減 | 安全域拡張 | 不活性/過活性 | protease panel | mask marginなし | 中-高 |
| pH依存recycling抗体 | soluble BCMA/sink対策 | 曝露改善 | 補助的 | 長期depletion | sink model | PK/PD利点なし | 中 |

## 推奨する初期方針
最初は標的biologyを検証できる最小フォーマットと、差別化を作る本命フォーマットを並行して評価する。流行技術を足すのではなく、単独抗体や2剤併用を超える空間薬理が出るかを最初に確認する。
