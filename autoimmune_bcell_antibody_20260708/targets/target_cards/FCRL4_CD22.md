# 標的カード: FCRL4 x CD22 組織B細胞サイレンサー

## 要約
- 標的: FCRL4 / Fc receptor-like protein 4, UniProt Q96PJ5。CD22 / Siglec-2, UniProt P20273。
- 疾患: 腺内B細胞高値・異所性リンパ組織型Sjögren病。
- モダリティ: Fc-silent FCRL4 x CD22 BsAb。
- 推奨度: discovery seedとして高。fresh tissue biologyが出るまでは臨床確度中。
- 仮説: 全B細胞ではなく、唾液腺病変のFCRL4陽性組織B細胞にCD22 brakeとFCRL4 brakeを同時に入れる。

## なぜ重要か
Sjögren開発は、広い患者集団と曖昧なendpointで失敗しやすい。FCRL4陽性の腺内B細胞を標的にすれば、B-cell-highでリンパ腫リスクや全身活動性を持つ患者に絞れる可能性がある。

## スコア
| 評価軸 | 点数 | 理由 |
|---|---:|---|
| 未充足ニーズ | 5 | disease-modifying biologicが乏しい。 |
| 標的biology | 4 | 唾液腺FCRL4+ B細胞の根拠に加え、FCRL4自体がBCR抑制性分子である可能性がある。ただし抗体agonismで再現できるかは未確定。 |
| 抗体適性 | 4 | 両標的とも細胞表面。 |
| 差別化 | 5 | 組織state標的 + inhibitory co-ligation。 |
| 安全域 | 4 | FCRL4 gateが効けば汎B細胞除去を避けられる。 |
| バイオマーカー | 4 | 腺組織、CXCL13、RF、低C4、高IgG。 |
| 開発容易性 | 3 | BsAb geometryとCD22 agonismが難しい。 |

## 既存ランドスケープ
CD22抗体epratuzumabはSLE Phase IIIで失敗した。ただしこれは「CD22 biology完全否定」ではなく、広い非バイオマーカー選択SLEでCD22単独modulationが標準治療上乗せに勝てなかった、と読むべきである。Sjögrenではrituximabの結果も一貫しない。BAFF、CD40L、FcRnは進んでいるが、組織B細胞state選択ではない。

## FcRL4標的の競合ランドスケープ
2026-07-12時点の公開情報では、FcRL4/FCRL4/CD307d/FCRH4を直接標的にした臨床段階の抗体薬、BsAb、ADC、CAR-Tは確認できなかった。ClinicalTrials.govでは `FCRL4`、`FcRL4`、`FCRH4`、`FcRH4`、`CD307d` の検索で登録試験0件である。`IRTA1` は1件ヒットするが、非ホジキンリンパ腫の病理・分子解析試験であり、治療薬競合ではない。

ただし、競争上の本命は近縁のFCRL5/FcRH5である。Genentech/RocheのcevostamabはFcRH5 x CD3 T-cell engagerとして多発性骨髄腫で開発され、さらにSLE with/without active LNを対象にしたPhase Ib試験が2026-07-31開始予定で登録されている。これはFcRL4直接競合ではないが、FCRL familyを自己免疫B細胞薬に使う流れが始まったという意味で重要である。

したがって本提案の競合メッセージは「FcRL4直撃は空白。ただしFCRL5 x CD3が自己免疫に入るため、FCRL family競争は始まっている」である。差別化は、全身性T-cell engager/depletionではなく、FcRL4+組織B細胞をFc-silentまたはFc-tunedに沈静化する点に置く。

詳細: [FCRL4_competitor_landscape.md](../../evidence/competitive_landscape/FCRL4_competitor_landscape.md)

## 抗体である必然性
FCRL4を病変組織B細胞への住所、CD22を抑制受容体として、同じ細胞上でcis co-ligationする必要がある。さらに、FCRL4自体もBCR抑制性の免疫調節分子として働く可能性があるため、FCRL4 x CD22 BsAbは「住所付きCD22抗体」ではなく「FCRL4陽性病変B細胞に2つの抑制入力を置く抗体」として設計できる。2剤併用では同じ膜ドメインでの空間制御を保証できない。

## FCRL4のBCR抑制をどう読むか
FCRL4/FcRH4陽性B細胞は、組織局在性の記憶B細胞集団として記載され、BCR応答が低い集団として扱われてきた。FCRL4はinhibitory receptorとして位置付けられ、ITIM様チロシンモチーフを介してSHP-1/SHP-2系を近づけ、BCR近位シグナルを落とす可能性がある。

ただし、重要な不明点がある。

| 論点 | 現時点の解釈 |
|---|---|
| FCRL4陽性細胞でBCR応答が低い | 既存文献と整合する。 |
| 抗FCRL4抗体でFCRL4をagonizeできる | 未確定。epitopeとcrosslinking geometry依存。 |
| FCRL4がSjögren病変でdriverか | 未確定。bystander/慢性刺激markerの可能性あり。 |
| FCRL4刺激が常に抑制的か | 未確定。TLR7/9、CD40、IL-21反応を増やすリスクを測る必要がある。 |

したがって、FCRL4は「住所 + 第二のブレーキ候補」と表現するのが最も正確である。

## CD22とFCRL4の共刺激仮説
ここでいう共刺激は活性化costimulationではなく、dual inhibitory co-agonismである。CD22はSiglec系のBCR抑制受容体、FCRL4は組織記憶B細胞stateに紐づく抑制候補であり、両者を同じB細胞膜上で近接させることでBCR microcluster近傍の脱リン酸化入力を増やす。

| シナリオ | 解釈 | 開発判断 |
|---|---|---|
| CD22単独 < FCRL4単独 < BsAb | dual brakeが成立。最も強いGo。 |
| CD22単独 < BsAb、FCRL4単独は弱い | FCRL4は主に住所。Go可能だが新規性はやや下がる。 |
| 2剤併用とBsAbが同等 | BsAb geometryの必然性が弱い。再設計またはNo-Go。 |
| FCRL4 ligationでTLR7/9/CD40/IL-21反応が増える | 自己免疫では危険。原則No-Goまたはneutral anchor epitopeへ変更。 |
| FCRL4刺激で抑制なし、CD22も弱い | No-Go。 |

## 抗FCRL4単独との比較
抗FCRL4単独は、FCRL4 x CD22 BsAbの単なる対照ではなく、独立候補である。CD22 agonismが弱くても、FCRL4+ disease-state B cellを直接標的化できるなら薬理は成立しうる。

| 抗FCRL4単独設計 | 狙い | BsAbとの関係 |
|---|---|---|
| Fc-silent agonist anti-FCRL4 | FCRL4 signalingだけでBCR/TLR/Tfh反応を抑える | これが十分効けばCD22 armは不要。 |
| Fc-active/Fc-tuned anti-FCRL4 | FCRL4+病変B細胞に限定したADCP/trogocytosis/軽度depletion | CD22非依存のstate B cell modulatorになる。 |
| non-blocking Fc-silent anti-FCRL4 | 内因性IgA/J-chain/FCRL4調節を邪魔せず、FCRL4+細胞を選択 | 安全なanchor benchmark。 |
| blocking anti-FCRL4 | FCRL4-IgA/J-chain相互作用を遮断 | 内因性抑制を外すリスクがあり、慎重に扱う。 |

判断は単純である。抗FCRL4単独がBsAbと同等または上回るなら、より単純な抗FCRL4単独へpivotする。BsAbを残す条件は、anti-FCRL4単独、anti-CD22単独、anti-FCRL4 + anti-CD22併用を明確に上回ることである。

## 腺外症状への影響予測
FcRL4+ B細胞を標的にした場合、最も期待できるのは唾液腺/粘膜B細胞ニッチに近い病態である。関節痛、神経障害、皮膚、腎、肺などの腺外症状は、FcRL4+ B細胞が直接その組織で病態を作っている証拠、またはRF/cryoglobulin/低C4/CXCL13などのB-cell-high systemic axisとの連動が必要である。

| 症状/病態 | 期待値 | 判断 |
|---|---|---|
| 唾液腺腫脹、口腔乾燥、MALT lymphoma risk | 高 | FcRL4+腺内B細胞との結びつきが最も強い。 |
| 眼/涙腺、他粘膜症状 | 中 | 粘膜B細胞stateとして妥当だが、組織ごとにFcRL4確認が必要。 |
| 関節痛/関節炎 | 中 | pSSでの直接証拠は弱い。RA滑膜FcRL4+ B細胞の強い根拠を参考に、真の滑膜炎がある群だけ狙う。 |
| 神経障害 | 低-中 | FcRL4直接証拠は不明。cryoglobulinemic/vasculitic neuropathyならB細胞軸で可能性。 |
| 皮膚紫斑/血管炎、腎病変 | 低-中 | cryoglobulin、RF、低C4と連動する場合のみ期待。 |
| 疲労、brain fog、慢性疼痛 | 低 | 多因子性でprimary endpointには不向き。 |

腺外症状を狙う場合は、乾燥症状だけでなく、CXCL13、BAFF、IL-21、RF、cryoglobulin、C4、高IgG、形質芽細胞、腺腫脹、MALT riskを用いて患者選択する。

## 他疾患展開
FcRL4起点で最も展開可能性が高いのは関節リウマチである。RA滑膜ではFcRL4+ B細胞がRANKL/TNF高発現の炎症性B細胞として報告され、FcRL4+ B細胞由来抗体がシトルリン化自己抗原に反応する報告もある。

| 優先 | 疾患 | 理由 | 次の確認 |
|---:|---|---|---|
| 1 | 関節リウマチ、滑膜B細胞高値/難治性RA | FcRL4+滑膜B細胞、RANKL/TNF、ACPA関連の根拠あり。 | 滑膜FcRL4+CD22+ B細胞でBsAbがBCR/TLR/RANKL/TNFを抑えるか。 |
| 2 | Sjögren関連MALT lymphoma/前リンパ腫ニッチ | FcRL4/IRTA1とMALT/LELの関係が強い。 | 自己免疫薬としてはFc-silent、腫瘍寄りならADC/Fc-enhancedを別検討。 |
| 3 | IgA/粘膜B細胞関連疾患 | FcRL4はsystemic IgA receptor。 | IgA immune complex疾患でFcRL4+病変B細胞がいるか。 |
| 4 | SLE/LN、Graves/MGなど | 2026年FCRL総説では候補に入るが直接性は弱い。 | 血液/組織single-cellでFCRL4+CD22+ B細胞を確認してから。 |
| 低 | ANCA、膜性腎症、水疱症、強皮症、IBD | 現時点で直接証拠が乏しい。 | 優先しない。 |

## epratuzumab失敗との合致
| epratuzumabから見える失敗仮説 | FCRL4 x CD22の返答 | 残るリスク |
|---|---|---|
| 広いSLEで組織state選択なし | FCRL4+ gland B-cell-high Sjögrenに絞る | FCRL4がbystanderの可能性 |
| CD22単独では疾患文脈が弱い | FCRL4 armでCD22 engagementを組織B細胞へ局在 | anti-CD22単独を超える必要 |
| CD22単独の抑制入力が弱い | FCRL4側のBCR抑制入力も同時に使う | FCRL4 agonismが本当に抑制的か要検証 |
| placebo/標準治療で臨床差が薄まる | 最初は唾液腺ex vivo機能でPoC | 臨床endpointは後で難しい |
| Fc依存trogocytosisが作用に関与 | まずFc-silentで真のCD22/SHP-1抑制を検証し、並行してFc-active/Fc-tunedでFCRL4-gated trogocytosisを評価 | Fc活性が必要ならFc-silent tissue-silencer仮説は弱まり、Fc-active tissue modulatorへpivot |

## Fc依存性trogocytosisの意味
Fc依存性trogocytosisとは、標的細胞に結合した抗体のFc部分がFcγR陽性細胞に認識され、そのFcγR陽性細胞が標的細胞膜の一部を取り込む現象である。epratuzumabでは、B細胞上のCD22だけでなく、CD19、CD21、CD79bなどBCR co-receptor関連分子も表面から低下することが報告されている。これはADCCのような細胞殺傷とは異なり、B細胞表面分子の再編成によってB細胞反応性を下げる可能性がある。

本提案でFc-silentを主案に置く理由は、trogocytosisを否定しているからではない。まずFCRL4 x CD22の空間薬理だけでCD22/SHP-1抑制が成立するかを検証し、慢性Sjögrenで望ましくない非選択的FcγR依存作用を避けるためである。Fc-activeはbackupではなく、初期比較に入れる重要な分岐である。

## 新規性監査
| 項目 | 判定 |
|---|---|
| 標的新規性 | FCRL4を自己免疫組織住所として使う点は新規。公開臨床上のFcRL4直接競合は見当たらない。CD22単独は既知。 |
| MoA新規性 | FCRL4+細胞上のcis CD22 silencingに加え、FCRL4側のBCR抑制も同時に使えれば非常に新規。 |
| 疾患ポジション | gland B-cell-high Sjögrenへのsegment shift。 |
| モダリティ新規性 | BsAbは薬理の中心で必須。 |
| バイオマーカー | FCRL4/CXCL13組織signatureに結びつく。 |
| 競合成功時 | BAFF/CD40L成功後も組織B細胞高値non-responderで残る。FCRL5 x CD3が成功しても、depletionではなくtissue silencingとして残す。 |
| 競合失敗時 | 汎B細胞除去失敗時も組織state標的として残る。 |

## コピーではない理由
CD22は疾患の住所ではなくブレーキである。FCRL4は住所であり、さらに第二のブレーキ候補でもある。したがって、epratuzumabの単純な焼き直しではなく、病変組織B細胞に限定したdual-brake BsAbである。

## リスク
- FCRL4がdriverではなく疲弊/慢性炎症markerかもしれない。
- FCRL4 agonismが抗体で再現できない可能性。
- FCRL4 ligationでTLR7/9、CD40、IL-21反応やIg産生が増える可能性。
- 腺外症状がFcRL4+腺内B細胞と連動せず、乾燥/腺症状以外に効かない可能性。
- FCRL5 x CD3など近縁FCRL family競合が自己免疫で先行し、FCRL family標的の社内優先順位を奪う可能性。
- CD22 agonismが弱い可能性。
- epratuzumab様のFc依存trogocytosisが必要ならFc-silent仮説は弱まり、Fc-active/Fc-tuned設計へpivotが必要。
- Fc-active化で非選択的trogocytosis、局所炎症、正常粘膜B細胞への作用が出る可能性。
- 唾液腺への薬剤到達とサンプル取得が難しい。
- 正常粘膜記憶B細胞への影響。

## 中止基準
- FCRL4+ B細胞が対象Sjögren群に少ない。
- FCRL4+細胞が自己抗体、抗原提示、Tfh相互作用、活動性と無関係。
- 唾液腺FcRL4+ B細胞量がESSDAI domain、CXCL13、RF、cryoglobulin、低C4、高IgGと相関しない。
- anti-FCRL4単独またはFCRL4 x CD22 BsAbでFCRL4側のSHP recruitmentやBCR抑制が出ない。
- FCRL4 ligationでTLR7/9、CD40、IL-21、Ig産生、CD86/HLA-DRが増える。
- anti-FCRL4単独がBsAbと同等または上回る場合は、BsAb主案から抗FCRL4単独主案へpivotする。
- BsAbがanti-CD22単独を上回らない。
- BsAbがanti-FCRL4単独を上回らない。
- BsAbがanti-FCRL4 + anti-CD22併用を上回らない。
- Fc-activeでのみ効く場合に、trogocytosisがFCRL4陽性病変B細胞に限定されない。
- Fc-active化で広範なB細胞表面分子stripping、炎症、または正常粘膜B細胞毒性が出る。
- 汎B細胞除去が必要になる。

## 最初の実験
1. 唾液腺spatial/IHCでFCRL4、CD22、CXCL13、Tfh、clonalityを確認。
2. fresh gland B-cell flowとBCR sequencing。
3. FCRL4 x CD22 geometry screenでCD22側SHP-1 recruitment、FCRL4側SHP-1/SHP-2 recruitment、Ca抑制を確認。
4. 自己唾液腺B-T co-cultureで抗原提示/Ig産生抑制。
5. anti-FCRL4 Fc-silent agonist、anti-FCRL4 neutral/non-blocking、anti-FCRL4 Fc-active/Fc-tuned、anti-CD22単独、2剤併用、Fc-silent BsAb、Fc-active/Fc-tuned BsAbを同一系で比較。
6. BCR readoutとしてpSyk、pBLNK、pPLCγ2、Ca flux、pERK、pAKTを測る。TLR7/9、CD40、IL-21刺激下の逆活性化も見る。
7. 唾液腺FcRL4+ B細胞量とESSDAI domain、CXCL13、RF、cryoglobulin、C4、高IgGを相関させる。
8. 関節症状があるpSSでは滑膜炎画像陽性群に絞り、可能なら滑膜液/滑膜生検でFcRL4+CD22+ B細胞を確認。
9. 神経障害はcryoglobulinemic/vasculitic phenotypeと非vasculitic phenotypeを分ける。
10. Fc-active条件では、CD22/CD19/CD21/CD79b低下、FcγR陽性細胞依存性、FCRL4陽性細胞選択性、正常粘膜B細胞への広がりを測る。

## 競合が成功/失敗した場合
- BAFF/CD40Lが成功: tissue B-cell-highまたはリンパ腫リスクsegmentで残る必要。
- BAFF/CD40Lが失敗: 組織B細胞state標的として価値が上がる。
- FCRL5 x CD3がSLE/LNで成功: FCRL family druggabilityの外部検証になる一方、Proposal 2はSjögren腺内FcRL4+ B細胞のtissue silencerとして差別化が必須。
- epratuzumab失敗をCD22全否定と読む場合: FCRL4-gated superiorityが必須。

## 主要根拠
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
- Cevostamab SLE/LN Phase Ib: https://clinicaltrials.gov/study/NCT07629583
- FcRH5/CD3 bispecific epitope biology: https://pubmed.ncbi.nlm.nih.gov/28262555/
