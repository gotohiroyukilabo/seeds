# Antibody Design Options: IL-36 receptor / IL1RL2

Target Card: `targets/target_cards/IL1RL2_IL36R.md`

## Design summary

推奨設計: `blocking antibody` または `Fc-silent blocking antibody`。IL-36Rは受容体阻害の臨床先例があり、HSなどIL-36-high皮膚疾患での患者選択が差別化の中心。

| Design | Initial fit | Mechanism of action | Expected benefit | Differentiation vs existing drugs | Safety risk | Developability risk | Initial assays | Kill criteria |
|---|---|---|---|---|---|---|---|---|
| Blocking antibody | High | IL-36RへのIL-36α/β/γシグナルを遮断。 | 上皮-好中球炎症を抑制。 | TNF/IL-17と異なる自然免疫/上皮炎症軸。 | 感染、皮膚バリア応答低下。 | Ligand複数種の完全遮断、受容体占有。 | IL-36刺激keratinocyte assay、HS lesion explant。 | IL-36-high患者組織で炎症抑制が出ない。 |
| Agonistic antibody | Low | IL-36Rを刺激する。 | 自己免疫/炎症疾患では不要。 | なし。 | 炎症悪化、発熱、皮膚炎増悪。 | アゴニズム制御困難。 | NF-kB/IL-8 induction assay。 | 炎症性サイトカイン誘導。 |
| Fc-silent antibody | High | IL-36R blockadeに限定し、Fc effectorを避ける。 | 慢性皮膚疾患で安全性を高める。 | Spesolimab-classとの差別化は、Fc設計より適応・患者選択が中心。 | 感染、効果不足。 | Fc silence、長期投与PK。 | FcγR/C1q陰性、keratinocyte blockade。 | Fc-silent化で効力/曝露が不足。 |
| Fc-enhanced antibody | Low | IL-36R発現細胞を除去。 | 病的上皮/免疫細胞除去の仮説。 | 既存阻害薬との差別化は弱く、安全性で劣る可能性。 | 正常上皮/免疫細胞傷害、皮膚バリア障害。 | 標的発現組織でのon-target toxicity。 | ADCC/ADCP、正常皮膚細胞毒性。 | 正常keratinocyte/immune cell killing。 |
| Bispecific antibody | Medium | IL-36R x IL-17/TNF/IL-1 pathwayなどの二重遮断。 | 複数炎症軸を同時制御し、HS非奏効例を狙う。 | 単独IL-36RやIL-17薬より深い炎症制御。 | 感染、過剰免疫抑制、皮膚防御低下。 | CMC複雑化、用量最適化困難。 | Dual cytokine blockade、HS explant multi-omics。 | 単剤併用相当の優位性がない、または感染リスクが過大。 |
| ADC | Low | IL-36R陽性細胞へpayload送達。 | 自己免疫では不適。 | なし。 | 上皮毒性、炎症悪化、全身毒性。 | ADC CMC、payload毒性。 | Internalization、normal skin toxicity。 | 正常皮膚毒性。 |
| Masked antibody | Medium | 炎症皮膚局所でIL-36R blockerを活性化。 | 全身曝露時の免疫抑制を低減する可能性。 | 慢性HSで安全性差別化。 | 活性化不十分、病変外活性化。 | Protease選択、mask安定性。 | HS lesion protease cleavage、masked potency shift。 | 病変選択的活性化が確認できない。 |
| pH-dependent recycling antibody | Medium | 受容体/リガンド結合後、酸性pHで解離して抗体再利用を改善。 | 投与間隔延長や高サイトカイン環境での抗原sink軽減。 | 用量・投与利便性で差別化。 | 長期 pathway blockade。 | pH依存性と受容体遮断potencyの両立。 | pH binding、receptor occupancy PK/PD。 | 通常IgG比でPK/PD利点なし。 |

## Initial recommendation

主案は `Fc-silent blocking antibody`。差別化は分子フォーマットよりも、IL-36 pathway-high HS/自己免疫皮膚サブセットの選択と、lesional explantでの薬効確認に置く。
