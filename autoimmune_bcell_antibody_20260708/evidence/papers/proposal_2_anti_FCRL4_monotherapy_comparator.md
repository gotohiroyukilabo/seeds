# Proposal 2 追加調査: 抗FCRL4単独抗体との比較

作成日: 2026-07-12

対象は `FCRL4 x CD22 組織B細胞サイレンサー` である。このメモでは、抗FCRL4抗体単独を単なる陰性対照ではなく、独立した候補/benchmarkとして扱う。

## 結論
抗FCRL4単独抗体は、必ず比較に入れるべきである。理由は、FCRL4が単なる住所ではなく、Sjögren唾液腺やRA滑膜などの病変組織B細胞stateを直接選べる標的だからである。

CD22 agonist活性が弱い場合でも、抗FCRL4単独で以下のいずれかが成立すれば、治療コンセプトとして残る。

| 成立ルート | 内容 |
|---|---|
| Fc-silent FCRL4 agonist | FCRL4そのものを刺激してBCR/TLR/Tfh反応を下げる。 |
| Fc-active/Fc-tuned anti-FCRL4 | FCRL4+病変B細胞だけをtrogocytosis、ADCP、限定的depletionでmodulateする。 |
| non-blocking anchor antibody | FCRL4+ state/niche B細胞へ結合し、内因性FCRL4/IgA調節を邪魔せず標的化する。 |
| IgA/J-chain axis modulation | FCRL4-IgA/J-chain相互作用が病態に関与する場合に遮断または調節する。 |

したがって、FCRL4 x CD22 BsAbは「抗FCRL4単独では足りない」ことを実験で示す必要がある。逆に、抗FCRL4単独が同等または上回るなら、BsAbより単純で開発しやすいシーズへpivotすべきである。

## 根拠文献
| 文献 | リンク | この比較での使いどころ |
|---|---|---|
| `Gene expression profiling of epithelium-associated FcRL4+ B cells in primary Sjögren's syndrome reveals a pathogenic signature.` Journal of Autoimmunity, 2020 | [PubMed](https://pubmed.ncbi.nlm.nih.gov/32201227/) / [DOI](https://doi.org/10.1016/j.jaut.2020.102439) | FCRL4+腺内B細胞が慢性活性化・炎症性signatureを持つ。抗FCRL4単独でstate B細胞を狙う根拠。 |
| `FcRL4+ B-cells in salivary glands of primary Sjögren's syndrome patients.` Journal of Autoimmunity, 2017 | [PubMed](https://pubmed.ncbi.nlm.nih.gov/28390747/) / [DOI](https://doi.org/10.1016/j.jaut.2017.03.012) | FCRL4+ B細胞が唾液腺病変とMALT lymphoma文脈にいる根拠。 |
| `Involvement of the HCK and FGR src-family kinases in FCRL4-mediated immune regulation.` Journal of Immunology, 2015 | [PubMed](https://pubmed.ncbi.nlm.nih.gov/25972488/) / [DOI](https://doi.org/10.4049/jimmunol.1401533) | FCRL4 signalingがHCK/FGR文脈で抑制にも活性化にも振れうることを示す。抗FCRL4 agonist設計の注意点。 |
| `Attenuation of HIV-associated human B cell exhaustion by siRNA downregulation of inhibitory receptors.` JCI, 2011 | [PubMed](https://pubmed.ncbi.nlm.nih.gov/21633172/) / [DOI](https://doi.org/10.1172/JCI45685) | FCRL4をinhibitory receptorとして読む根拠。FCRL4 knockdownでBCR応答性が増えるなら、FCRL4 agonismは抑制方向に働く可能性。 |
| `Cutting edge: human FcRL4 and FcRL5 are receptors for IgA and IgG.` Journal of Immunology, 2012 | [PubMed](https://pubmed.ncbi.nlm.nih.gov/22491254/) / [DOI](https://doi.org/10.4049/jimmunol.1102651) | FCRL4がIgA receptorであり、抗体で相互作用をblockingできる可能性。 |
| `FCRL4 Is an Fc Receptor for Systemic IgA, but Not Mucosal Secretory IgA.` Journal of Immunology, 2020 | [PubMed](https://pubmed.ncbi.nlm.nih.gov/32513851/) / [DOI](https://doi.org/10.4049/jimmunol.2000293) | primary FCRL4-bearing memory B cellsがIgAと結合し、AgR/BCR regulationに関わる可能性。 |
| `FcRL4 is an IgA receptor that primarily binds the joining chain.` PNAS, 2026 | [PubMed](https://pubmed.ncbi.nlm.nih.gov/42308047/) / [DOI](https://doi.org/10.1073/pnas.2600183123) | FCRL4-IgA/J-chain構造の最新根拠。IgA immune complex internalizationは期待しすぎない注意点。 |

## 抗FCRL4単独抗体のMoA案
| 設計 | 作用機序 | 期待利点 | 主要リスク | 初期評価 | Kill criteria |
|---|---|---|---|---|---|
| Fc-silent agonist anti-FCRL4 | FCRL4をcluster/agonizeし、BCR近位シグナルを抑える | CD22 agonism不要。最もシンプルな非除去型silencer | HCK/FGR文脈で活性化側に振れる可能性 | FCRL4 phosphorylation、SHP-1/SHP-2、pSyk、Ca flux、pERK、TLR7/9 | TLR/Ig産生/CD86/HLA-DR増強 |
| Fc-active/Fc-tuned anti-FCRL4 | FCRL4+ B細胞にADCP/trogocytosis/軽度depletionを誘導 | CD22 biologyに依存せず、state/niche B細胞を直接modulate | 正常粘膜FCRL4+ B細胞、局所炎症、過剰depletion | ADCP、trogocytosis、CD19/CD21/CD79b変化、正常粘膜B細胞影響 | FCRL4非依存作用、正常粘膜B細胞毒性 |
| non-blocking Fc-silent anti-FCRL4 | FCRL4+細胞を標識し、内因性IgA/J-chain regulationを邪魔しない | 安全なanchor/benchmark | 単独薬効が弱い | ligand competition、BCR/TLR readout | 結合以外の機能なし |
| blocking anti-FCRL4 | FCRL4-IgA/J-chain相互作用を遮断 | IgA immune complex病態なら有効かもしれない | FCRL4の内因性抑制を外して悪化する可能性 | IgA/J-chain binding blockade、BCR/TLR readout | BCR/TLR活性化、Ig産生増加 |
| anti-FCRL4 ADC | FCRL4+病変B細胞を除去 | 強力 | 慢性Sjögrenでは重い。FCRL4-IgA complex internalizationは期待薄 | 抗体自身のinternalization、payload感受性 | 正常粘膜B細胞毒性、internalization不足 |

## FCRL4 x CD22 BsAbとの比較仮説
| 結果 | 解釈 | 次の判断 |
|---|---|---|
| anti-FCRL4単独がBsAbと同等または上回る | CD22 armは不要。FCRL4 state/niche targetingだけで十分。 | 抗FCRL4単独を主案にpivot。BsAbは下げる。 |
| anti-FCRL4単独は効くがBsAbが明確に上回る | FCRL4 targetingにCD22 brakeが上乗せされる。 | BsAb継続。抗FCRL4単独はbenchmark。 |
| anti-FCRL4単独は弱いがFc-activeで効く | FCRL4 signalingよりFc依存modulationが主作用。 | Fc-tuned anti-FCRL4とFc-tuned BsAbを比較。 |
| anti-FCRL4単独で逆活性化 | FCRL4 agonismは危険。 | neutral anchor epitopeまたはBsAbのFCRL4 arm再設計。 |
| BsAbもanti-FCRL4単独も効かない | FCRL4はbystanderか、抗体で薬理化できない。 | No-Go。 |

## 最小比較セット
最初の実験では、以下を同一患者サンプル、同一濃度レンジ、同一readoutで比較する。

| 条件 | 目的 |
|---|---|
| vehicle/isotype | baseline |
| anti-FCRL4 Fc-silent agonist epitope | FCRL4 signalingだけで抑制できるか |
| anti-FCRL4 Fc-silent neutral/non-blocking epitope | 結合だけの効果、内因性ligand温存 |
| anti-FCRL4 Fc-active/Fc-tuned | state B cell modulation/depletionの可能性 |
| anti-CD22単独 | CD22 benchmark |
| anti-FCRL4 + anti-CD22 2剤併用 | BsAb geometryの必要性 |
| FCRL4 x CD22 Fc-silent BsAb | dual brake仮説 |
| FCRL4 x CD22 Fc-active/Fc-tuned BsAb | FCRL4-gated trogocytosis仮説 |

## Readout
| 分類 | 測定項目 |
|---|---|
| BCR近位 | pSyk、pBLNK、pPLCγ2、Ca flux、pERK、pAKT |
| FCRL4 signaling | FCRL4 phosphorylation、SHP-1/SHP-2、HCK/FGR依存性 |
| TLR/Tfh反応 | CpG/TLR9、R848/TLR7、CD40L、IL-21、NF-κB、CD86、HLA-DR |
| B細胞機能 | IgG/IgA/RF、自己抗体関連Ig、抗原提示、T cell activation |
| Fc依存作用 | ADCP、trogocytosis、CD19/CD21/CD79b変化、FcγR依存性 |
| 安全域 | 正常血中B細胞、扁桃/粘膜B細胞、FCRL4陰性B細胞への作用 |

## 提案への反映
プレゼンでは次のように言うのがよい。

```text
CD22 agonismに賭け切らない。
FCRL4+ disease-state B cellそのものを標的化できるなら、抗FCRL4単独でも成立する。
だから最初から抗FCRL4単独をhead-to-headで置き、BsAbはそれを超えた時だけ主案に残す。
```

この整理にすると、proposal 2はCD22依存の脆い仮説ではなく、`FCRL4+ disease-state B cell targeting platform` になる。
