# Proposal 2 薬理・抗体設計 参考文献リンク集

作成日: 2026-07-08

対象は `FCRL4 x CD22 組織B細胞サイレンサー` である。このページは、提案2を薬理・抗体設計の観点から説明するための文献リンク集であり、臨床試験、臨床有効性、患者アウトカム中心の文献は含めない。

## 範囲
含めるもの:

- FCRL4/FcRH4陽性組織B細胞のbiology
- FCRL4/FcRH4陽性組織B細胞のBCR抑制仮説
- 抗FCRL4単独抗体とのhead-to-head比較
- Sjögren腺外症状とFcRL4他疾患展開
- FcRL4/FCRL5競合ランドスケープのうち、抗体薬理・標的化形式に関係する情報
- FcRL4をT cell engagerへ展開する場合のCD3/CD8-biased設計と自己免疫TCE競合
- CD22/Siglec-2のBCR抑制薬理
- epratuzumabの抗体薬理とFc依存性trogocytosis
- Fc-silent/Fc-tuned抗体設計
- BsAbによるco-ligation/空間薬理
- ADCを検討する時のCD22 internalization/標的設計背景

含めないもの:

- epratuzumabのSLE Phase II/III臨床試験
- rituximab、BAFF阻害、CD40L阻害、FcRn阻害などの臨床成績比較
- FcRL4/FCRL5競合の網羅的な事業・特許調査
- inotuzumabなどCD22薬剤の臨床有効性論文
- Sjögren病の臨床endpointや治験デザイン中心の論文

## 競合ランドスケープ
詳細メモ: [FCRL4_competitor_landscape.md](../competitive_landscape/FCRL4_competitor_landscape.md)

| 論点 | 薬理・抗体設計上の意味 |
|---|---|
| FcRL4直撃の公開臨床競合は確認できない | 新規性は高いが、外部clinical validationはない。fresh tissue薬理が必須。 |
| IRTA1/FcRL4は病理マーカーとして先行 | IHC/RNAscope/flowによる患者選択の足場になる。治療用epitopeは別に作る。 |
| FCRL5 x CD3のcevostamabがSLE/LNへ進出 | FCRL family標的の自己免疫応用が現実化。Proposal 2はT-cell engagerではなくtissue silencerとして差別化する。 |
| FCRL5 CAR-TもMMで動く | FCRL family標的が複数モダリティへ広がる兆候。FcRL4 ADC/CAR-Tは慢性自己免疫では低優先。 |

## T cell engager方向性
詳細メモ: [FCRL4_TCE_design.md](../../antibodies/design_options/FCRL4_TCE_design.md)

| 論点 | 薬理・抗体設計上の意味 |
|---|---|
| CD8A-only BsAb | CD8Aはco-receptorであり、単独ではT細胞主活性化signalとして弱い。低優先。 |
| FcRL4 x low-affinity CD3 | TCE方向性の主案。FcRL4+病変B細胞を短期resetする。 |
| FcRL4 2+1 x low-affinity CD3 | FcRL4高発現細胞でavidityを作り、標的密度gateを狙う。 |
| masked/prodrug TCE | 全身T細胞活性化を下げる可能性。ただしSjögren組織でmask解除条件が必要。 |
| 自己免疫TCE競合 | CD19 x CD3、CD20 x CD3、BCMA x CD3、FcRH5 x CD3が自己免疫へ入り始めており、FcRL4 tissue-state選択性が必須。 |

## まず読むべき文献
| 優先 | 文献 | リンク | 提案2での使いどころ |
|---:|---|---|---|
| 1 | Haacke et al. `FcRL4+ B-cells in salivary glands of primary Sjögren's syndrome patients.` Journal of Autoimmunity, 2017 | [PubMed](https://pubmed.ncbi.nlm.nih.gov/28390747/) / [DOI](https://doi.org/10.1016/j.jaut.2017.03.012) | FCRL4をSjögren唾液腺B細胞の「住所」として使う中核根拠。 |
| 2 | Ehrhardt et al. `Expression of the immunoregulatory molecule FcRH4 defines a distinctive tissue-based population of memory B cells.` J Exp Med, 2005 | [PubMed](https://pubmed.ncbi.nlm.nih.gov/16157685/) / [DOI](https://doi.org/10.1084/jem.20050879) | FCRL4/FcRH4が組織局在性・機能的に独特な記憶B細胞を示す基礎根拠。FCRL4を住所だけでなく免疫調節分子として読む入口。 |
| 3 | Müller et al. `CD22: A Regulator of Innate and Adaptive B Cell Responses and Autoimmunity.` Frontiers in Immunology, 2018 | [PubMed](https://pubmed.ncbi.nlm.nih.gov/30323814/) / [DOI](https://doi.org/10.3389/fimmu.2018.02235) | CD22をB細胞brakeとして使う薬理の基礎。 |
| 4 | Rossi et al. `Trogocytosis of multiple B-cell surface markers by CD22 targeting with epratuzumab.` Blood, 2013 | [PubMed](https://pubmed.ncbi.nlm.nih.gov/23821660/) / [DOI](https://doi.org/10.1182/blood-2012-12-473744) | epratuzumab作用が単純なCD22 blockingではなく、Fc依存性trogocytosisを含みうる根拠。 |
| 5 | Beum et al. `Fcγ-receptor-mediated trogocytosis impacts mAb-based therapies.` Blood, 2015 | [PubMed](https://pubmed.ncbi.nlm.nih.gov/25498911/) / [DOI](https://doi.org/10.1182/blood-2014-10-569244) | Fc-active/Fc-tuned案を評価に入れる理由を説明する抗体薬理レビュー。 |
| 6 | Szili et al. `Suppression of innate and adaptive B cell activation pathways by antibody coengagement of FcγRIIb and CD19.` mAbs, 2014 | [PubMed](https://pubmed.ncbi.nlm.nih.gov/24828435/) / [DOI](https://doi.org/10.4161/mabs.28841) | 抑制受容体を抗体co-engagementでB細胞に入れる設計の先行薬理。FCRL4 x CD22 BsAbの論理に近い。 |
| 7 | Labrijn et al. `Bispecific antibodies: a mechanistic review of the pipeline.` Nature Reviews Drug Discovery, 2019 | [PubMed](https://pubmed.ncbi.nlm.nih.gov/31175342/) / [DOI](https://doi.org/10.1038/s41573-019-0028-1) | BsAbを単なる2標的抗体ではなく、空間薬理ツールとして説明する時の総説。 |
| 8 | Schlothauer et al. `Novel human IgG1 and IgG4 Fc-engineered antibodies with completely abolished immune effector functions.` PEDS, 2016 | [PubMed](https://pubmed.ncbi.nlm.nih.gov/27578889/) / [DOI](https://doi.org/10.1093/protein/gzw040) | Fc-silent主案の実装候補を考える時の基礎文献。 |
| 9 | Saunders et al. `Profiling the Biophysical Developability Properties of Common IgG1 Fc Effector Silencing Variants.` Antibodies, 2023 | [PubMed](https://pubmed.ncbi.nlm.nih.gov/37753968/) / [DOI](https://doi.org/10.3390/antib12030054) | Fc-silent variantのdevelopability比較に使う。 |
| 10 | `Mapping the B-cell axis in Sjögren's disease: repertoire, microenvironment, and potential routes to precision treatment.` Current Opinion in Immunology, 2026 | [PubMed](https://pubmed.ncbi.nlm.nih.gov/41435726/) / [DOI](https://doi.org/10.1016/j.coi.2025.102712) | SjögrenをB細胞軸・組織微小環境・precision treatmentとして語る最新の背景レビュー。 |

## FCRL4と組織B細胞
| 文献 | リンク | 読むポイント |
|---|---|---|
| Haacke et al. `FcRL4+ B-cells in salivary glands of primary Sjögren's syndrome patients.` Journal of Autoimmunity, 2017 | [PubMed](https://pubmed.ncbi.nlm.nih.gov/28390747/) / [DOI](https://doi.org/10.1016/j.jaut.2017.03.012) | FCRL4陽性B細胞がSjögren唾液腺病変で報告される。提案2では「FCRL4高発現が全例で確立」ではなく「病変組織B細胞stateの候補」として扱う。 |
| Ehrhardt et al. `Expression of the immunoregulatory molecule FcRH4 defines a distinctive tissue-based population of memory B cells.` J Exp Med, 2005 | [PubMed](https://pubmed.ncbi.nlm.nih.gov/16157685/) / [DOI](https://doi.org/10.1084/jem.20050879) | FcRH4/FCRL4陽性記憶B細胞の組織局在、表現型、BCR応答性の特徴。 |
| `Antibodies Encoded by FCRL4-Bearing Memory B Cells Preferentially Recognize Commensal Microbial Antigens.` Journal of Immunology, 2018 | [PubMed](https://pubmed.ncbi.nlm.nih.gov/29703863/) / [DOI](https://doi.org/10.4049/jimmunol.1701549) | FCRL4-bearing memory B cellが粘膜・常在抗原文脈に寄る可能性。安全性では正常粘膜B細胞への影響を見る必要がある。 |
| `Mapping the B-cell axis in Sjögren's disease.` Current Opinion in Immunology, 2026 | [PubMed](https://pubmed.ncbi.nlm.nih.gov/41435726/) / [DOI](https://doi.org/10.1016/j.coi.2025.102712) | 最新レビューとして、B細胞repertoire、組織微小環境、精密医療の流れを確認する。 |
| `Gene expression profiling of epithelium-associated FcRL4+ B cells in primary Sjögren's syndrome reveals a pathogenic signature.` Journal of Autoimmunity, 2020 | [PubMed](https://pubmed.ncbi.nlm.nih.gov/32201227/) / [DOI](https://doi.org/10.1016/j.jaut.2020.102439) | 腺内FcRL4+ B細胞が慢性活性化・炎症性signatureを持つ根拠。 |

## FCRL4のBCR抑制とCD22共刺激
詳細メモ: [proposal_2_FCRL4_BCR_suppression.md](proposal_2_FCRL4_BCR_suppression.md)

抗FCRL4単独比較メモ: [proposal_2_anti_FCRL4_monotherapy_comparator.md](proposal_2_anti_FCRL4_monotherapy_comparator.md)

| 論点 | 読む文献 | 提案2での使いどころ |
|---|---|---|
| FCRL4は住所だけではない | Ehrhardt et al., 2005 | FCRL4を組織B細胞markerかつ免疫調節分子として扱う。 |
| FCRL4陽性細胞は粘膜/組織記憶B細胞文脈を持つ | FCRL4-bearing memory B cell, 2018 | FCRL4刺激で正常粘膜B細胞や常在抗原応答に影響するリスクを説明する。 |
| FCRL4陽性細胞がSjögren唾液腺にいる | Haacke et al., 2017 | FCRL4をgland B-cell-high Sjögrenの患者選択/組織住所として使う。 |
| CD22とFCRL4のdual brake | CD22 review + FCRL4 tissue B cell文献 | FCRL4 x CD22 BsAbを「住所付きCD22抗体」ではなくdual inhibitory co-agonistとして説明する。 |
| 未確定点 | fresh gland B cell assay | 抗FCRL4抗体でBCR抑制が再現するか、TLR7/9/CD40/IL-21反応が増えないかを最初に確認する。 |

## 抗FCRL4単独抗体
| 論点 | 文献 | 提案2での使いどころ |
|---|---|---|
| FCRL4 signalingはHCK/FGR文脈で変わる | FCRL4-mediated immune regulation via HCK/FGR, 2015 | 抗FCRL4 agonistは抑制にも逆活性化にも振れうる。 |
| FCRL4 downregulationでBCR応答性が増える | JCI tissue-like memory B cell exhaustion, 2011 | FCRL4をinhibitory receptorとして読む根拠。 |
| FCRL4はIgA receptor | FcRL4/FcRL5 Ig receptor, 2012 | blocking/non-blocking epitope設計に必要。 |
| FCRL4はsystemic IgA/J-chainと関係する | FCRL4 systemic IgA, 2020; FcRL4 J-chain structure, 2026 | IgA/J-chain/FCRL4軸を邪魔するか温存するかの判断。 |
| 抗FCRL4単独が効く可能性 | pSS FcRL4+ pathogenic signature, 2020 | CD22 agonismなしでもFCRL4+ disease-state B cell targetingで成立しうる。 |

## 腺外症状と他疾患展開
詳細メモ: [proposal_2_FCRL4_extraglandular_and_indication_expansion.md](proposal_2_FCRL4_extraglandular_and_indication_expansion.md)

| 論点 | 文献 | 提案2での使いどころ |
|---|---|---|
| Sjögren腺外症状はB-cell-high axisで層別すべき | cryoglobulinemic vasculitis、CXCL13/BAFF/IL-21、Tfh-B cell文献 | 関節/神経/皮膚/腎/肺はprimaryではなく、B-cell-high secondary endpointにする。 |
| RAはFcRL4横展開の最有力 | RA FcRL4+ RANKL-producing B cells, 2015 | FcRL4+滑膜B細胞をSjögren以外の組織B細胞標的として扱う。 |
| RA FcRL4+ B細胞は自己抗原反応性を持ちうる | RA FcRL4+ B cells and citrullinated autoantigens, 2017 | RAでのFCRL4 x CD22/FCRL4 x FCGR2B仮説の根拠。 |
| FcRL4はIgA receptor | FCRL4 Is an Fc Receptor for Systemic IgA, 2020 | IgA/粘膜/免疫複合体疾患への外挿。ただし直接疾患証拠は必要。 |

## CD22/Siglec-2のB細胞抑制薬理
| 文献 | リンク | 読むポイント |
|---|---|---|
| Müller et al. `CD22: A Regulator of Innate and Adaptive B Cell Responses and Autoimmunity.` Frontiers in Immunology, 2018 | [PubMed](https://pubmed.ncbi.nlm.nih.gov/30323814/) / [DOI](https://doi.org/10.3389/fimmu.2018.02235) | CD22をBCR/TLR応答の抑制受容体として位置付ける。 |
| Walker and Smith. `CD22: an inhibitory enigma.` Immunology, 2008 | [PubMed](https://pubmed.ncbi.nlm.nih.gov/18067554/) / [DOI](https://doi.org/10.1111/j.1365-2567.2007.02752.x) | CD22のcis/trans ligand、BCR proximity、抑制/活性化の複雑さを理解する。 |
| Tsubata. `Molecular interactions regulate BCR signal inhibition by CD22 and CD72.` Trends in Immunology, 2004 | [PubMed](https://pubmed.ncbi.nlm.nih.gov/15364057/) / [DOI](https://doi.org/10.1016/j.it.2004.08.002) | CD22とCD72の比較。提案3のCD72とベンチマークする時にも使える。 |
| `CD22 as a Target for Hematological Malignancies and Autoimmune Diseases.` International Journal of Molecular Sciences, 2026 | [PubMed](https://pubmed.ncbi.nlm.nih.gov/42353124/) / [DOI](https://doi.org/10.3390/ijms27125406) | CD22標的モダリティの最新レビュー。臨床成績ではなく、標的特性とモダリティ選択の背景として読む。 |

## epratuzumabの抗体薬理とtrogocytosis
| 文献 | リンク | 読むポイント |
|---|---|---|
| Carnahan et al. `Epratuzumab, a humanized monoclonal antibody targeting CD22: characterization of in vitro properties.` Clinical Cancer Research, 2003 | [PubMed](https://pubmed.ncbi.nlm.nih.gov/14506197/) | epratuzumabの結合、internalization、B細胞作用のin vitro characterization。臨床有効性ではなく薬理の入口。 |
| Rossi et al. `Trogocytosis of multiple B-cell surface markers by CD22 targeting with epratuzumab.` Blood, 2013 | [PubMed](https://pubmed.ncbi.nlm.nih.gov/23821660/) / [DOI](https://doi.org/10.1182/blood-2012-12-473744) | CD22だけでなくCD19/CD21/CD79bも低下するという、Fc依存性trogocytosisの中心文献。 |
| Beum et al. `The shaving reaction: rituximab/CD20 complexes are removed from mantle cell lymphoma and chronic lymphocytic leukemia cells by THP-1 monocytes.` Journal of Immunology, 2006 | [PubMed](https://pubmed.ncbi.nlm.nih.gov/16456022/) / [DOI](https://doi.org/10.4049/jimmunol.176.4.2600) | 抗体結合標的がFcγR陽性細胞によって標的細胞表面から剥がされる現象の古典的基礎。 |
| Beum et al. `Loss of CD20 and bound CD20 antibody from opsonized B cells occurs more rapidly because of trogocytosis mediated by Fc receptor-expressing effector cells than direct internalization by the B cells.` Journal of Immunology, 2011 | [PubMed](https://pubmed.ncbi.nlm.nih.gov/21841127/) / [DOI](https://doi.org/10.4049/jimmunol.1101189) | internalizationとtrogocytosisを分けて考える時の参考。 |
| Beum et al. `Fcγ-receptor-mediated trogocytosis impacts mAb-based therapies.` Blood, 2015 | [PubMed](https://pubmed.ncbi.nlm.nih.gov/25498911/) / [DOI](https://doi.org/10.1182/blood-2014-10-569244) | Fc-active/Fc-tunedを評価枝に入れる根拠。Fc-silent主案が「trogocytosis否定」ではないことを説明しやすい。 |

## BsAbとco-ligation設計
| 文献 | リンク | 読むポイント |
|---|---|---|
| Szili et al. `Suppression of innate and adaptive B cell activation pathways by antibody coengagement of FcγRIIb and CD19.` mAbs, 2014 | [PubMed](https://pubmed.ncbi.nlm.nih.gov/24828435/) / [DOI](https://doi.org/10.4161/mabs.28841) | B細胞上で抑制受容体を共架橋して反応を落とす薬理。FCRL4 x CD22の先行概念に近い。 |
| Horton et al. `Antibody-mediated coengagement of FcγRIIb and B cell receptor complex suppresses humoral immunity in systemic lupus erythematosus.` Journal of Immunology, 2011 | [PubMed](https://pubmed.ncbi.nlm.nih.gov/21357255/) / [DOI](https://doi.org/10.4049/jimmunol.1003412) | FcγRIIb/BCR co-engagementの自己免疫文脈での薬理。 |
| Veri et al. `Inhibition of B cell receptor-mediated activation of primary human B cells by coengagement of CD19 and FcγRIIb with Fc-engineered antibodies.` Molecular Immunology, 2008 | [PubMed](https://pubmed.ncbi.nlm.nih.gov/18691763/) / [DOI](https://doi.org/10.1016/j.molimm.2008.06.027) | Fc-engineered antibodyで抑制受容体を使う設計思想。 |
| Labrijn et al. `Bispecific antibodies: a mechanistic review of the pipeline.` Nature Reviews Drug Discovery, 2019 | [PubMed](https://pubmed.ncbi.nlm.nih.gov/31175342/) / [DOI](https://doi.org/10.1038/s41573-019-0028-1) | BsAbのformat、valency、geometry、MoA分類を確認する総説。 |
| Li et al. `Membrane-Proximal Epitope Facilitates Efficient T Cell Synapse Formation by Anti-FcRH5/CD3 and Is a Requirement for Myeloma Cell Killing.` Cancer Cell, 2017 | [PubMed](https://pubmed.ncbi.nlm.nih.gov/28262555/) / [DOI](https://doi.org/10.1016/j.ccell.2017.02.001) | FCRL family標的をBsAbで使う時に、epitope距離と免疫シナプスgeometryが効くことを示す先行例。Proposal 2でもFCRL4 epitope/geometry screenが必須。 |

## Fc-silent/Fc-tuned抗体設計
| 文献 | リンク | 読むポイント |
|---|---|---|
| Schlothauer et al. `Novel human IgG1 and IgG4 Fc-engineered antibodies with completely abolished immune effector functions.` PEDS, 2016 | [PubMed](https://pubmed.ncbi.nlm.nih.gov/27578889/) / [DOI](https://doi.org/10.1093/protein/gzw040) | LALA-PGなどFc effector低減の実装を考える基礎。 |
| Oganesyan et al. `Effector-attenuating Substitutions That Maintain Antibody Stability and Reduce Toxicity in Mice.` JBC, 2017 | [PubMed](https://pubmed.ncbi.nlm.nih.gov/28077575/) / [DOI](https://doi.org/10.1074/jbc.M116.767749) | effectorを落としつつ安定性を保つFc variant設計。 |
| Saunders et al. `Profiling the Biophysical Developability Properties of Common IgG1 Fc Effector Silencing Variants.` Antibodies, 2023 | [PubMed](https://pubmed.ncbi.nlm.nih.gov/37753968/) / [DOI](https://doi.org/10.3390/antib12030054) | Fc-silent variantの物性・developability比較。BsAb化する前に読む。 |
| `pH-responsive antibodies for therapeutic applications.` Journal of Biomedical Science, 2021 | [PubMed](https://pubmed.ncbi.nlm.nih.gov/33482842/) / [DOI](https://doi.org/10.1186/s12929-021-00709-7) | pH-dependent recycling抗体の設計背景。提案2では低優先だが、可溶性sinkや組織滞留を考える時の補助。 |

## ADC/internalizationの参考
提案2ではADCは主案ではない。慢性Sjögren病で組織B細胞を殺しにいく設計は安全域が厳しいためである。ただし、CD22はinternalizing targetとして知られており、ADCをなぜ低優先にするかを説明する補助文献として以下を置く。

| 文献 | リンク | 読むポイント |
|---|---|---|
| `Targeting CD22 for the Treatment of B-Cell Malignancies.` ImmunoTargets and Therapy, 2021 | [PubMed](https://pubmed.ncbi.nlm.nih.gov/34262884/) / [DOI](https://doi.org/10.2147/ITT.S288546) | CD22標的モダリティ全体を確認する。臨床成績ではなく、CD22 internalizationとADC/免疫毒素の設計背景を拾う。 |
| `CD22 as a Target for Hematological Malignancies and Autoimmune Diseases.` International Journal of Molecular Sciences, 2026 | [PubMed](https://pubmed.ncbi.nlm.nih.gov/42353124/) / [DOI](https://doi.org/10.3390/ijms27125406) | 最新のCD22標的レビュー。自己免疫への読み替え可能性と限界を確認する。 |

## 提案2への読み替え
| 論点 | 文献で支えたいこと | プレゼンでの言い方 |
|---|---|---|
| FCRL4 gate | FCRL4/FcRH4陽性B細胞は組織局在性・Sjögren唾液腺病変との関連がある | 全B細胞を叩くのではなく、病変組織B細胞stateを選ぶ。 |
| FCRL4 brake | FCRL4自体もBCR応答を弱める免疫調節分子として使える可能性がある | FCRL4は住所であり、第二のブレーキ候補でもある。 |
| 抗FCRL4単独 | FCRL4+ disease-state B cellを直接標的化できる | CD22 agonismが弱くても、抗FCRL4単独で成立する可能性がある。BsAbは単独を超える必要。 |
| CD22 brake | CD22はBCR/TLR反応を制御する抑制受容体である | CD22は疾患住所ではなくブレーキである。FCRL4で住所と第二ブレーキを足す。 |
| 腺外症状 | FcRL4直接ではなく、B-cell-high systemic axisとの連動を見る | 関節/神経/皮膚/腎/肺はprimaryではなく層別secondary endpointにする。 |
| RA横展開 | RA滑膜FcRL4+ B細胞はRANKL/TNFや自己抗原反応性と関係する | FcRL4 x CD22を滑膜B細胞サイレンサーとして横展開できる可能性。 |
| epratuzumabからの学習 | epratuzumabはCD22単独薬理に加え、Fc依存性trogocytosisを含みうる | 失敗はCD22 biology全否定ではなく、患者選択・組織選択・geometry不足の可能性として読む。 |
| Fc-silent主案 | Fc作用を切ることで、FCRL4 x CD22 cis co-ligationそのものの薬理を検証できる | Fc-silentはtrogocytosis否定ではなく、機序をきれいに切る初期主案である。 |
| Fc-active/Fc-tuned枝 | FcγR依存性trogocytosisが必要なら、FCRL4 gateで病変B細胞に限定できるかを試す | Fc-activeはbackupではなく、初期から比較する重要な分岐である。 |
| BsAbの必然性 | co-engagementは単剤や2剤併用と異なる空間薬理を作れる | anti-FCRL4 + anti-CD22併用では同じ膜上でCD22/FCRL4 brakeを入れる保証がない。 |
| ADC低優先 | CD22 internalizationはADC向きだが、慢性自己免疫でpayload毒性と正常粘膜B細胞毒性が重い | ADCは技術的には可能でも、提案2の疾患目的とはズレやすい。 |

## 実験デザインに落とす時の対応
| 参考文献群 | 実験で確認すること |
|---|---|
| FCRL4/FcRH4組織B細胞 | fresh唾液腺でFCRL4+CD22+ B細胞の頻度、局在、clonality、CXCL13/Tfh近接、自己抗体/TLR応答を測る。 |
| FCRL4 BCR抑制 | anti-FCRL4単独とFCRL4 x CD22 BsAbで、FCRL4側SHP-1/SHP-2 recruitment、pSyk、pBLNK、pPLCγ2、Ca flux、pERKを測る。 |
| 抗FCRL4単独比較 | anti-FCRL4 Fc-silent agonist、neutral/non-blocking、Fc-active/Fc-tunedを分けて、BsAbと同一readoutで比較する。 |
| 腺外症状 | 唾液腺FcRL4+ B細胞量とESSDAI domain、CXCL13、RF、cryoglobulin、C4、高IgGを相関させる。 |
| RA横展開 | RA滑膜液/滑膜生検でFcRL4+CD22+ B細胞、RANKL、TNF、IgA、ACPA反応性、BsAb機能を測る。 |
| CD22薬理 | CD22 phosphorylation、SHP-1 recruitment、BCR誘導Ca flux、ERK/AKT、TLR9/R848応答、Ig産生を測る。 |
| epratuzumab/trogocytosis | CD22、CD19、CD21、CD79bの表面低下、FcγR陽性細胞依存性、internalizationとの分離を測る。 |
| BsAb/co-ligation | anti-CD22単独、anti-FCRL4単独、2剤併用、Fc-silent BsAb、Fc-active/Fc-tuned BsAbを同一系で比較する。 |
| FCRL5競合 | Cevostamab/FcRH5 x CD3とは異なり、FcRL4 x CD22がdepletionではなくsilencingで成立するかを示す。 |
| Fc-silent/Fc-tuned | FcγR binding、C1q binding、ADCC/ADCP、物性、凝集、発現量、熱安定性を比較する。 |
| ADC/internalization | FCRL4/CD22 internalization、正常粘膜B細胞への取り込み、payload感受性を確認する。ただし初期優先度は低い。 |
