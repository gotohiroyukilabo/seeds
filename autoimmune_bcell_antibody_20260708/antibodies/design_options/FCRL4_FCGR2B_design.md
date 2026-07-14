# FcRL4 x FCGR2B BsAb案: 組織B細胞限定FcγRIIbブレーキ

作成日: 2026-07-15

## 位置付け
このファイルは `FCRL4 x CD22` とは別案である。CD22案がSiglec-2/CD22 brakeをFcRL4+ B細胞へ置くのに対し、FcRL4 x FCGR2B案はFcγRIIb/CD32Bという強いB細胞抑制受容体を、FcRL4+病変B細胞stateに限定してco-engageする。

## 1文仮説
FcRL4+唾液腺/滑膜B細胞上でFCGR2Bをcis co-ligateし、BCR/TLR/Tfh helpへの応答を非除去的に抑えるFcRL4 x FCGR2B BsAbを開発する。

## 標的情報
| 項目 | 内容 |
|---|---|
| B細胞側gate | FCRL4 / Fc receptor-like protein 4, UniProt Q96PJ5 |
| 相方 | FCGR2B / Fc gamma receptor IIb, CD32B, UniProt P31994 |
| 局在 | FCRL4、FCGR2Bとも膜タンパク質 |
| 想定format | Fc-silent IgG-like BsAb、FCGR2B低親和性arm |
| 主目的 | FcRL4+病変B細胞の非除去型silencing |

## なぜFCGR2Bを考えるのか
FCGR2BはB細胞の代表的な抑制性Fc受容体で、ITIMを介してBCR応答を下げる。CD19 x FCGR2B型のobexelimab/XmAb5871は、B細胞を枯渇させずに抑制する自己免疫薬理として臨床段階まで進んでいる。

FcRL4 x FCGR2Bの狙いは、obexelimabのように広いCD19+ B細胞へブレーキを入れるのではなく、FcRL4+ disease-state B cellに抑制入力を局在させることである。これはCD22案よりも、既存のFCGR2B co-engagement薬理に近く、薬理実証の足場が強い。

## 現時点の外部根拠
| 論点 | 根拠 | 読み方 |
|---|---|---|
| FCGR2B co-engagementはBCR/TLR応答を抑える | XmAb5871 in vitro studies | BCR、TLR9、Ig産生、サイトカインを落とせる薬理がある。 |
| RA B細胞でも抑制が示される | XmAb5871 RA B cell paper | RA滑膜FcRL4+ B細胞への横展開と相性がよい。 |
| SLE患者B細胞でもFCGR2B co-engagementは抑制的 | SLE humoral immunity paper | CD22よりもBCR抑制の説明がしやすい。 |
| Obexelimabは非枯渇型B細胞治療として臨床化 | SLE Phase 2、IgG4-RD Phase 2/3 | 外部validationが強い一方、CD19 x FCGR2Bとの差別化が必須。 |
| FcRL4+ B細胞はSjögren唾液腺に存在 | pSS FcRL4 literature | FcRL4をCD19の代わりに病変B細胞gateとして使う根拠。 |

## 競合状況
直接のFcRL4 x FCGR2B競合は確認できない。一方で、obexelimabは明確な隣接競合である。

| 競合 | 標的/形式 | 状態 | FcRL4 x FCGR2Bへの意味 |
|---|---|---|---|
| Obexelimab / XmAb5871 | CD19 x FCGR2B | IgG4-RD Phase 3、wAIHA Phase 3、SLE Phase 2など | 薬理validationは強いが、CD19 x FCGR2B後追いに見えやすい。FcRL4 gateの必然性が必要。 |
| CD19/CD20 B cell depletion | 汎B細胞除去 | 多数 | 非除去型silencerとして差別化。 |
| FcRL4 x CD22 | FcRL4 + CD22 brake | 自社案 | CD22よりFCGR2Bの抑制薬理は強そうだが、FCGR2Bはmyeloid/血小板文脈に注意。 |

ClinicalTrials.govではobexelimabがIgG4-RD、wAIHA、SLE、relapsing MSで臨床開発中である。これはFCGR2B co-engagementの競争圧が高いことを意味する。

## 作用機序案
| 設計 | 作用機序 | 期待 |
|---|---|---|
| Fc-silent FcRL4 x FCGR2B cis BsAb | FcRL4+ B細胞上でFCGR2Bを近接させ、ITIM/SHP系を入れる | 主案。非除去型tissue B cell silencer。 |
| FcRL4 x FCGR2B low-affinity FCGR2B arm | FCGR2B単独結合を弱め、FcRL4陽性細胞でだけavidityを出す | peripheral sinkと広範B細胞抑制を避ける。 |
| FcRL4 x FCGR2B pH-tuned/recycling | 組織滞留や受容体占有を調整 | 低優先。まず機能が先。 |
| Fc-active型 | FcγR依存作用も加える | 原則避ける。FCGR2B薬理の解釈が崩れる。 |

## CD22案との違い
| 論点 | FcRL4 x CD22 | FcRL4 x FCGR2B |
|---|---|---|
| ブレーキ受容体 | CD22/Siglec-2 | FCGR2B/CD32B |
| 外部薬理validation | epratuzumab失敗が目立つ | obexelimab/XmAb5871で非枯渇型B細胞抑制の臨床validationがある |
| 新規性 | CD22失敗の再解釈が必要 | obexelimab後追いに見えやすい |
| 差別化軸 | FCRL4とCD22のdual brake | CD19ではなくFcRL4+病変組織B細胞に限定する点 |
| 主な懸念 | CD22 agonismが弱い | FCGR2B競合が強く、差別化が狭い |

## 期待される利点
- CD22より強いBCR/TLR抑制が期待できる。
- obexelimabの先行薬理により、初期PoC設計が明確。
- 非除去型なので慢性Sjögren/RAに合う。
- FcRL4 gateにより、CD19 x FCGR2Bより組織B細胞stateへ寄せられる。
- anti-FcRL4単独、FcRL4 x CD22、obexelimab-like CD19 x FCGR2Bを同一系で比較しやすい。

## 既存薬との差別化
最大の課題はobexelimabである。FcRL4 x FCGR2Bは、単にCD19をFcRL4に置き換えたme-betterでは弱い。

差別化するには、次のどちらかが必要である。

1. FcRL4+病変B細胞ではCD19 x FCGR2Bより強く、FcRL4陰性B細胞では弱い。
2. Sjögren唾液腺/RA滑膜の組織B細胞で、CD19 x FCGR2Bでは届かない病変stateを選べる。

この2点が出ない場合、obexelimabに対する存在理由が薄い。

## 安全性リスク
- FCGR2BはB細胞だけでなくmyeloid系にも関係するため、結合特異性とFc-silent化が重要。
- FCGR2B armの親和性が高いと、FcRL4 gateなしに広くB細胞/免疫細胞へ結合する。
- 正常粘膜FcRL4+ B細胞を慢性的に抑え、防御免疫を落とす可能性。
- FCGR2B co-engagementで過剰にB細胞抑制し、低Igや感染リスクを招く可能性。
- Fc領域が残ると意図しないFcγR bindingが混ざるため、Fc-silent設計が必須。

## Developabilityリスク
- FCGR2B armのepitope/affinityが薬理と安全域を決める。
- FcRL4とFCGR2Bが同一細胞上で十分近接できるか不明。
- FcRL4発現密度が低いと、FCGR2B co-engagementに必要なavidityが足りない可能性。
- CD19 x FCGR2Bとの差別化データを出すため、benchmark抗体が必要。

## 初期評価系
| 評価 | 実験 |
|---|---|
| 共発現 | fresh唾液腺/RA滑膜でFcRL4+ B細胞のFCGR2B発現をflow/spatialで確認。 |
| cis co-ligation | FcRL4 x FCGR2Bが同一B細胞上でFCGR2B phosphorylation、SHP-1/SHIP recruitmentを誘導するか。 |
| BCR抑制 | pSyk、pBLNK、pPLCγ2、Ca flux、pERK、pAKTを測る。 |
| TLR/Tfh抑制 | CpG/TLR9、R848/TLR7、CD40L、IL-21条件でNF-κB、CD86、HLA-DR、Ig産生を見る。 |
| benchmark | anti-FcRL4単独、FcRL4 x CD22、CD19 x FCGR2B-like、anti-CD19/anti-CD20 depletionと比較。 |
| 組織選択性 | FcRL4陽性 vs 陰性B細胞、血中B細胞 vs 腺内B細胞で作用差を見る。 |

## Kill criteria
- FcRL4+ B細胞でFCGR2B共発現が低い。
- FcRL4 x FCGR2BがCD19 x FCGR2B-likeを上回らない。
- FcRL4陰性B細胞にも広く作用し、FcRL4 gateが効かない。
- BCR/TLR/Tfh応答の抑制が弱い。
- FCGR2B armの単独結合で広範な免疫抑制が出る。
- 正常粘膜B細胞で安全域が取れない。

## 推奨度
**中-高。**

3候補の中では最も自己免疫薬らしく、非除去型で慢性疾患に合う。薬理の外部validationも強い。一方で、obexelimab/CD19 x FCGR2Bの後追いに見えやすいため、FcRL4+組織B細胞での選択性と優位性を最初に示す必要がある。

## 参考文献・リンク
- XmAb5871 suppresses BCR/TLR activation: https://pubmed.ncbi.nlm.nih.gov/24828435/
- XmAb5871 in RA B cells: https://pubmed.ncbi.nlm.nih.gov/24782179/
- FcγRIIb/BCR coengagement in SLE B cells: https://pubmed.ncbi.nlm.nih.gov/21357255/
- Obexelimab in SLE Phase 2: https://pubmed.ncbi.nlm.nih.gov/37459248/
- Obexelimab in IgG4-RD Phase 2: https://pubmed.ncbi.nlm.nih.gov/38251576/
- Obexelimab in IgG4-RD Phase 3: https://pubmed.ncbi.nlm.nih.gov/42233621/
- ClinicalTrials.gov obexelimab SLE: https://clinicaltrials.gov/study/NCT06559163
- ClinicalTrials.gov obexelimab IgG4-RD: https://clinicaltrials.gov/study/NCT05662241
- FcRL4+ B cells in Sjögren salivary glands: https://pubmed.ncbi.nlm.nih.gov/28390747/
