# FcRL4 x CD8A BsAb案: CD8 T細胞リクルートによる病変B細胞reset

作成日: 2026-07-15

## 位置付け
このファイルは `FCRL4 x CD22` とは別案である。CD22案が病変B細胞を沈静化するsilencerであるのに対し、FcRL4 x CD8A案はFcRL4+病変B細胞をCD8+ T細胞へ提示し、限定的に除去/resetする攻めた設計である。

## 1文仮説
Sjögren腺内またはRA滑膜のFcRL4+ disease-state B細胞を、CD8+ T細胞に近接させて短期的に除去するFcRL4 x CD8A BsAbを検討する。ただし、CD8A単独はT細胞の主活性化受容体ではないため、純粋なCD8-only BsAbは低優先で、CD8-biased T-cell engagerまたはtrispecificへの発展余地として扱う。

## 標的情報
| 項目 | 内容 |
|---|---|
| B細胞側gate | FCRL4 / Fc receptor-like protein 4, UniProt Q96PJ5 |
| 相方 | CD8A / T-cell surface glycoprotein CD8 alpha chain, UniProt P01732 |
| 局在 | FCRL4、CD8Aとも膜タンパク質 |
| 想定format | Fc-silent IgG-like BsAb、またはCD8-biased TCEへの発展形 |
| 主目的 | FcRL4+病変B細胞の除去/reset |

## なぜCD8Aを考えるのか
CD8A/CD8Bは細胞傷害性T細胞の代表的な表面分子であり、CD8 co-receptorはTCR/MHC-I認識とLck近接に関わる。病変組織内にCD8+ T細胞が存在し、FcRL4+ B細胞がリンパ上皮病変、MALT lymphoma前段階、RA滑膜炎症ニッチにいるなら、CD8+ T細胞をFcRL4+ B細胞へ向ける発想は一見魅力的である。

しかし、CD8はCD3/TCR複合体そのものではない。CD8Aを結合するだけで、CD3 x tumor antigen型T-cell engagerのような抗原非依存の強いT細胞活性化と殺傷が起きるとは言いにくい。したがって、この案の核心は「CD8を使えば安全なTCEになる」ではなく、「CD8+ T細胞に偏らせた病変B細胞resetを作れるか」である。

## 現時点の外部根拠
| 論点 | 根拠 | 読み方 |
|---|---|---|
| FcRL4+ B細胞はSjögren唾液腺にいる | Haacke et al., 2017 | FcRL4は病変B細胞側のgateになりうる。 |
| FcRL4+ B細胞はpathogenic signatureを持つ | pSS FcRL4+ B cell RNA-seq, 2020 | 除去/reset対象としての妥当性を支える。 |
| CD8はco-receptorでありTCR signalingを補助する | CD8 co-receptor review, 2024 | CD8A単独engagementでは主活性化signalが不足する可能性が高い。 |
| 自己免疫でT-cell engagerによるB細胞resetの兆候がある | CD19 x CD3 blinatumomab in refractory RA, 2024 | TCEは自己免疫でも使える可能性があるが、これはCD3 TCEでありCD8-onlyではない。 |
| TCEはMGなど難治自己免疫にも探索され始めている | CD19 x CD3/BCMA x CD3 case reports, 2025 | 強いB cell/plasma cell resetは有効性の兆しがある一方、CRS/感染/低Igが問題になる。 |

## 競合状況
FcRL4 x CD8Aの公開臨床開発は確認できない。ClinicalTrials.govで `CD8 bispecific antibody`、`CD8A antibody`、`CD8 T cell engager` を検索しても、FcRL4 x CD8Aに該当する直接競合は見つからなかった。

ただし、競合はCD8AではなくT-cell engager全体で見るべきである。CD19 x CD3、BCMA x CD3、CD20 x CD3、FcRH5 x CD3のようなTCEがB細胞疾患・自己免疫へ広がっている。特にFcRH5 x CD3のcevostamabがSLE/LNへ進む予定であり、FcRL family x T cell engagerという隣接競合は強い。

## 作用機序案
| 設計 | 作用機序 | 評価 |
|---|---|---|
| FcRL4 x CD8A pure BsAb | FcRL4+ B細胞とCD8+ T細胞を近接させる | CD8A単独では活性化signal不足の可能性。低優先。 |
| FcRL4 x CD8A Fc-active | CD8近接 + FcγR細胞のADCP/trogocytosisを併用 | 薬理が混ざり、安全性説明が難しい。 |
| FcRL4 x low-affinity CD3, CD8-biased design | CD3活性化を弱め、CD8+ T細胞寄りの殺傷を狙う | CD8A pureより現実的。BsAbというよりTCE最適化案。 |
| FcRL4 x CD8A x CD3 trispecific | CD8+ T細胞選択とCD3 activationを両立 | 革新的だがCMC/安全性が重い。今回の3候補では発展形として扱う。 |

## 期待される利点
- FcRL4+病変B細胞を沈静化ではなく短期resetできる。
- FcRL4 gateが効けば、CD19/CD20/CD3 TCEより病変組織B細胞に寄せられる。
- Sjögren関連MALT lymphoma前段階、MALT lymphoma高リスク、RA滑膜FcRL4+炎症性B細胞など、より攻めた患者群では魅力がある。
- CD22やFCGR2Bなどの抑制受容体agonismが効かない場合のbackupになる。

## 既存薬との差別化
CD19 x CD3やCD20 x CD3は広くB細胞を狙う。FcRL4 x CD8Aは、FcRL4+組織B細胞stateをgateにする点が違う。ただし、CD8Aだけで殺傷活性が成立しない場合、結局はCD3 TCEへ寄ってしまい、差別化は弱くなる。

FcRH5 x CD3/cevostamabとの違いは、FCRL5+形質細胞/B lineage全体ではなく、FcRL4+粘膜/組織B細胞stateを狙う点である。SLE/LNではcevostamabに近くなりすぎるため、初期適応はSjögren腺内B細胞高値またはRA滑膜B細胞高値に置くべきである。

## 安全性リスク
- CD8+ T細胞活性化が病変組織炎症を悪化させる可能性。
- 唾液腺/粘膜内で局所組織傷害が起こる可能性。
- FcRL4+正常粘膜記憶B細胞を除去し、防御免疫を落とす可能性。
- CD3 TCEへ寄せる場合はCRS、ICANS様リスク、感染、低Ig、T細胞疲弊を評価する必要。
- CD8A結合抗体がCD8機能を阻害し、抗ウイルス/抗腫瘍免疫に影響する可能性。

## Developabilityリスク
- CD8A armは、活性化を起こさず単に結合するだけの可能性が高い。
- CD8AはT細胞側の標的であり、親和性が高すぎるとperipheral sinkが大きい。
- CD8A/CD8B、CD8αα/CD8αβ、NK/T細胞subsetへの結合差を制御する必要。
- CD8-biased CD3やtrispecificへ発展させると、分子設計と安全性評価が一気に難しくなる。

## 初期評価系
| 評価 | 実験 |
|---|---|
| 標的存在 | fresh唾液腺/RA滑膜でFcRL4+ B細胞とCD8+ T細胞の距離、頻度、空間配置を見る。 |
| pure CD8A BsAbの成立性 | FcRL4+ B細胞 + autologous CD8+ T細胞でCD69、CD25、CD107a、granzyme B、IFNγ、target killingを測る。 |
| CD8A依存性 | CD8 blocking、MHC-I blocking、TCR stimulationの有無で殺傷が変わるか見る。 |
| CD3 TCEとの差 | FcRL4 x low-affinity CD3、CD19 x CD3、FcRH5 x CD3 benchmarkと比較。 |
| 組織安全性 | salivary gland organoid/sliceで上皮傷害、炎症性サイトカイン、正常粘膜B細胞への影響を見る。 |
| cytokine risk | IFNγ、TNF、IL-2、IL-6、GM-CSFを低標的密度条件も含めて測る。 |

## Kill criteria
- CD8A pure BsAbでFcRL4+ B細胞殺傷が出ない。
- 殺傷に外部TCR/CD3刺激が必須で、BsAb単独の薬理として成立しない。
- FcRL4陰性B細胞や正常粘膜B細胞にも同程度の作用が出る。
- CD8+ T細胞のサイトカインが高く、慢性自己免疫薬として許容できない。
- CD3 TCEへ寄せないと効かず、FcRL4 x CD3と実質的に同じになる。
- Sjögren/RA組織でFcRL4+ B細胞とCD8+ T細胞の空間近接が乏しい。

## 推奨度
**条件付き/低-中。**

革新性は高いが、CD8A単独ではT細胞活性化が不足する可能性が最大の弱点である。最初から主案にするより、`FcRL4+病変B細胞を除去するならどこまで攻めるか` を検証する探索枝として扱う。純粋CD8A BsAbより、低親和性CD3またはCD8-biased TCEへの発展形を比較に入れる方が現実的である。

## 参考文献・リンク
- FcRL4+ B cells in Sjögren salivary glands: https://pubmed.ncbi.nlm.nih.gov/28390747/
- pSS FcRL4+ B cell pathogenic signature: https://pubmed.ncbi.nlm.nih.gov/32201227/
- CD8 co-receptor structure/function review: https://pubmed.ncbi.nlm.nih.gov/39253084/
- CD19 x CD3 BiTE in refractory RA: https://pubmed.ncbi.nlm.nih.gov/38671240/
- CD19 x CD3 blinatumomab in refractory MG: https://pubmed.ncbi.nlm.nih.gov/40583272/
- BCMA x CD3 teclistamab in refractory MG: https://pubmed.ncbi.nlm.nih.gov/40534130/
- FcRL4 competitive landscape: ../../evidence/competitive_landscape/FCRL4_competitor_landscape.md
