# 抗体設計案: FCRL4 x CD22

## 設計仮説
anti-CD22の焼き直しではなく、FCRL4陽性組織B細胞上でCD22 brakeを入れる設計である。追加仮説として、FCRL4自体もBCR抑制性の免疫調節分子として働く可能性があるため、FCRL4 armを単なる住所ではなく第二のbrakeとして設計する余地がある。

| 設計 | 作用機序 | 期待利点 | 差別化 | 安全性リスク | 初期評価系 | 中止基準 | 優先度 |
|---|---|---|---|---|---|---|---|
| blocking抗体 | FCRL4機能/ligandを阻害 | 単純 | ligand不明では弱い。endogenous inhibitory ligandを遮断すると逆効果 | 粘膜記憶B細胞影響 | ligand assay、BCR/TLR readout | 機能不明または逆活性化 | 低 |
| agonist抗体 | CD22またはFCRL4を刺激して抑制 | 非除去型制御 | true inhibitionなら有用 | FCRL4刺激でTLR7/9、CD40、IL-21反応が増える可能性 | SHP-1/SHP-2、pSyk、Ca抑制、TLR readout | 抑制なし、またはTLR/Ig産生増強 | 中 |
| Fc-silent抗体 | Fc effectorなしでFCRL4/CD22 co-ligation | 殺さず沈静化し、CD22/SHP-1とFCRL4側抑制をきれいに検証 | 中核設計 | 効力不足 | FcR binding、B細胞抑制、SHP recruitment | Fc effectorなしで機能せず、他形式へのpivotも不可 | 高 |
| Fc-active/Fc-tuned抗体 | FCRL4+細胞でFcγR依存trogocytosisまたは軽度effector機能を誘導 | epratuzumab様作用をFCRL4陽性病変B細胞に限定できる可能性 | Fc-silent不十分時の重要分岐 | 非選択的trogocytosis、局所炎症、粘膜免疫低下 | CD22/CD19/CD21/CD79b低下、FcγR依存性、正常B細胞影響 | FCRL4非依存に広く表面分子strippingが起きる | 中-高 |
| Fc強化抗体 | FCRL4+細胞depletion | 病的組織B細胞除去 | CD20より選択的なら有用 | 粘膜免疫低下 | ADCC/ADCP | 安全域なし | 中 |
| BsAb | FCRL4住所 + CD22 brake。理想はFCRL4 brakeも同時に入れるdual inhibitory co-agonism | 疾患state選択的silencing | 中核革新 | off-cell bridging、FCRL4側逆活性化 | cis/trans binding、pSyk/pBLNK/pPLCγ2/Ca、TLR readout | anti-CD22単独または2剤併用を超えない | 高 |
| ADC | FCRL4+細胞へpayload | 強力除去 | 慢性Sjögrenでは重い | payload毒性 | internalization | 正常粘膜B細胞毒性 | 低-中 |
| masked抗体 | 腺炎症で活性化 | 全身影響低減 | proteaseがあれば有用 | 不活性/全身活性 | 唾液腺protease | 選択的unmaskなし | 中 |
| pH依存recycling抗体 | shed antigen対策 | 曝露改善 | 補助的 | 分布変化 | shed antigen assay | sinkなし | 低 |

## 推奨する初期方針
最初は抗FCRL4単独、Fc-silent BsAb、Fc-active/Fc-tuned BsAbを並行比較する。抗FCRL4単独は陰性対照ではなく、FCRL4+ disease-state B cellを直接標的化する独立候補である。Fc-silent BsAbはCD22 brake仮説とFCRL4 brake仮説をきれいに検証するため、Fc-active/Fc-tunedはepratuzumab様trogocytosisがFCRL4 gateで病変B細胞に限定できるかを見るために必要である。

## FCRL4 armの設計分岐
| FCRL4 arm | 狙い | 期待利点 | 主要リスク | 初期評価系 | Kill criteria |
|---|---|---|---|---|---|
| agonist epitope | FCRL4側のBCR抑制を積極的に入れる | CD22単独より強いdual brake | TLR7/9やTfh help反応の増強 | FCRL4 phosphorylation、SHP-1/SHP-2 recruitment、pSyk/Ca、CpG/R848/CD40/IL-21 readout | TLR/Ig産生/CD86/HLA-DR増強 |
| neutral anchor epitope | FCRL4を住所として使い、CD22薬理を主に見る | 安全にFCRL4+細胞選択性を出す | 新規性がCD22 retargetingに寄る | FCRL4 binding、internalization、CD22/SHP-1、BCR抑制 | anti-CD22単独を超えない |
| non-blocking epitope | endogenous FCRL4 ligandを邪魔しない | 自然な抑制入力を温存 | ligand不明で評価が難しい | ligand competition、不明なら複数epitope比較 | blockingで逆活性化、epitope差なし |
| internalizing epitope | FCRL4+細胞除去/ADCの可能性を見る | 強力 | 慢性Sjögrenでは重い | internalization、payload感受性、正常粘膜B細胞影響 | 正常粘膜B細胞毒性 |

## 抗FCRL4単独設計
| 設計 | 作用機序 | 期待利点 | BsAbとの比較 | 安全性リスク | 初期評価系 | Kill criteria |
|---|---|---|---|---|---|---|
| Fc-silent agonist anti-FCRL4 | FCRL4 signalingでBCR/TLR/Tfh反応を抑える | CD22 agonism不要。最も単純 | BsAbと同等なら単独へpivot | HCK/FGR文脈で逆活性化 | FCRL4 phosphorylation、SHP-1/SHP-2、pSyk、Ca、TLR7/9 | TLR/Ig産生/CD86/HLA-DR増強 |
| Fc-active/Fc-tuned anti-FCRL4 | FCRL4+病変B細胞にADCP/trogocytosis/軽度depletion | state/niche B細胞を直接modulate | Fc-active BsAbより安全/有効なら単独へpivot | 正常粘膜B細胞、局所炎症 | ADCP、trogocytosis、CD19/CD21/CD79b、FcγR依存性 | FCRL4非依存作用、正常粘膜B細胞毒性 |
| non-blocking Fc-silent anti-FCRL4 | FCRL4+細胞に結合し、内因性IgA/J-chain調節を邪魔しない | 安全なanchor benchmark | BsAbがこれを超えるか確認 | 単独薬効が弱い | ligand competition、BCR/TLR readout | 結合以外の機能なし |
| blocking anti-FCRL4 | FCRL4-IgA/J-chain相互作用を遮断 | IgA immune complex病態なら有効かもしれない | 原則低優先 | 内因性抑制解除 | IgA/J-chain binding、BCR/TLR readout | BCR/TLR活性化、Ig産生増加 |

## CD22 x FCRL4共刺激の判断
共刺激という言葉は誤解を招きやすい。本提案で狙うのは活性化costimulationではなく、CD22とFCRL4の共抑制刺激である。成功の形は、同じFCRL4+CD22+ B細胞上でBsAbがcisに結合し、BCR近位シグナルを単剤/2剤併用より強く落とすことである。

| 結果 | 判断 |
|---|---|
| BsAbがanti-CD22単独、anti-FCRL4単独、2剤併用を上回る | Go。BsAb geometryの必然性あり。 |
| anti-FCRL4単独がBsAbと同等または上回る | BsAbより単純な抗FCRL4単独へpivot。 |
| BsAbがanti-CD22単独のみ上回るが2剤併用と同等 | geometry再設計。新規性は弱まる。 |
| FCRL4 agonist armでTLR7/9/CD40/IL-21反応が増える | agonist epitopeはNo-Go。neutral anchorへ変更。 |
| FCRL4陰性B細胞にも強く作用する | gate失敗。No-Goまたは親和性/valency調整。 |
| FCRL4側SHP recruitmentなし、CD22側のみ | CD22 retargetingとして継続可だが、dual brake主張は下げる。 |
