# Antibody Design Options: OSM receptor / OSMR

Target Card: `targets/target_cards/OSMR.md`

## Design summary

推奨設計: `Fc-silent blocking antibody`。OSMRは慢性炎症・線維化・組織リモデリングを狙う仮説標的であり、標的細胞除去よりもシグナル遮断が適切。

| Design | Initial fit | Mechanism of action | Expected benefit | Differentiation vs existing drugs | Safety risk | Developability risk | Initial assays | Kill criteria |
|---|---|---|---|---|---|---|---|---|
| Blocking antibody | High | OSMRを介するOSM-family signalingを阻害。 | 慢性炎症、痒み、線維化/リモデリングを抑える可能性。 | TNF/IL-17/IL-4Rと異なるstromal remodeling軸。 | 創傷治癒、上皮修復、感染防御への影響。 | 受容体複合体、ligand選択性、疾患組織到達性。 | OSM刺激fibroblast/keratinocyte assay、HS/SSc tissue explant。 | ヒト病変組織でOSMR依存性が示せない。 |
| Agonistic antibody | Low | OSMRを刺激する。 | 自己免疫では通常不適。 | なし。 | 炎症・線維化・痒み悪化。 | アゴニズム制御困難。 | STAT3/NF-kB activation assay。 | 炎症/線維化マーカー誘導。 |
| Fc-silent antibody | High | OSMRシグナル遮断に限定し、標的細胞傷害を避ける。 | 線維芽細胞/上皮細胞を殺さず機能調整できる。 | Vixarelimab-classとの差別化は適応、epitope、OSM/IL-31関連作用の範囲。 | 修復応答抑制、効果不足。 | Fc silence、受容体遮断potency。 | FcγR/C1q陰性、OSM-induced gene blockade。 | Fc-silentでも細胞機能毒性または効果不足。 |
| Fc-enhanced antibody | Low | OSMR発現細胞をADCC/ADCPで除去。 | 病的線維芽細胞除去の仮説。 | 線維芽細胞標的治療として差別化仮説はある。 | 正常線維芽細胞/上皮細胞傷害、創傷治癒障害。 | 標的発現の広さ、on-target tissue toxicity。 | ADCC vs normal fibroblasts/keratinocytes。 | 正常組織細胞傷害が出る。 |
| Bispecific antibody | Medium | OSMR x IL-13/IL-31/IL-17/TGF-beta activationなどを同時制御。 | 痒み+リモデリング、炎症+線維化を同時に狙える。 | 単一サイトカイン阻害では残る慢性病変に差別化。 | 免疫抑制、創傷治癒障害、予期せぬpathway interaction。 | CMC、標的組み合わせの妥当性、用量最適化。 | Dual pathway tissue explant、fibroblast/keratinocyte co-culture。 | 単剤併用や単独OSMRより優位性なし。 |
| ADC | Low | OSMR発現細胞へpayload送達。 | 病的線維芽細胞除去の仮説のみ。 | 自己免疫では毒性が強すぎる可能性。 | 正常組織毒性、創傷治癒障害、payload毒性。 | Internalization不足、payload選択。 | Internalization、normal tissue cytotoxicity。 | 正常線維芽細胞/上皮細胞毒性。 |
| Masked antibody | Medium | 炎症/線維化組織でOSMR blockerを活性化。 | 正常組織修復への影響を低減。 | chronic remodeling標的の安全性差別化。 | 活性化部位の不確実性、効果不足。 | Mask cleavage、組織プロテアーゼ依存。 | SSc/HS tissue protease cleavage、masked potency。 | 疾患組織選択性がない。 |
| pH-dependent recycling antibody | Medium | pH依存結合により抗体再利用や受容体占有を調整。 | 慢性投与で投与間隔改善の可能性。 | 投与利便性で競合差別化。 | 長期OSMR blockade。 | pH設計、受容体internalization挙動。 | pH binding、receptor occupancy、PK/PD model。 | 通常IgGより曝露/効果の利点なし。 |

## Initial recommendation

主案は `Fc-silent blocking antibody`。最初の実験では、OSM/OSMR-highのヒト疾患組織で、炎症・線維化・痒み関連転写プログラムを抑えられるかを確認する。
