# Proposal 2 先輩コメントへの回答メモ

作成日: 2026-07-20

## 目的
FcRL4 x CD22、およびFcRL4 x CD3案に対してもらった以下のコメントに、文献根拠と開発上の見方を整理して回答する。

- FcRL4を標的とした抗体の先行例がないため、開発ハードルが高いかも
- どれくらいFcRL4が発現しているのか
- CD19 x FcγRIIB（obexelimab）との差別化
- FcRL4はマウスでのホモログが存在しないから開発ハードルが高い

結論として、コメントはいずれも妥当であり、完全に論破するべきではない。むしろ、FcRL4案は「臨床validated target」ではなく、**組織病変B細胞stateを狙う高リスク・高新規性のseed**として提示するのがよい。勝ち筋は、最初の実験で発現量、患者選択、anti-FcRL4単独との差、obexelimabとの差を一気に切れる設計にすることである。

## 一言回答
| コメント | 回答の方向性 | プレゼンでの言い方 |
|---|---|---|
| FcRL4抗体の先行例がない | その通り。臨床先行例の少なさは開発ハードル。ただし、FCRL4は膜タンパク質/CD markerで、病理・研究抗体とヒト病変組織データはある。 | 「validated drug targetではないので、最初から発現・薬理・speciesをkill gateに置く。逆に直接競合が少ないのが新規性の源泉。」 |
| どれくらい発現しているか | pSS唾液腺、RA滑膜で存在・局在の根拠はある。pSSではparotid 29/30、labial 17/24で陽性細胞が報告される。ただし、抗体薬に必要な絶対receptor densityは不明。 | 「発現していることは認められているが、薬に十分な密度かは未確定。最初の実験でmolecules/cell相当まで定量する。」 |
| obexelimabとの差別化 | obexelimabはCD19 x FcγRIIBの非除去型・広域B細胞抑制で、IgG4-RDではPhase 3陽性。強いbenchmark。FcRL4 x CD22は病変組織FcRL4+ B細胞にCD22 brakeを入れるniche/state選択型、FcRL4 x CD3は短期reset型。 | 「B細胞全体を抑えるobexelimabに対し、FcRL4案は組織病変B細胞stateを選ぶ。広域B細胞抑制で十分ならobexelimabに勝てない。」 |
| マウスホモログがない | その通り。標準マウス薬効モデルやsurrogate toxが使いにくい。ヒト組織ex vivo、cyno交差性、human FCRL4 KI/ヒト化モデルを初期から組む必要がある。 | 「マウスで効いたから進める、という開発ではなく、ヒト組織薬理を主軸にする。cyno交差性がなければ大きなNo-Go寄り。」 |

## 1. FcRL4標的抗体の先行例がない点

### 事実
2026-07-20時点でClinicalTrials.govを `FCRL4`、`FcRL4`、`CD307d`、`FCRH4` で検索した範囲では、FcRL4を治療標的とする公開臨床試験は確認できなかった。`IRTA1` ではNHLの病理・分子解析試験が1件ヒットするが、治療介入ではない。

一方、FcRL4/IRTA1/CD307dは単なる机上標的ではない。NCBI Geneでは、FCRL4は4つの細胞外Ig-like domain、膜貫通領域、ITIMを持つ膜タンパク質として記載されている。Human Protein Atlasでも膜局在の遺伝子として扱われ、リンパ組織に偏ったRNA発現、リンパ球サブセットでの膜/細胞質染色が報告される。ただしHPAのIHCは、抗体染色とRNAの整合性に注意が必要とされている。

### 考察
先行例がないことは、プラスとマイナスの両方を持つ。

| 見方 | 内容 |
|---|---|
| マイナス | ヒト安全性、標的占有率、薬力学、推奨投与量、species cross-reactivity、epitope薬理が未成熟。 |
| プラス | 直接競合が薄く、CD19/CD20/BAFF/APRIL/FcRn/CD40Lのような混雑領域ではない。 |
| 実務上の意味 | FcRL4案は「後期開発しやすい標的」ではなく、「初期に強い反証実験を置く探索seed」として扱うべき。 |

このコメントへの良い返答は、先行例がないことを否定するのではなく、**だからこそ最初の実験を重くする**ことである。

### 必須の初期kill gate
- ヒト病変組織で、FcRL4+ B細胞が患者選択可能な頻度で存在する。
- FcRL4が細胞表面に十分な密度で出ている。
- anti-FcRL4単独、anti-CD22単独、2剤併用、FcRL4 x CD22が比較できる。
- FcRL4 x CD3では、CD19 x CD3より低いサイトカインでFcRL4+病変B細胞を選択的に殺せる。
- cynomolgus monkeyなど毒性評価種への交差性、またはそれに代わる説得力のあるヒト組織安全性パッケージがある。

## 2. FcRL4発現量はどれくらいか

### 認められていること
FcRL4が病変組織B細胞に存在することは、少なくともSjögren唾液腺とRA滑膜では文献上かなり明確である。

| 疾患/組織 | 報告内容 | FcRL4案への意味 |
|---|---|---|
| 正常組織 | FcRL4は正常ではmucosa-associated B cellの小集団に発現し、血液・脾臓・末梢リンパ節では稀とされる。 | 全身B細胞標的ではなく、粘膜/組織B細胞state標的として見える。正常粘膜B細胞毒性は懸念。 |
| pSS唾液腺 | pSS診断時の唾液腺でFcRL4+細胞が報告され、parotidでは29/30、labialでは17/24で明瞭に検出。parotidの方がlabialより多い。 | 発現の有無は強い。ただしparotid寄りで、labial biopsyだけだと過小評価の可能性。 |
| pSSのLEL | FcRL4+ B細胞はductal epithelium/lymphoepithelial lesion近傍に局在し、PAX5+で増殖性。 | 腺上皮ニッチを狙う仮説と合う。 |
| pSS関連MALT lymphoma | pSS関連parotid MALT lymphomaでFcRL4発現が保存され、mRNAもpSS非リンパ腫parotidより高い。 | MALT risk/前リンパ腫ニッチ患者選択の根拠になる。 |
| pSS血中 | 血中FcRL4+ B細胞はpSSとnon-SS siccaで濃縮されないとの報告。 | 血中flowだけでは患者選択できない可能性。組織/唾液腺バイオマーカーが必要。 |
| RA滑膜 | FcRL4+ B細胞はRA滑膜/滑液に存在し、TNFα/RANKL高発現、citrullinated antigen反応性が多い。 | Sjögren以外の組織B細胞疾患への展開根拠。 |
| 2026年レビュー | FCRL4/FCRL5は活性化CD27- memory B cellに富み、RA、Sjögren、SLE、Graves、MGなどで疾患・文脈依存的に増えると整理。 | FcRL4は単一疾患専用ではなく、組織B細胞state標的として広がる可能性。 |

### まだ不明なこと
ここは先輩コメントの通り、抗体医薬としてはまだ不明点が大きい。

| 不明点 | なぜ重要か | 最初にやる測定 |
|---|---|---|
| receptor density、molecules/cell相当 | BsAb/TCE/ADCでは標的密度が薬効と安全域を決める。 | 定量flow、QIF、標準化IHC、RNAscope、CITE-seq。 |
| 患者内/患者間のばらつき | 一部患者だけなら精密医療になる。 | pSS parotid/labial、RA synovium、normal mucosaのTMA/flow。 |
| CD22との同一細胞共発現 | FcRL4 x CD22がcis co-ligationできるかを決める。 | FcRL4/CD22/CD19/CD20/CD27/IgA/CD11c/T-betの多重染色。 |
| T細胞との空間近接 | FcRL4 x CD3 TCEが組織内で成立するかを決める。 | spatial transcriptomics/IMCでFcRL4+ B cellとCD3/CD8/Tph/Tfh距離を測る。 |
| 正常粘膜B細胞での発現密度 | 安全域を決める。 | 扁桃、Peyer板相当、腸管、口腔粘膜、気道粘膜で比較。 |
| FcRL4発現と臨床症状の相関 | 腺症状以外への効果を説明できるかを決める。 | 腺腫脹、LEL、CXCL13、RF/cryoglobulin、低C4、神経障害/関節痛との相関。 |

### このコメントへの結論
「FcRL4が病変組織B細胞で高発現であることは認められているか？」への答えは、次の表現が安全である。

```text
Sjögren唾液腺、特にparotidのLEL近傍B細胞やpSS関連MALT lymphoma、RA滑膜B細胞でFcRL4+ B細胞が増えることは文献で支持されている。
ただし、抗体医薬の投与設計に必要な絶対発現密度、患者選択cutoff、正常粘膜との差はまだ不明。
したがって、発現は仮説の入口として十分だが、最初のGo/No-Goは発現定量で置く。
```

## 3. CD19 x FcγRIIB（obexelimab）との差別化

### obexelimabの位置付け
obexelimab/XmAb5871は、CD19にFabで結合し、FcγRIIBを改変Fcで高親和性に共架橋する非除去型B細胞抑制抗体である。BCR、TLR9、BAFF/IL-4など複数の活性化経路を抑え、B細胞を大きく枯渇させずに機能抑制する設計である。

公開臨床では、SLE Phase 2では主要評価項目は未達だったが、time to loss of improvementやB-cell pathway high群の探索解析でシグナルがあった。IgG4-RDでは2026年のPhase 3で、週1回皮下注obexelimabがflare riskとステロイド使用量を低下させたと報告されている。したがって、obexelimabは**非除去型B細胞抑制の強いbenchmark**である。

### FcRL4 x CD22との差
| 軸 | obexelimab | FcRL4 x CD22 |
|---|---|---|
| B細胞側の入口 | CD19。広いB-lineage標的。 | FcRL4。粘膜/病変組織/慢性活性化B cell stateに寄せる。 |
| 抑制受容体 | FcγRIIB。BCRと共架橋してITIM brakeを入れる。 | CD22。さらにFCRL4 armがagonisticならFCRL4側ITIMも利用できる可能性。 |
| 薬理 | 非除去型・広域B細胞抑制。 | 病変組織FcRL4+ B細胞のstate/niche選択的silencing。 |
| 患者選択 | B-cell pathway highなど血液/遺伝子発現で選ぶ余地。 | FcRL4+ LEL、parotid腺腫脹、MALT risk、RA滑膜FcRL4+ B細胞など組織biomarkerで選ぶ。 |
| 強み | 臨床validationが強い。IgG4-RD Phase 3陽性。 | 直接競合が薄い。汎B細胞抑制では届かない組織B細胞ニッチを狙える可能性。 |
| 弱み | 広域B細胞作用、CD19陽性B-lineage全体への影響。 | 発現量、species、薬理、抗FCRL4単独との差が未確定。 |

### FcRL4 x CD3との差
| 軸 | obexelimab | FcRL4 x CD3 |
|---|---|---|
| 薬理の強さ | B細胞活性を抑える。原則非除去型。 | T細胞によりFcRL4+ B細胞を短期reset/除去する。 |
| 適した患者 | 慢性的なB-cell activationを抑えたい患者。 | FcRL4+組織B細胞が多い、腺腫脹/MALT risk/難治滑膜炎など、局所B細胞resetが必要な患者。 |
| 主リスク | efficacy不足、持続投与、広域B細胞抑制。 | CRS、局所組織傷害、正常粘膜B細胞除去、発現不足。 |
| 差別化の本質 | FcγRIIB brakeを使う広域抑制。 | B細胞stateを選んだdepletion/reset。 |

### 差別化が成立する条件
FcRL4 x CD22は、単に「CD19をFcRL4に変えたobexelimab類似品」と見られると弱い。差別化を成立させるには、次のいずれかが必要である。

- FcRL4+組織B細胞が、obexelimabで十分に抑えきれない病変ニッチを形成している。
- obexelimabのような広域CD19抑制よりも、FcRL4 gateにより正常B細胞影響を明確に下げられる。
- CD22 co-ligationが、FcRL4+細胞上でanti-CD22単独、anti-FcRL4単独、2剤併用を超える薬理を出す。
- FCRL4 armが単なる住所ではなく、FCRL4側のBCR抑制/ITIM経路を生かすdual brakeになる。
- pSS parotid LEL、MALT-risk、RA滑膜FcRL4+ B cellなど、obexelimabと違う患者定義を作れる。

逆に、次の場合はobexelimabとの差別化は弱くなる。

- 「B細胞を非除去で抑える」以上の説明ができない。
- FcRL4+ B細胞が低頻度で、薬効の大半がCD22単独で説明できる。
- 組織biomarkerなしで全身自己免疫に広く出す。
- CD22 agonismがanti-FcRL4単独を上回らない。

### anti-FcRL4単独との比較を必ず入れる
ユーザー仮説の通り、CD22 agonist活性がなくても、FcRL4を起点に病変B細胞に作用できる可能性がある。したがって、FcRL4 x CD22を推すなら、anti-FcRL4単独を陰性対照ではなく**本命比較対象**として置くべきである。

| 比較 | 期待する判定 |
|---|---|
| anti-FcRL4単独 vs FcRL4 x CD22 | BsAbが単独を上回ればCD22 armの必然性あり。単独が同等ならanti-FcRL4へpivot。 |
| anti-CD22単独 vs FcRL4 x CD22 | FcRL4 gateによる病変B細胞選択性が出るかを見る。 |
| anti-FcRL4 + anti-CD22 2剤併用 vs BsAb | BsAb geometry/cis co-ligationの必然性を見る。 |
| Fc-silent BsAb vs Fc-tuned BsAb | CD22/FCRL4 brakeのみで足りるか、Fc依存性trogocytosis/ADCPが必要かを見る。 |
| obexelimab-like comparator vs FcRL4 x CD22 | 広域CD19/FCGR2B抑制に対して、組織B細胞選択性または安全域で勝てるかを見る。 |

## 4. マウスホモログがない点

### 事実
マウスでFcRL4の明確な一対一ホモログがない、という指摘は妥当である。FCRL familyは種差が大きく、文献ではマウスで確認されるFCRL orthologはFCRL1、FCRL5、FCRL6、FCRLA、FCRLBに限られると整理されている。BgeeのヒトFCRL4 ortholog listにも、Mus musculusは出てこない。一方で、cynomolgus monkeyを含む霊長類にはFCRL4 orthologが掲載されている。

### 開発上の問題
| 問題 | 具体的な影響 |
|---|---|
| 通常マウス薬効モデルが使えない | NOD/ShiLtJなどSjögren様モデル、CIA/CAIAなどRAモデルで、ヒトFcRL4薬理をそのまま見られない。 |
| surrogate抗体が作りにくい | マウス対応分子がなければ、mouse anti-Fcrl4 surrogateで薬効/毒性を見る発想が成立しにくい。 |
| 安全性種の選択が重い | cyno交差性がなければ、GLP toxの説得力が落ちる。 |
| 組織ニッチの再現性が低い | pSSのparotid LEL近傍FcRL4+ B細胞というヒト病理をマウスで再現しにくい。 |
| CD3 TCEでは特に重い | TCEは免疫系全体のspecies差が大きく、ヒトCD3/ヒトFcRL4両方のモデルが必要になりやすい。 |

### de-risk方針
FcRL4案では、マウス中心ではなくヒト組織中心の開発パッケージにする。

1. ヒト病変組織での発現定量を最初に行う。
2. fresh pSS parotid/labial biopsy、RA synovium、扁桃/粘膜正常組織を使ったex vivo薬理を主軸にする。
3. cynomolgus FCRL4への結合、epitope保存性、細胞発現を最初に確認する。
4. cyno交差性がある場合、探索毒性とPK/PDをcynoで組む。
5. cyno交差性がない場合、human FCRL4 knock-in、ヒト免疫系マウス、ヒト唾液腺slice/organoidで補完する。ただし、これはGLP toxの代替としては弱いことを明記する。
6. FcRL4 x CD3は、ヒトPBMC/組織co-cultureでcytokine windowを先に見て、動物薬効は補助扱いにする。

### No-Go条件
- cyno FCRL4への交差性がなく、かつヒト組織ex vivo薬理の再現性も弱い。
- ヒト正常粘膜B細胞への作用が病変B細胞と同等。
- humanized modelで標的依存性が示せない。
- TCEの場合、FcRL4依存的killingに必要な濃度でCRS cytokineが高すぎる。

## CD22案とCD3案への反映

### FcRL4 x CD22
この案は、先輩コメントを踏まえてもまだ残せる。ただし、プレゼンでは「CD22 agonist BsAb」とだけ言うとobexelimab類似に見える。より強い言い方は次である。

```text
FcRL4+病変組織B細胞を選択し、その同一細胞上でCD22/FcRL4の抑制入力を入れるstate-selective tissue B-cell silencer。
```

この案の勝ち筋は、anti-FcRL4単独を超えること、またはanti-FcRL4単独へ素早くpivotできることにある。Fc-silentはdual brakeをきれいに検証するための設計、Fc-tunedはFc依存性trogocytosis/ADCPが必要な場合の設計分岐として残す。

推奨スタンス: **条件付きで継続**。

### FcRL4 x CD3
この案は革新性は高いが、発現量とspeciesの不確実性がより重く出る。慢性Sjögren全般に出すには強すぎる。対象は、FcRL4+組織B細胞が多く、局所B細胞resetの必然性がある患者に絞るべきである。

想定患者は、pSSのparotid腫脹/LEL/MALT-risk、RAの難治滑膜炎、自己抗体神経疾患の一部など。ただし、CD19/CD20/BCMA/FcRH5 x CD3競合が増えているため、FcRL4 x CD3は「TCEをやる」だけでは弱い。**CD19 x CD3より低いサイトカインで病変組織B細胞を選択的にresetできる**ことを示す必要がある。

推奨スタンス: **高リスクの探索枝として継続**。CD22案より開発ハードルは高い。

## 最初にやるべき検証パッケージ
| 優先 | 実験 | 目的 | Go基準 | No-Go基準 |
|---|---|---|---|---|
| 1 | pSS parotid/labial、RA synovium、正常粘膜でFcRL4定量 | 発現量コメントへの回答 | 患者サブセットでFcRL4+ B細胞頻度と表面密度が明確、正常組織との差がある | 発現が低く、患者選択cutoffが作れない |
| 1 | FcRL4/CD22/CD19/CD20/IgA/CD11c/T-betの多重染色 | CD22案の成立性 | FcRL4+細胞でCD22共発現、病変state marker陽性 | CD22共発現が弱い |
| 1 | anti-FcRL4単独、anti-CD22単独、2剤併用、FcRL4 x CD22比較 | BsAbの必然性 | BsAbまたはanti-FcRL4単独がBCR/TLR/Tfh help readoutを抑える | CD22単独と差がない、または活性化する |
| 2 | Fc-silent vs Fc-tuned比較 | Fc依存性trogocytosisの必要性 | Fc-tunedで選択的trogocytosis/ADCP、Fc-silentで十分な抑制のどちらかが成立 | Fc依存作用が非選択的、正常B細胞にも強い |
| 2 | obexelimab-like comparator比較 | 競合差別化 | FcRL4+組織B細胞で選択性、安全域、または組織readoutが上回る | 広域CD19/FCGR2B抑制に全て負ける |
| 2 | FcRL4 x low-affinity CD3 vs CD19 x CD3 | TCE差別化 | 同等killingを低cytokine、かつFcRL4依存的に達成 | CD19 x CD3と同じ広域除去になる |
| 3 | cyno交差性・epitope保存 | species hurdle | cyno細胞/組織に交差し、発現分布がヒトと許容範囲 | cyno非交差、代替パッケージも弱い |

## プレゼン用の回答案
```text
ご指摘の通り、FcRL4は抗体医薬としては先行臨床例がほぼなく、マウスホモログも乏しいため、開発ハードルは高いです。
一方で、pSS唾液腺のLEL近傍やRA滑膜ではFcRL4+ B細胞が文献上確認されており、特にpSS parotidでは高頻度に検出されています。
ただし、抗体薬に必要な発現密度はまだ不明なので、最初のGo/No-Goは発現定量に置きます。

obexelimabはCD19 x FcγRIIBの広域・非除去型B細胞抑制として強いbenchmarkです。
FcRL4 x CD22はそれを模倣するのではなく、FcRL4+病変組織B細胞に限定してCD22/FcRL4 brakeを入れるstate-selective tissue B-cell silencerとして位置付けます。
もし広域B細胞抑制で十分ならobexelimabが強く、我々の案は不要です。
逆に、病変組織FcRL4+ B細胞が患者サブセットの症状やMALT riskを支えていて、そこを選択的に抑える必要があるなら、FcRL4案の意味が出ます。

FcRL4 x CD3はさらに高リスクですが、CD19/CD20 TCEより病変B細胞に寄せた短期reset薬として探索価値があります。
ただし、発現密度、正常粘膜B細胞安全性、cyno交差性が通らなければ早期に止めます。
```

## 最終コメント
先輩コメントを受けた後の提案の形は、次のように少し修正するのがよい。

- FcRL4を「validated clinical target」とは言わない。
- 「発現している」ではなく、「病変組織で検出されるが、薬剤標的密度はこれから定量」と言う。
- obexelimabを敵視せず、強いbenchmarkとして前面に置く。
- CD22案は、obexelimab類似ではなく、FcRL4+病変組織B細胞stateに対するCD22/FcRL4 dual brakeとして説明する。
- CD3案は、慢性維持薬ではなく、FcRL4-high組織B細胞を短期resetする高リスク探索枝として説明する。
- マウスホモログ問題は認め、ヒト組織ex vivoとcyno交差性を最初の開発判断に入れる。

## 参考文献・リンク
- FcRL4+ B-cells in salivary glands of primary Sjögren's syndrome patients. Journal of Autoimmunity 2017. https://pubmed.ncbi.nlm.nih.gov/28390747/
- Gene expression profiling of epithelium-associated FcRL4+ B cells in primary Sjögren's syndrome reveals a pathogenic signature. Journal of Autoimmunity 2020. https://pubmed.ncbi.nlm.nih.gov/32201227/
- Expression of FcRL4 defines a pro-inflammatory, RANKL-producing B cell subset in rheumatoid arthritis. Annals of the Rheumatic Diseases 2015. https://pubmed.ncbi.nlm.nih.gov/24431391/
- B cells expressing the IgA receptor FcRL4 participate in the autoimmune response in patients with rheumatoid arthritis. Journal of Autoimmunity 2017. https://pubmed.ncbi.nlm.nih.gov/28343748/
- The inhibitory potential of Fc receptor homolog 4 on memory B cells. PNAS 2003. https://pubmed.ncbi.nlm.nih.gov/14597715/
- FcRL4 is an IgA receptor that primarily binds the joining chain. PNAS 2026. https://pubmed.ncbi.nlm.nih.gov/42308047/
- Fc receptor-like proteins and their role in B-cell responses and autoimmune diseases. Immunology Letters 2026. https://doi.org/10.1016/j.imlet.2026.107144
- FCRL4 NCBI Gene. https://www.ncbi.nlm.nih.gov/gene/83417
- FCRL4 Human Protein Atlas. https://www.proteinatlas.org/ENSG00000163518-FCRL4/tissue
- FCRL4 Bgee ortholog/expression page. https://www.bgee.org/gene/ENSG00000163518
- Evolution of Fc Receptor-Like Scavenger in Mammals. Frontiers in Immunology 2020. https://www.frontiersin.org/articles/10.3389/fimmu.2020.590280/full
- Antibody-mediated coengagement of FcγRIIb and B cell receptor complex suppresses humoral immunity in systemic lupus erythematosus. Journal of Immunology 2011. https://pubmed.ncbi.nlm.nih.gov/21357255/
- Suppression of innate and adaptive B cell activation pathways by antibody coengagement of FcγRIIb and CD19. mAbs 2014. https://pubmed.ncbi.nlm.nih.gov/24828435/
- Suppression of rheumatoid arthritis B cells by XmAb5871. Arthritis & Rheumatology 2014. https://pubmed.ncbi.nlm.nih.gov/24782179/
- Obexelimab in SLE Phase 2. Arthritis & Rheumatology 2023. https://pubmed.ncbi.nlm.nih.gov/37459248/
- Obexelimab in IgG4-related disease Phase 2 pilot. Lancet Rheumatology 2023. https://pubmed.ncbi.nlm.nih.gov/38251576/
- Obexelimab for the Treatment of IgG4-Related Disease. NEJM 2026. https://pubmed.ncbi.nlm.nih.gov/42233621/
- ClinicalTrials.gov obexelimab IgG4-RD Phase 3, NCT05662241. https://clinicaltrials.gov/study/NCT05662241
- ClinicalTrials.gov obexelimab SLE Phase 2, NCT06559163. https://clinicaltrials.gov/study/NCT06559163
- ClinicalTrials.gov obexelimab wAIHA Phase 3, NCT05786573. https://clinicaltrials.gov/study/NCT05786573
- ClinicalTrials.gov obexelimab relapsing MS Phase 2, NCT06564311. https://clinicaltrials.gov/study/NCT06564311
