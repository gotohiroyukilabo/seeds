# 病態局所的に作用する抗体医薬コンセプトの先行事例

作成日: 2026-07-20

## このメモの問い
今回の大きなコンセプトは次のように定義できる。

```text
自己免疫疾患に対して、全身の免疫を広く抑えるのではなく、
病態局所または病変細胞stateに選択的に作用する抗体医薬品を作る。
```

この発想と同じ、または近い先行事例を調べ、FcRL4 x CD22 / FcRL4 x CD3案への示唆を整理する。

## 結論
同じ思想の先行例は存在する。最も強い成功例は、IBDにおける**vedolizumab**である。これはα4β7 integrinを阻害し、腸管へのリンパ球homingを抑える「gut-selective」抗体として承認されている。

一方で、FcRL4案と完全に同じ先行例、つまり「自己免疫の病変組織に存在するB細胞state markerを使い、その細胞だけを抑制またはresetする抗体/BsAb」は、公開情報上は明確な承認薬・臨床後期品としては見当たらない。

したがって、プレゼン上の言い方は次が良い。

```text
局所選択的免疫介入という発想自体は、vedolizumabなどで臨床的に成立している。
ただし、既存例の多くは「臓器homing」や「炎症ECM」への局所化であり、
FcRL4案は「病変組織B細胞state」をゲートにする点が新しい。
```

## 局所選択性を作る4つの型
| 型 | 代表例 | 作用部位の選び方 | FcRL4案との関係 |
|---|---|---|---|
| 臓器homing gate | vedolizumab、etrolizumab、anti-MAdCAM-1 | 腸管へ入るリンパ球、または腸管内皮addressinを狙う | 「全身免疫を避ける」臨床成功例。FcRL4案は腸ではなく病変B細胞stateをgateにする。 |
| 炎症組織ECM gate | F8-IL10 / Dekavil / PF-06687234 | inflamed tissueのfibronectin extra-domain Aに薬剤を集める | FcRL4案より細胞非特異的。PETや組織PKで局所集積を証明する考え方は参考になる。 |
| 病変細胞state gate | ABBV-3373、litifilimab、FcRL4案 | 活性化TNF+細胞、BDCA2+ pDC、FcRL4+ B細胞などを狙う | FcRL4案に最も近い思想。ただしFcRL4はさらに組織局在性が強い可能性がある。 |
| 条件付き活性化 gate | masked/probody anti-TNF、masked TCE | 炎症/腫瘍局所のproteaseで抗体を活性化する | FcRL4 x CD3の安全化に特に参考。自己免疫ではまだ前臨床中心。 |

## 先行事例1: Vedolizumab

### 概要
Vedolizumabはα4β7 integrinに結合し、MAdCAM-1との相互作用を阻害する抗体である。α4β7は腸管homingリンパ球に発現し、MAdCAM-1は腸管粘膜内皮に関わるため、腸管選択的な炎症抑制を狙う。

### なぜ今回のコンセプトに近いか
Vedolizumabは、「全身免疫を広く抑えるのではなく、病変臓器への免疫細胞の流入を選択的に止める」という意味で、今回のコンセプトの代表的成功例である。

特に重要なのは、natalizumabとの対比である。Natalizumabはα4 integrin全体を抑えるため、α4β1/VCAM-1軸も巻き込み、中枢神経系の免疫監視低下とPMLリスクが問題になった。一方、vedolizumabはα4β7に絞ることで、腸管選択性と安全性のバランスを改善した。

### 成功からの学び
- 局所選択性は、抗体医薬として臨床的に成立しうる。
- 「どの臓器/組織へ入る免疫細胞か」を決めるaddress codeを狙うと、全身免疫抑制との差別化がしやすい。
- 安全性の差別化は、単なる仮説ではなく、natalizumabのような広域標的との比較で強く説明できる。

### 限界
- 腸管選択的ではあるが、IBD病変細胞だけを狙うわけではない。
- 正常腸管免疫やGALTにも影響しうる。
- 作用機序は現在も完全には単純ではなく、ヒトで本当にどの細胞移動を止めているかは議論が残る。

### FcRL4案への示唆
FcRL4案は、vedolizumabの「臓器homing gate」より一段狭い「病変B細胞state gate」を狙う。つまり、臓器全体ではなく、病変組織内のFcRL4+ B細胞に絞る点が差別化である。

一方で、vedolizumabほど標的biologyが成熟していないため、FcRL4案では発現定量と患者選択の初期検証がより重要になる。

## 先行事例2: Etrolizumab

### 概要
Etrolizumabはβ7 integrinを標的とする抗体で、α4β7/MAdCAM-1による腸管homingに加え、αEβ7/E-cadherinによる腸管上皮内保持にも作用する設計だった。

### 結果
UC/CDで大規模Phase 3プログラムが行われたが、UCでは導入試験の一部のみ陽性、維持試験は主要評価項目未達があり、Rocheは2020年に混合結果を公表した。ClinicalTrials.govのUC extension試験NCT02118584は、親試験の混合有効性結果に基づくprogram discontinuationで終了している。

### 学び
- 「より局所的」「より機序的に凝っている」だけでは勝てない。
- 局所選択型抗体でも、患者選択、endpoint、投与量、組織内薬理が合わないと失敗する。
- FcRL4 x CD22でも、「CD22とFcRL4を同時に触るから良い」という説明だけでは弱い。anti-FcRL4単独、anti-CD22単独、2剤併用、obexelimab-like comparatorに対する実験的優位が必要である。

## 先行事例3: Anti-MAdCAM-1抗体 Ontamalimab / SHP647

### 概要
OntamalimabはMAdCAM-1を標的とする完全ヒトIgG2抗体である。MAdCAM-1は腸管粘膜関連のaddressinで、α4β7+細胞の腸管homingに関わる。標的が免疫細胞側ではなく、腸管内皮側にある点がvedolizumabと異なる。

### 結果
Phase 3 UC試験では、導入・維持で臨床寛解や内視鏡改善のシグナルが報告され、安全性上の大きな懸念は示されなかった。ただし、プログラムは2020年に安全性/有効性と無関係の理由で中止されたと論文中に記載されている。

### 学び
- 病変臓器の内皮/vascular addressを標的にして、局所免疫細胞流入を制御する考え方は臨床試験まで進んでいる。
- FcRL4案では、内皮addressではなくB細胞stateを標的にするが、「局所に薬理を寄せる」という説明の系譜として使える。
- ただし、MAdCAM-1/α4β7のような強い臓器homing軸と比べると、FcRL4は疾患・患者ごとのばらつきが大きい可能性がある。

## 先行事例4: F8-IL10 / Dekavil / PF-06687234

### 概要
F8-IL10は、fibronectin extra-domain A（FnEDA）に結合するF8抗体断片に、免疫抑制性サイトカインIL-10を融合したimmunocytokineである。FnEDAは炎症や組織リモデリングで増えるECM成分であり、RA滑膜などの炎症組織へIL-10を届けることを狙う。

### RAでの状況
前臨床では、F8がRA滑膜をよく染色し、F8-IL10が関節炎病変に集積してCIAを抑制した。RA患者3例のPET-guided translational studyでは、[124I]F8-IL10がPET陽性関節に集積し、標的/背景比は平均2.5程度だった。一方で、肝臓・脾臓への取り込みも見られ、全身炎症時のFnEDA発現がbiodistributionに影響する可能性が示された。

ClinicalTrials.govでは、RA Phase Ib（NCT02076659）は完了、RA Phase II（NCT02270632）は新規RA薬の承認に伴うリクルート困難で終了、さらにRAへの関節内投与試験NCT07245992が2026年1月開始としてrecruitingとなっている。

### UCでの状況
PF-06687234として、UC患者でinfliximabへのadd-on Phase IIaが行われた。試験は20例でfutilityにより早期中止され、主要評価項目は未達だった。重要なのは、探索endpointである大腸粘膜組織中PF-06687234濃度が、66検体中1検体でしか定量下限を超えなかった点である。

### 学び
- 「炎症組織に抗体で薬理を届ける」考え方は臨床まで進んでいる。
- しかし、局所標的を選んでも、実際に十分な組織濃度が入らなければ薬効は出ない。
- 組織PK、PET/imaging、biopsy中濃度、標的占有率を早期から測るべきである。
- FcRL4案でも、血中PKだけでは不十分であり、唾液腺/滑膜内のFcRL4+ B細胞への結合・占有を直接見る必要がある。

## 先行事例5: ABBV-3373 / ABBV-154

### 概要
ABBV-3373は、adalimumab様のanti-TNF抗体にglucocorticoid receptor modulator（GRM）を結合したADCである。狙いは、TNFを発現する活性化免疫細胞へGRMを届け、全身グルココルチコイド曝露を避けつつ抗炎症効果を出すことである。

### 結果
RA Phase IIaでは、ABBV-3373はhistorical adalimumab comparatorよりDAS28-CRP改善が大きいと報告された。重篤な有害事象として肺炎、上気道感染、アナフィラキシーショックなどが報告され、投与時間変更後には同様のアナフィラキシーイベントは報告されなかった。

後続のABBV-154はRA、PMR、Crohn病でPhase II試験が行われたが、ClinicalTrials.govではいずれもterminatedで、RAはbusiness decision、PMR/Crohn病はstrategic considerationsと記載されている。公開情報だけでは、明確な有効性失敗または安全性失敗とは断定できない。

### なぜ今回のコンセプトに近いか
これは「抗体で病変細胞stateへ薬理を届ける」という点で非常に近い。FcRL4 x CD22やFcRL4 x CD3はpayload ADCではないが、FcRL4+ B細胞を病変stateとして選択するという考え方はABBV-3373に近い。

### 学び
- 自己免疫でもADC的な発想は既に臨床PoCまで進んでいる。
- ただし、payloadが抗炎症でも、安全性、投与反応、感染、開発戦略が重い。
- FcRL4案でADCを使う場合、慢性Sjögrenでは重すぎる可能性が高い。むしろFcRL4 x CD22のようなsilencing型、またはFcRL4 x CD3の短期reset型の方が説明しやすい。

## 先行事例6: AVX-470

### 概要
AVX-470は、経口投与されるbovine-derived anti-TNF antibodyであり、UCの消化管局所でTNFを中和し、全身曝露を抑えることを狙った抗体製剤である。mAbではなくポリクローナル抗体に近いが、局所作用抗体という意味で参考になる。

### 結果
UC first-in-human試験では、全身血中濃度は低く、便中でTNF結合能を持つbovine Igが検出され、安全性は概ね良好だった。最高用量群では臨床・内視鏡・バイオマーカー改善の傾向が報告されたが、承認薬にはなっていない。

### 学び
- 投与経路で局所化する戦略もある。
- ただし、局所投与/経口投与では、組織深部への到達、病変細胞接触、薬効再現性が問題になる。
- FcRL4案では、唾液腺や滑膜への局所投与は現実的に難しいため、全身投与でも病変B細胞に選択的に作用する設計が必要である。

## 先行事例7: Litifilimab / anti-BDCA2

### 概要
LitifilimabはBDCA2を標的とする抗体で、BDCA2はplasmacytoid dendritic cell（pDC）にほぼ特異的に発現する。BDCA2 engagementによりtype I interferon産生を抑える。

### 結果
2022年のNEJM Phase 2では、cutaneous lupus erythematosusでCLASI-A改善、SLEでは関節数改善が報告された。ただし、二次評価項目の多くは主解析を十分に支持せず、herpes zosterなどの感染関連イベントも報告された。

### なぜ今回のコンセプトに一部近いか
Litifilimabは臓器局所薬ではないが、「全免疫を抑えるのではなく、病態に重要な特殊免疫細胞を狙う」という点でFcRL4案に近い。FcRL4案も、B細胞全体ではなく、病変組織B細胞stateを狙う点が本質である。

### 学び
- 細胞種選択性は、全身免疫抑制の回避に役立つが、完全な局所性ではない。
- 細胞種が希少でも病態駆動力が高ければ薬理は成立しうる。
- FcRL4案では、FcRL4+ B細胞が「数は少ないが病態駆動力が高い」ことを示せるかが鍵になる。

## 先行事例8: Baminercept / LTβR-Ig

### 概要
BaminerceptはLTβR-Ig fusion proteinで、lymphotoxin/LIGHT pathwayを阻害し、Sjögrenの標的組織内リンパ球構造や炎症を変えることを狙った。

### 結果
primary Sjögren's syndromeのPhase IIでは、唾液分泌やESSDAIの主要な臨床改善は示されなかった。一方で、CXCL13低下やB/T細胞サブセット変化など、LTβR signaling阻害を示す薬力学的変化は観察された。関連解析では、LTβR-IgがPD1- naive T cell recruitmentは止めるが、病原性が疑われるPD1+ effector T cellには十分効かない可能性が示唆された。

### 学び
- Sjögrenでは、標的組織のリンパ構造を狙う発想は既に試されている。
- しかし、標的経路が局所病原細胞の中核でなければ、薬力学が出ても臨床効果に繋がらない。
- FcRL4案では、「FcRL4+ B細胞がLEL/腺障害/MALT risk/systemic symptomsに本当に効いているのか」を最初に問うべきである。

## 先行事例9: Masked / protease-activated antibody

### 概要
Masked antibody / probodyは、全身循環中では抗原結合部位をmaskし、病変局所のproteaseでmaskを切って活性化する設計である。臨床開発の中心は腫瘍だが、炎症疾患にも応用可能な思想である。

2026年のmAbs論文では、IGF-II由来maskを使ったprotease-dependent conditional activation抗体が報告され、anti-TNFαではMMP2/9切断後に活性が戻り、collagen antibody-induced arthritis modelでadalimumab/infliximab並みの有効性を維持しつつ、Listeria感染challengeで参照抗体のような生存低下が測定されなかったとされる。さらにanti-IL-1β抗体などにも展開可能性が示された。

### 学び
- 「全身では眠らせ、炎症局所で起こす」設計は、自己免疫抗体薬の安全域拡大に直結する。
- FcRL4 x CD3のようにCRSや正常粘膜B細胞への作用が懸念される設計では、masked CD3 armまたはmasked FcRL4 armが有力な安全化案になる。
- ただし、自己免疫疾患ごとのprotease環境、mask解除効率、正常炎症との区別は未成熟であり、臨床validatedではない。

## FcRL4案の位置づけ
| 比較対象 | 既存コンセプト | FcRL4案の違い |
|---|---|---|
| Vedolizumab | 腸管homingを止める臓器選択型抗体 | FcRL4案は臓器ではなく、病変組織B細胞stateを選ぶ。 |
| Anti-MAdCAM-1 | 腸管内皮addressを標的化 | FcRL4案は内皮ではなく、病態B細胞そのものを標的化。 |
| F8-IL10 | 炎症ECMへ抗炎症payloadを集める | FcRL4案はECMではなく、細胞表面標的を使うため、BsAb/TCE/ADC設計に展開しやすい。 |
| ABBV-3373 | TNF+活性化細胞へGRM payloadを届ける | FcRL4案はB細胞state markerを使い、payloadではなくsilencing/resetも可能。 |
| Litifilimab | pDCという希少病態細胞を抑制 | FcRL4案も希少細胞stateを狙うが、さらに病変組織局在を患者選択に使う。 |
| Masked anti-TNF | 炎症proteaseで抗体を活性化 | FcRL4 x CD3の安全化技術として組み合わせ可能。 |

## FcRL4 x CD22への示唆
FcRL4 x CD22は、先行事例の中ではvedolizumabよりもABBV-3373/litifilimabに近い。つまり「臓器全体」ではなく「病態細胞state」を狙う。

プレゼンでは次のように言うと強い。

```text
vedolizumabが腸管homingを使って免疫抑制を腸へ寄せたように、
FcRL4 x CD22はSjögren腺内やRA滑膜のFcRL4+ B細胞stateを使って、
B細胞抑制を病変局所へ寄せる。
```

ただし、FcRL4 x CD22は「局所に存在する細胞を抑える」だけであり、薬剤自体が局所でのみ活性化されるわけではない。そのため、正常粘膜FcRL4+ B細胞への作用は必ず評価する必要がある。

### FcRL4 x CD22のGo条件
- 病変組織FcRL4+ B細胞でCD22が十分共発現している。
- FcRL4+ B細胞でBCR/TLR/Tfh help readoutがanti-CD22単独、anti-FcRL4単独、2剤併用より強く抑えられる。
- FcRL4陰性B細胞、血中B細胞、正常粘膜B細胞への作用が限定的。
- obexelimab-like CD19 x FcγRIIB comparatorより、組織B細胞選択性または安全域の明確な利点がある。

## FcRL4 x CD3への示唆
FcRL4 x CD3は、先行事例の中では「局所化TCE」という未成熟な領域に入る。CD19/CD20/BCMA x CD3の自己免疫応用は全身B細胞resetに寄っているが、FcRL4 x CD3は病変B細胞stateでresetを狭める設計である。

この案を強くするには、masked antibody技術を組み合わせる価値がある。

| 安全化案 | 狙い |
|---|---|
| low-affinity CD3 | 標的細胞依存性を高め、cytokine releaseを下げる。 |
| FcRL4 2+1 avidity gate | FcRL4高発現細胞でのみTCE活性を上げる。 |
| protease-masked CD3 arm | 炎症局所でのみTCEを活性化する。 |
| protease-masked FcRL4 arm | 全身正常粘膜B細胞への結合を下げる。 |
| local short-course dosing | 慢性投与ではなく短期resetにする。 |

### FcRL4 x CD3のGo条件
- CD19 x CD3より低いcytokineで、FcRL4+病変B細胞を同等以上に減らせる。
- FcRL4低発現/陰性B細胞へのkillingが明確に低い。
- 唾液腺slice/organoidやRA synovium explantで、上皮/滑膜組織傷害が許容範囲。
- masked設計を入れる場合、病変組織proteaseで十分に解除され、血清/正常組織では解除されない。

## 「同じ先行事例があるか」への短い答え
```text
同じ思想の先行例はあります。
代表はvedolizumabで、全身免疫抑制ではなく腸管homingを選択的に抑える抗体として成功しています。
また、F8-IL10/Dekavilのような炎症組織ECMへの薬剤集積、ABBV-3373のような活性化TNF+細胞へのADC、masked anti-TNFのような炎症局所活性化技術もあります。

ただし、FcRL4案のように、自己免疫の病変局所B細胞stateをゲートにして、B細胞をsilenceまたはTCEでresetする先行臨床例は明確には見当たりません。
したがって、コンセプトは先行例に支えられる一方、FcRL4でB細胞stateを狙う点は十分に新規性があります。
```

## 研究開発上の教訓
| 教訓 | 先行例 | FcRL4案での対応 |
|---|---|---|
| 局所選択性は臨床価値になる | vedolizumab | 「全身B細胞抑制ではなく組織B細胞state」という主張を前面に出す。 |
| 局所化だけでは有効性は保証されない | etrolizumab | anti-FcRL4単独、anti-CD22単独、2剤併用、obexelimab-likeと比較する。 |
| 組織濃度を測らないと危険 | PF-06687234 | 唾液腺/滑膜でdrug occupancy、組織PK、標的細胞結合を測る。 |
| 局所標的でも全身炎症で分布が広がる | F8-IL10 | 正常粘膜、肝脾、リンパ組織、炎症非標的組織を確認する。 |
| 自己免疫ADCは成立しうるが重い | ABBV-3373/ABBV-154 | FcRL4 ADCは低優先。まずsilencer/TCE短期resetを検討。 |
| 希少病態細胞を狙う抗体は成立しうる | litifilimab | FcRL4+ B細胞の病態駆動性を、頻度だけでなく機能で示す。 |
| 条件付き活性化はTCE安全化に重要 | masked anti-TNF, probody/TCE技術 | FcRL4 x CD3ではmasked/low-affinity/avidity gateを早期設計に入れる。 |

## 参考文献・リンク
- Vedolizumab mechanism overview. https://pubmed.ncbi.nlm.nih.gov/27252400/
- Vedolizumab for IBD review and natalizumab/PML comparison. https://pubmed.ncbi.nlm.nih.gov/24918648/
- GEMINI long-term safety of vedolizumab. https://pmc.ncbi.nlm.nih.gov/articles/PMC7540482/
- Etrolizumab Phase 3 program overview. https://pubmed.ncbi.nlm.nih.gov/32445184/
- Roche etrolizumab Phase 3 mixed results announcement. https://www.roche.com/media/releases/med-cor-2020-08-10
- Etrolizumab UC extension terminated due to program discontinuation. https://clinicaltrials.gov/study/NCT02118584
- Ontamalimab Phase 3 UC/CD. https://pubmed.ncbi.nlm.nih.gov/38096402/
- Ontamalimab PK/PD. https://pubmed.ncbi.nlm.nih.gov/32119128/
- Ontamalimab long-term UC safety. https://pubmed.ncbi.nlm.nih.gov/33599720/
- Dekavil/F8-IL10 preclinical RA. https://pubmed.ncbi.nlm.nih.gov/19781067/
- Dekavil/F8-IL10 Phase Ib RA. https://pubmed.ncbi.nlm.nih.gov/25438467/
- F8-IL10 PET-guided RA translational study. https://pubmed.ncbi.nlm.nih.gov/30550295/
- F8IL10 RA Phase II, NCT02270632. https://clinicaltrials.gov/study/NCT02270632
- F8IL10 intra-articular RA Phase I, NCT07245992. https://clinicaltrials.gov/study/NCT07245992
- PF-06687234 UC Phase IIa. https://pubmed.ncbi.nlm.nih.gov/41684726/
- ABBV-3373 RA Phase IIa anti-TNF-GRM ADC. https://pubmed.ncbi.nlm.nih.gov/36512671/
- ABBV-3373 RA trial, NCT03823391. https://clinicaltrials.gov/study/NCT03823391
- ABBV-154 RA trial, NCT04888585. https://clinicaltrials.gov/study/NCT04888585
- AVX-470 oral locally acting anti-TNF antibody UC first-in-human. https://pubmed.ncbi.nlm.nih.gov/26822613/
- AVX-470 tissue biomarker study. https://pubmed.ncbi.nlm.nih.gov/26802087/
- Litifilimab anti-BDCA2 in SLE. https://pubmed.ncbi.nlm.nih.gov/36069871/
- Litifilimab anti-BDCA2 in cutaneous lupus. https://pubmed.ncbi.nlm.nih.gov/35939578/
- Baminercept/LTβR-Ig in primary Sjögren's syndrome Phase II. https://pubmed.ncbi.nlm.nih.gov/29604186/
- Sjögren target tissue T-cell subsets and LTβR/LIGHT axis. https://pubmed.ncbi.nlm.nih.gov/27815440/
- Protease-activated pro-antibody concept including anti-TNF. https://pmc.ncbi.nlm.nih.gov/articles/PMC5599682/
- IGF-II masked protease-activated anti-TNF/anti-IL-1β platform. https://pubmed.ncbi.nlm.nih.gov/42093183/
