# 提案2 詳細メモ: FCRL4 x CD22組織B細胞サイレンサー

作成日: 2026-07-08

## 0. このレポートの目的
`outputs/seed_proposal_2.md` の内容を、自分で説明できるレベルまで噛み砕くためのメモである。

中心の問いは、Sjögren病でなぜ組織B細胞を狙うのか、epratuzumabの失敗をどう読むのか、FCRL4 x CD22 BsAbがその失敗とどこまで合致するのかである。

## 1. Sjögren病の基礎
Sjögren病は唾液腺・涙腺の慢性炎症を中心とする自己免疫疾患である。乾燥だけでなく、疲労、関節痛、神経障害、肺病変、腎病変、低補体、高IgG、リンパ腫リスクを伴う患者がいる。

```text
唾液腺炎症 → B細胞/Tfh様細胞集積 → 自己抗体・RF・高IgG → 腺障害/全身病変/リンパ腫リスク
```

Sjögrenを一括りにすると治験は失敗しやすい。B-cell-highで、まだ動かせる腺内B細胞ニッチを持つ患者に絞る必要がある。

## 2. 既存B細胞治療の課題
rituximabはSjögrenで一貫した成功を示していない。理由として、患者集団が広すぎる、乾燥/疲労endpointが難しい、血中B細胞を減らしても腺内ニッチが残る、形質細胞や不可逆組織破壊が残る、などが考えられる。

## 3. FCRL4とは何か
FCRL4はB細胞表面タンパク質で、粘膜・組織にいる記憶B細胞や上皮近傍B細胞の目印になりうる。

| 項目 | 内容 |
|---|---|
| タンパク質 | FCRL4 |
| UniProt ID | Q96PJ5 |
| 役割 | 病変組織B細胞への住所 |
| 根拠 | pSS唾液腺のFCRL4+ B細胞報告 |

ここではFCRL4を「殺す標的」ではなく「薬を病変組織B細胞へ届ける住所」として使う。

## 3.5 FCRL4は住所だけではなくBCRブレーキかもしれない
今回の追加調査で重要なのは、FCRL4を単なる表面マーカーとして扱うより、BCR応答を弱める免疫調節分子として扱った方が提案2の新規性が上がる点である。

文献上、FCRL4/FcRH4陽性の組織型記憶B細胞は、一般的な末梢血記憶B細胞とは異なり、上皮近傍・粘膜組織に局在し、BCR刺激への反応性が低い集団として記載されている。さらにFCRL4はinhibitory receptorとして扱われ、ITIM様のチロシンモチーフを介してSHP系 phosphataseを近づけ、BCR近位シグナルを弱める可能性がある。

```text
BCR刺激
  ↓
CD79A/CD79B ITAM → Lyn/Syk → BLNK/PLCγ2 → Ca flux/ERK/NF-κB
  ↓
FCRL4が同じ膜近傍に入る
  ↓
SHP-1/SHP-2様の脱リン酸化入力
  ↓
pSyk、pBLNK、pPLCγ2、Ca fluxが低下する可能性
```

ただし、ここはまだ強く言い切りすぎない方がよい。FCRL4陽性B細胞でBCR応答が低いことと、抗FCRL4抗体でFCRL4を刺激すれば薬理的にBCR抑制を再現できることは同じではない。提案2では、FCRL4を「住所 + 第二のブレーキ候補」として扱い、実験でFCRL4 agonismが本当に抑制に寄与するかを確認する。

## 3.6 FCRL4 biologyで注意すべき逆向きリスク
FCRL4陽性組織B細胞は、BCR応答が低い一方で、粘膜・慢性炎症・TLR刺激に適応したB細胞stateである可能性がある。つまり、FCRL4を刺激すると常に沈静化するとは限らない。

特に注意するのは次である。

| リスク | 意味 |
|---|---|
| TLR7/9反応の増強 | CpG/R848刺激下でNF-κB、CD86、Ig産生が上がるなら自己免疫では危険。 |
| CD40/IL-21反応の増強 | Tfh helpが強い唾液腺ニッチでB細胞活性化を助ける可能性。 |
| endogenous ligandの遮断 | FCRL4に自然な抑制ligandがある場合、blocking epitopeでは逆にブレーキを外す可能性。 |
| internalizationだけが起きる | 表面FCRL4が減るだけで抑制シグナルが出ない可能性。 |
| 疲弊marker問題 | FCRL4がdriverではなく慢性刺激後の結果にすぎない可能性。 |

したがって、FCRL4 armは「結合できればよい」ではなく、epitopeとgeometryが薬理そのものである。

## 4. CD22とは何か
CD22はB細胞の抑制性受容体で、BCRシグナルにブレーキをかける。UniProt IDはP20273である。

ただしanti-CD22抗体epratuzumabはSLE Phase IIIで失敗している。したがって「CD22を触るだけ」では不十分である。

## 5. なぜFCRL4 x CD22なのか
FCRL4 armで病変組織B細胞を選び、CD22 armでその同じB細胞に抑制シグナルを入れる。

```text
FCRL4+ gland B cell
  ↓
FCRL4 x CD22 BsAbが同じ細胞上で結合
  ↓
CD22/SHP-1系の抑制シグナル
  ↓
BCR/TLR/Tfh helpへの反応が低下
  ↓
抗原提示・Ig産生・局所炎症ニッチが弱まる
```

anti-FCRL4とanti-CD22の2剤併用では、同じ膜ドメインでのcis co-ligationを保証できない。ここにBsAbの必然性がある。

## 5.5 CD22とFCRL4を共刺激する意味
ここでいう共刺激は、B細胞を活性化するcostimulationではなく、2つの抑制性受容体を同じB細胞上で同時に動かす「共抑制刺激」である。より正確には、FCRL4 x CD22 BsAbによるdual inhibitory co-agonismである。

狙いは次の3層で考えると分かりやすい。

| 層 | 役割 | 成功した時の意味 |
|---|---|---|
| FCRL4 gate | FCRL4陽性の病変組織B細胞を選ぶ | 血中/正常B細胞への作用を抑える。 |
| CD22 brake | CD22/SHP-1系でBCR応答を下げる | epratuzumabで足りなかったCD22薬理を、病変B細胞に集中させる。 |
| FCRL4 brake | FCRL4側のBCR抑制入力を同時に使う | CD22単独では弱い抑制を、別の抑制受容体入力で補強する。 |

この考え方にすると、提案2は「FCRL4で住所を付けたCD22抗体」から、「病変組織B細胞に2つの内因性ブレーキを同時に入れるBsAb」に変わる。ここがかなり革新的で、プレゼン上も強い。

一方で、CD22とFCRL4の両方がSHP系に寄るなら、完全に独立なブレーキではなく冗長かもしれない。この場合、BsAbは相乗ではなく、単にCD22単独と同程度になる可能性がある。逆に、CD22はSiglec系、FCRL4は組織記憶B細胞stateに紐づく抑制受容体なので、膜上の位置、ligand依存性、internalization、TLR/CD40との接続が違えば、相補的になる可能性がある。

## 5.6 共刺激で一番見たいデータ
最も欲しい結果は、Fc-silent FCRL4 x CD22 BsAbがanti-CD22単独、anti-FCRL4単独、anti-FCRL4 + anti-CD22併用を超えて、FCRL4+ B細胞だけでBCR近位シグナルを落とすことである。

```text
理想データ

FCRL4+CD22+ gland B cell
  anti-CD22単独            → 少し抑制
  anti-FCRL4単独           → 少し抑制、または条件依存
  anti-FCRL4 + anti-CD22   → 中等度抑制
  FCRL4 x CD22 BsAb        → pSyk/pBLNK/pPLCγ2/Ca fluxが明確に低下
  FCRL4陰性B cell          → 作用が弱い
```

この結果なら、BsAbである必然性が非常に強い。2剤併用を超えることができれば、「同じ膜上で2つのブレーキを配置する空間薬理」が主張できる。

## 5.7 抗FCRL4単独は弱い対照ではない
抗FCRL4単独は、単なる比較対照ではなく、独立した候補として扱うべきである。理由は、CD22 agonismがなくても、FCRL4+ disease-state B cellそのものを狙えるからである。

この視点はかなり重要である。もしFCRL4+ B細胞が病変組織ニッチの中心で、自己抗体、抗原提示、Tfh help、TLR応答を担っているなら、CD22にブレーキを入れなくても、FCRL4+細胞だけを抗体でmodulateするだけで効く可能性がある。

```text
FCRL4+ gland B cell
  ↓
抗FCRL4抗体が結合
  ↓
1. FCRL4 signalingでBCR/TLR反応を抑える
または
2. FcγR依存にtrogocytosis/ADCP/軽度depletion
または
3. IgA/J-chain/FCRL4軸を調節
  ↓
病変B細胞ニッチが弱まる
```

つまり、FCRL4 x CD22 BsAbは「抗FCRL4単独では足りない」ことを示して初めて本当に必要になる。抗FCRL4単独が同等なら、BsAbではなく抗FCRL4単独へpivotした方がよい。

## 5.8 抗FCRL4単独の3つの設計
| 設計 | 狙い | 成功した時の意味 | リスク |
|---|---|---|---|
| Fc-silent agonist anti-FCRL4 | FCRL4 signalingだけでBCR/TLR/Tfh反応を抑える | CD22 agonism不要。最も単純なsilencer。 | HCK/FGR文脈で逆にTLR/NF-κBやIg産生が増える可能性。 |
| Fc-active/Fc-tuned anti-FCRL4 | FCRL4+病変B細胞をtrogocytosis、ADCP、軽度depletionでmodulate | state/niche B細胞を直接叩ける。 | 正常粘膜FCRL4+ B細胞、局所炎症、過剰depletion。 |
| non-blocking Fc-silent anti-FCRL4 | 内因性IgA/J-chain/FCRL4調節を邪魔せず結合 | 安全なanchor benchmark。 | 結合だけで薬効が出ない可能性。 |

blocking anti-FCRL4は慎重に扱う。FCRL4-IgA/J-chain軸が病的なら遮断は有効かもしれないが、FCRL4の内因性抑制を外すと逆にBCR/TLR応答が増える可能性がある。

## 5.9 FcRL4標的の競合ランドスケープ
今回の競合調査で一番大事な結論は、FcRL4そのものを標的にした公開臨床競合は見つからない一方で、近縁のFCRL5/FcRH5はかなり動いている、ということである。

ClinicalTrials.govでは、`FCRL4`、`FcRL4`、`FCRH4`、`FcRH4`、`CD307d` の検索で登録試験は0件だった。`IRTA1` は1件出るが、これは非ホジキンリンパ腫の病理・分子解析で、治療薬ではない。

一方、FCRL5/FcRH5ではcevostamabがある。これはFcRH5 x CD3 T-cell engagerで、多発性骨髄腫では複数試験が走っている。さらに重要なのは、SLE with/without active lupus nephritisを対象にしたPhase Ib試験が2026-07-31開始予定で登録されている点である。

```text
FcRL4直撃競合: 公開臨床ではほぼ空白
FCRL5隣接競合: すでにBsAb/T-cell engagerで自己免疫へ入り始めた
```

これはProposal 2にとって悪い話だけではない。FCRL familyが抗体薬の標的になりうることを外部が検証してくれるからである。ただし、社内プレゼンでは「FCRL5 x CD3があるならFcRL4 x CD22は何が違うのか」と必ず聞かれる。

答えは次である。

| 論点 | FCRL5 x CD3/cevostamab | FcRL4 x CD22 Proposal 2 |
|---|---|---|
| 主作用 | T cell engagerによるB-lineage/plasma cell系の強いdepletion | FcRL4+組織B細胞の抑制的silencing |
| 主疾患 | MM、SLE/LNへ展開 | B-cell-high Sjögren、特に腺内/粘膜B細胞ニッチ |
| 安全性論点 | CRS、感染、過剰B細胞/形質細胞抑制 | 正常粘膜FcRL4+ B細胞、局所炎症、Fc活性の有無 |
| 差別化軸 | 強い細胞傷害 | 組織state選択 + dual brake + 慢性自己免疫向け |

したがって、Proposal 2は「FCRL family標的の二番煎じ」ではなく、「FCRL5 x CD3のように殺しにいくのではなく、FcRL4+病変組織B細胞を沈める」というポジションにする。競合詳細は [FCRL4_competitor_landscape.md](../evidence/competitive_landscape/FCRL4_competitor_landscape.md) にまとめた。

## 6. epratuzumabの失敗をどう読むか
epratuzumabの失敗を「CD22 biology完全否定」と読むのは粗い。より正確には次である。

```text
広いSLE集団で、CD22単独modulationを標準治療に上乗せしても明確な臨床差が出なかった。
```

失敗した組み合わせは、CD22単独、広いSLE、組織B細胞ニッチ非選択、biomarker非選択、標準治療上乗せである。

## 7. epratuzumab失敗とFCRL4 x CD22の合致
| epratuzumabから見える失敗仮説 | FCRL4 x CD22の返答 | 合致度 |
|---|---|---|
| 患者選択が粗い | FCRL4+ gland B-cell-highに絞る | 高い |
| 組織B細胞ニッチを狙っていない | FCRL4を唾液腺B細胞住所にする | 高い |
| CD22単独modulationが弱い | FCRL4上でCD22をco-ligateする | 中-高 |
| placebo/標準治療で差が薄まる | 初期PoCはex vivo組織機能で見る | 中 |
| Fc依存trogocytosisが作用の一部かもしれない | Fc-silentで真のCD22/SHP-1抑制を直接確認する | 注意が必要 |

最後の点が最重要である。epratuzumabの作用にはFcγR陽性細胞を介したtrogocytosis、つまりB細胞表面分子の引き抜きが関わる報告がある。もしそれが主作用なら、Fc-silent FCRL4 x CD22は弱くなる可能性がある。

## 8. Fc依存性trogocytosisとは何か

trogocytosisは、免疫細胞同士が接触した時に、一方の細胞がもう一方の細胞膜の一部を「かじり取る」ように取り込む現象である。抗体薬の文脈では、標的細胞表面に結合した抗体のFc部分が、単球、NK細胞、顆粒球などのFcγRに結合することで起こりうる。

epratuzumabの場合は、概念的には以下のように理解できる。

```text
epratuzumabがB細胞上のCD22に結合
  ↓
抗体Fcが単球/NK細胞/顆粒球などのFcγRに結合
  ↓
FcγR陽性細胞がB細胞膜の一部を引き抜く
  ↓
CD22だけでなく、近傍のCD19、CD21、CD79bなどもB細胞表面から減る
  ↓
BCR co-receptor機能が弱まり、B細胞反応性が下がる可能性
```

重要なのは、これは典型的なADCCのようにB細胞を殺す現象とは限らない点である。むしろ「B細胞表面の受容体セットを書き換える」作用に近い。ただし、FcγR陽性細胞に依存するため、組織のmyeloid cell量、FcγR発現、炎症状態で作用が変わりやすい。

## 9. それでもなぜFc-silentから始めるのか

Fc依存性trogocytosisが重要かもしれないなら、最初からFc-activeにすべきではないか、という疑問はもっともである。ただし、この提案でFc-silentを主案に置く理由は4つある。

| 理由 | 内容 |
|---|---|
| 1. 機序をきれいに切り分けるため | FCRL4 x CD22の本当に新しい点は、FCRL4陽性組織B細胞上でCD22 brakeを入れる空間薬理である。Fc-activeだと、CD22/SHP-1抑制なのか、trogocytosisなのか、depletionなのかが混ざる。 |
| 2. 慢性Sjögrenでの安全性 | 唾液腺病変にはmyeloid cellも存在しうる。Fc-activeで非選択的trogocytosisや炎症、局所組織障害が出ると慢性疾患には重い。 |
| 3. epratuzumabの単純再現を避けるため | epratuzumab様Fc依存modulationを繰り返すだけなら新規性が弱い。Fc-silentで効けば、epratuzumabを超える説明がしやすい。 |
| 4. Fc-activeはbackupとして評価できるため | Fc-silentで効かない場合でも、FCRL4 gateによりtrogocytosisを病変B細胞へ限定できるなら、Fc-active/Fc-tuned設計へpivotできる。 |

つまり、Fc-silentは「trogocytosisは不要」と決め打ちしているのではない。最初に最もクリーンな仮説を検証し、必要ならFc-activeへ分岐するための設計である。

## 10. 必須比較実験
| 比較対象 | 目的 |
|---|---|
| anti-CD22単独 | epratuzumab様modulationを超えるか |
| anti-FCRL4 Fc-silent agonist | FCRL4 ligation単独でBCR抑制または逆活性化が起きるか |
| anti-FCRL4 neutral/non-blocking | FCRL4結合だけの安全性と内因性ligand温存を見る |
| anti-FCRL4 Fc-active/Fc-tuned | FCRL4+病変B細胞のFc依存modulationが成立するか |
| anti-FCRL4 + anti-CD22併用 | BsAbの空間薬理が必要か |
| FCRL4 x CD22 Fc-silent | dual inhibitory co-agonismで抑制できるか |
| FCRL4 x CD22 Fc-active | Fc依存trogocytosisが必要か |

Fc-silent BsAbだけがFCRL4+ gland B cellのBCR/TLR/Tfh反応を強く抑えるなら、epratuzumab失敗とFCRL4 BsAbのメリットは最もきれいに合致する。

一方、抗FCRL4単独がBsAbと同等または上回るなら、BsAbの必然性は下がる。その場合は、抗FCRL4単独を主案にする方が、分子が単純で、CMCも臨床説明も楽になる。

一方、Fc-activeでしか効かない場合も即中止ではない。その場合は、FCRL4 gateによってtrogocytosisが病変B細胞に限定されるか、正常粘膜B細胞や血中B細胞に広く起きないかを見る。限定できるなら、Fc-silent tissue-silencerではなく、FCRL4-gated Fc-active tissue modulatorとして再設計する余地がある。

## 11. 抗体設計
主案はFc-silent FCRL4 x CD22 BsAbである。Fc-silentにする理由は、組織B細胞をむやみに殺さず、CD22とFCRL4の抑制シグナルそのものを見たいからである。ただし、Fc-active/Fc-tuned BsAbも初期から比較に入れる。ADCは慢性Sjögrenでは重いので低優先。

FCRL4 armは、単に高親和性であればよいわけではない。少なくとも以下の設計を横比較する。

| FCRL4 arm設計 | 目的 |
|---|---|
| agonist epitope | FCRL4側のBCR抑制を積極的に入れる。 |
| neutral anchor epitope | FCRL4を住所としてだけ使い、CD22薬理を主に見る。 |
| non-blocking epitope | endogenous inhibitory ligandを邪魔しない。 |
| internalizing epitope | ADCやtarget removal向きだが、本提案では低優先。 |

## 12. 患者選択
唾液腺FCRL4/IRTA1様B細胞、CXCL13、focus score、RF、低C4、高IgG、腺エコーを組み合わせる。乾燥症状だけの患者は最初の対象にしない。

## 12.5 腺外症状には効くのか
Sjögren病は乾燥だけの疾患ではない。関節痛、疲労、神経障害、皮膚紫斑、肺、腎、リンパ腫リスクなどがある。したがって、FCRL4+腺内B細胞に絞った時に、腺外症状まで効くのかは必ず聞かれる。

答えは、「全部に効くとは言わない。B細胞高活動性とつながる腺外症状だけ狙う」である。

```text
FcRL4+腺内B細胞
  ↓
腺局所のBCR/TLR/Tfh反応、CXCL13、BAFF/APRIL、RF/IgA/RF clone
  ↓
血中B-cell-high signature、cryoglobulin、低C4、高IgG
  ↓
一部の腺外症状、特に血管炎/紫斑/cryoglobulinemic neuropathy/リンパ腫リスク
```

このつながりがある患者なら、腺外症状も動く可能性がある。一方で、慢性疼痛、疲労、brain fog、小線維/自律神経障害、不可逆な神経障害は、FcRL4+ B細胞を抑えても動かない可能性が高い。

| 腺外症状 | 期待 | 理由 |
|---|---|---|
| 関節痛/関節炎 | 中 | pSS関節痛でFcRL4直接証拠は少ない。ただしRA滑膜ではFcRL4+ B細胞がRANKL/TNFを出すため、真の滑膜炎を伴う患者では狙える可能性。 |
| 神経障害 | 低-中 | cryoglobulinemic/vasculitic neuropathyならB細胞-免疫複合体軸で可能性。非vasculitic neuropathyは弱い。 |
| 皮膚紫斑/血管炎 | 中 | RF、cryoglobulin、低C4と連動するなら可能性。 |
| 腎/肺病変 | 低-中 | 病型依存。MALT/リンパ組織ニッチやcryoglobulinと関係する場合だけ狙う。 |
| 疲労/brain fog/慢性疼痛 | 低 | 多因子性。primary endpointにしない。 |

つまり、提案2の対象患者は「乾燥症状がある人」ではなく、「腺内FCRL4+ B細胞が高く、全身B-cell-high signatureも持つ人」である。

## 12.6 FcRL4起点で他疾患に広げられるか
他疾患展開で最も重要なのは関節リウマチである。RAでは、FcRL4+ B細胞が滑膜液/滑膜組織に存在し、RANKLやTNFを高発現する炎症性B細胞として報告されている。また、RA滑膜FcRL4+ B細胞由来抗体がシトルリン化自己抗原に反応する報告もある。

これはかなり面白い。なぜなら、SjögrenでのFCRL4 x CD22は「唾液腺組織B細胞のdual brake」だが、RAでは「滑膜組織B細胞のdual brake」として横展開できるからである。

| 疾患 | 展開可能性 | コメント |
|---|---|---|
| RA滑膜B細胞高値/難治性RA | 高 | FcRL4+RANKL+ B細胞の根拠がある。競合は過密だが、組織B細胞state標的としては面白い。 |
| Sjögren関連MALT lymphoma/前リンパ腫 | 中-高 | FcRL4/IRTA1とMALT/LELの関係が強い。ただし自己免疫薬より腫瘍薬に近づく。 |
| IgA/粘膜B細胞関連疾患 | 中 | FcRL4はsystemic IgA receptor。IgA nephropathyや粘膜免疫疾患は仮説止まり。 |
| SLE/LN | 低-中 | exhausted/atypical B cell文脈はあるが、CD22失敗の本丸なので組織gateがないと弱い。 |
| Graves/Hashimoto/MG | 低 | FCRL発現報告はあるが、FcRL4+組織B細胞標的としてはまだ遠い。 |
| ANCA、膜性腎症、水疱症、強皮症、IBD | 低 | 現時点ではFcRL4直接証拠が乏しい。 |

RAへ広げる場合も、血液ではなく滑膜で見る。滑膜FcRL4+CD22+ B細胞、RANKL、TNF、IgA、ACPA反応性、BCR/TLR応答を確認し、FCRL4 x CD22 BsAbがanti-CD22単独や2剤併用を超えるかを見る。

## 13. 主なリスク
FCRL4がdriverでない、FCRL4 agonismがBCR抑制を再現しない、FCRL4 ligationでTLR7/9やTfh help反応が増える、腺外症状がFcRL4+腺内B細胞と連動しない、CD22 agonismが弱い、Fc-silentで効かない、Fc-active化で非選択的trogocytosisが出る、唾液腺到達が悪い、粘膜記憶B細胞を抑えすぎる、endpointが遅い。

## 14. 最初にやるべき検証
fresh唾液腺サンプルでFCRL4+CD22+ B細胞の頻度、クローン拡大、Tfh相互作用、CD22/SHP-1抑制、FCRL4側のSHP-1/SHP-2 recruitment、BCR/TLR反応、B-T co-cultureでのIg産生低下を確認する。Fc-active条件では、CD22/CD19/CD21/CD79bの表面低下、FcγR陽性細胞依存性、正常B細胞への広がりも測る。

BCR抑制のreadoutは、pSyk、pBLNK、pPLCγ2、Ca flux、pERK、pAKT、NF-κB、CD86/HLA-DR、Ig産生を最初から入れる。TLR7/9、CD40、IL-21刺激で逆に増える場合は重要な地雷として扱う。

腺外症状については、ESSDAI domain別に見る。特に関節、末梢神経、皮膚、腎、肺を分ける。関節症状は超音波/MRIで滑膜炎を確認し、神経障害はcryoglobulinemic/vasculitic neuropathyと非vasculitic neuropathyを分ける。血液ではCXCL13、BAFF、IL-21、RF、cryoglobulin、C4、高IgG、形質芽細胞を同時に測る。

## 15. 継続/中止基準
継続条件: FCRL4+ B細胞が病変に存在し、病態関連で、BsAbがanti-CD22単独、anti-FCRL4単独、2剤併用を上回る。理想はFc-silentでもBCR近位シグナルとIg産生/抗原提示の抑制が出ること。Fc-activeでのみ効く場合は、trogocytosisがFCRL4陽性病変B細胞に限定され、安全域があることを条件に継続する。

中止条件: FCRL4が無関係、FCRL4 ligationでBCR抑制が出ないだけでなくTLR7/9/CD40/IL-21反応が増える、CD22抑制なし、anti-CD22単独/2剤併用と差がない、Fc-active化で非選択的trogocytosisや炎症が出る、汎B細胞除去が必要。

## 16. 最終コメント
この提案は非常にプレゼンしやすい。epratuzumabの失敗を「CD22はダメ」と捨てるのではなく、「CD22単独・広いSLE・組織非選択では足りなかった」と再解釈し、その弱点をFCRL4 gateとBsAb geometryで補うからである。

ただし、Fc-silentで本当にCD22/SHP-1 brakeとFCRL4側のBCR抑制が出るかは賭けである。出なかった場合も、Fc-activeにすれば救える可能性はあるが、その時は「epratuzumab様作用をFCRL4で病変B細胞に限定できるか」が勝負になる。

今回の追加考察を踏まえると、提案2の一番強い言い方は次である。

```text
FCRL4を住所として使うだけでは普通のretargetingだが、
FCRL4を第二のBCR brakeとしてCD22と同時に使えれば、
病変組織B細胞にだけdual inhibitory signalを入れる新しい抗体薬理になる。
```

## 17. 主要参考文献
- Epratuzumab Phase III EMBODY: https://doi.org/10.1002/art.39856
- Epratuzumab Phase IIb EMBLEM: https://doi.org/10.1136/annrheumdis-2012-202760
- Epratuzumab trogocytosis: https://doi.org/10.1182/blood-2012-12-473744
- FcRL4+ B cells in Sjögren salivary glands: https://doi.org/10.1016/j.jaut.2017.03.012
- Gene expression profiling of epithelium-associated FcRL4+ B cells in pSS: https://doi.org/10.1016/j.jaut.2020.102439
- RA FcRL4+ RANKL-producing B cells: https://doi.org/10.1136/annrheumdis-2013-204116
- RA FcRL4+ B cells and citrullinated autoantigens: https://doi.org/10.1016/j.jaut.2017.03.004
- FcRH4/FCRL4 tissue-based memory B cells: https://doi.org/10.1084/jem.20050879
- FCRL4-bearing memory B cells and commensal antigens: https://doi.org/10.4049/jimmunol.1701549
- FCRL4-mediated immune regulation via HCK/FGR: https://doi.org/10.4049/jimmunol.1401533
- FCRL4 as IgA receptor: https://doi.org/10.4049/jimmunol.1102651
- FCRL4 systemic IgA/J-chain biology: https://doi.org/10.4049/jimmunol.2000293
- FcRL4 J-chain binding structure: https://doi.org/10.1073/pnas.2600183123
