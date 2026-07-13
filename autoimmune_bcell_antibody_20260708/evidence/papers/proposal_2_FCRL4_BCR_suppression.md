# Proposal 2 追加調査: FCRL4のBCR抑制とCD22共刺激

作成日: 2026-07-12

対象は `FCRL4 x CD22 組織B細胞サイレンサー` である。このメモは、FCRL4を単なる病変B細胞の住所として使うだけでなく、BCR抑制性の免疫調節分子として使えるかを整理する。

## 結論
FCRL4は、提案2では「住所」だけでなく「第二のBCRブレーキ候補」として扱うべきである。FCRL4/FcRH4陽性B細胞は組織局在性の記憶B細胞として記載され、BCR応答が低い集団として扱われてきた。したがって、CD22とFCRL4を同じFCRL4陽性病変B細胞上で共抑制刺激できれば、提案2は単なるCD22 retargetingではなく、dual inhibitory co-agonismになる。

ただし、FCRL4を抗体で刺激すれば必ずBCR抑制が出る、と言い切るのは危険である。FCRL4陽性組織B細胞は粘膜記憶B細胞/TLR応答とも関係する可能性があり、FCRL4 ligationでTLR7/9、CD40、IL-21、Ig産生、抗原提示が増える場合はNo-Goに近い。

追加で重要なのは、抗FCRL4単独抗体が独立候補になる点である。CD22 agonismが弱くても、FCRL4+ disease-state B cellそのものを選択的にmodulateできれば、FCRL4 x CD22 BsAbより単純な候補として成立する。詳細は [proposal_2_anti_FCRL4_monotherapy_comparator.md](proposal_2_anti_FCRL4_monotherapy_comparator.md) にまとめた。

## 根拠文献
| 文献 | リンク | この提案での読み方 |
|---|---|---|
| Ehrhardt et al. `Expression of the immunoregulatory molecule FcRH4 defines a distinctive tissue-based population of memory B cells.` J Exp Med, 2005 | [PubMed](https://pubmed.ncbi.nlm.nih.gov/16157685/) / [DOI](https://doi.org/10.1084/jem.20050879) | FCRL4/FcRH4を組織局在性の記憶B細胞stateとして見る中核根拠。FCRL4を単なる表面マーカーではなく免疫調節分子として扱う。 |
| Haacke et al. `FcRL4+ B-cells in salivary glands of primary Sjögren's syndrome patients.` Journal of Autoimmunity, 2017 | [PubMed](https://pubmed.ncbi.nlm.nih.gov/28390747/) / [DOI](https://doi.org/10.1016/j.jaut.2017.03.012) | FCRL4陽性B細胞がSjögren唾液腺病変に存在することの中核根拠。 |
| `Antibodies Encoded by FCRL4-Bearing Memory B Cells Preferentially Recognize Commensal Microbial Antigens.` Journal of Immunology, 2018 | [PubMed](https://pubmed.ncbi.nlm.nih.gov/29703863/) / [DOI](https://doi.org/10.4049/jimmunol.1701549) | FCRL4-bearing memory B cellが粘膜・常在抗原文脈に寄る可能性。安全性では正常粘膜B細胞への影響を見る。 |
| Müller et al. `CD22: A Regulator of Innate and Adaptive B Cell Responses and Autoimmunity.` Frontiers in Immunology, 2018 | [PubMed](https://pubmed.ncbi.nlm.nih.gov/30323814/) / [DOI](https://doi.org/10.3389/fimmu.2018.02235) | CD22をBCR/TLR応答の抑制受容体として位置付ける。 |
| Walker and Smith. `CD22: an inhibitory enigma.` Immunology, 2008 | [PubMed](https://pubmed.ncbi.nlm.nih.gov/18067554/) / [DOI](https://doi.org/10.1111/j.1365-2567.2007.02752.x) | CD22 agonismが単純ではなく、cis ligand、BCR近接、epitope/geometry依存であることの注意点。 |

## FCRL4をどう解釈するか
| 見方 | 内容 | 提案2への影響 |
|---|---|---|
| 住所 | FCRL4陽性の唾液腺病変B細胞を選ぶ | 最低限の価値。CD22 retargetingとして成立。 |
| 第二のブレーキ | FCRL4自体がBCR応答を弱める | BsAbの革新性が上がる。dual brakeとして説明できる。 |
| 慢性刺激marker | BCR/TLR刺激を受けた結果として上がるだけ | causalityが弱い。biomarkerとしては使えても標的妥当性は下がる。 |
| 粘膜記憶B細胞marker | 常在菌/粘膜抗原応答と関係する | 正常粘膜免疫への影響が安全性リスクになる。 |

## FCRL4のBCR抑制仮説
仮説は次である。

```text
FCRL4+CD22+ 病変B細胞
  ↓
FCRL4 x CD22 BsAbが同じ細胞上で結合
  ↓
CD22側: SHP-1 recruitment
FCRL4側: SHP-1/SHP-2様の抑制入力
  ↓
BCR近位シグナル低下
  ↓
pSyk / pBLNK / pPLCγ2 / Ca flux / pERK / pAKT低下
  ↓
抗原提示、Tfh help応答、Ig産生が下がる
```

この仮説が正しければ、FCRL4は単なる住所ではない。病変B細胞を選ぶ住所であり、その病変B細胞を沈静化するブレーキでもある。

## CD22とFCRL4を共刺激する意義
「共刺激」という言葉は、免疫学では活性化costimulationを連想させるため注意が必要である。ここで狙うのは、CD22とFCRL4を同時に活性化してB細胞を活性化することではない。狙いは共抑制刺激、つまりdual inhibitory co-agonismである。

| ポイント | 期待 |
|---|---|
| 同じB細胞でcis co-ligationする | 2剤併用よりもBCR microcluster近傍に抑制入力を置ける。 |
| CD22とFCRL4の抑制入力を重ねる | CD22単独では弱い可能性を補う。 |
| FCRL4陽性細胞に限定する | epratuzumabのような広いCD22 modulationと差別化する。 |
| Fc-silentで評価する | Fc依存性trogocytosisを混ぜず、純粋な抑制受容体薬理を見る。 |

## 成功シナリオ
| シナリオ | 意味 | 判断 |
|---|---|---|
| FCRL4 x CD22 BsAbがanti-CD22単独、anti-FCRL4単独、2剤併用を上回る | BsAb geometryとdual brakeが効いている | 強いGo |
| BsAbはanti-CD22単独を上回るが2剤併用と同等 | retargeting効果はあるが空間薬理が弱い | geometry再設計 |
| anti-FCRL4単独でもBCR抑制が出る | FCRL4 agonismが有効 | FCRL4 armのepitope最適化 |
| FCRL4 agonismは弱いがBsAbでだけ効く | CD22との近接が重要 | BsAb継続 |

## 危険シナリオ
| シナリオ | 意味 | 判断 |
|---|---|---|
| FCRL4 ligationでTLR7/9、CD40、IL-21反応が増える | 組織B細胞を沈静化せず、活性化側へ倒す | 原則No-Go |
| FCRL4 agonist epitopeがIg産生、CD86、HLA-DRを上げる | 抗原提示/Tfh helpを強める | agonist epitopeはNo-Go |
| FCRL4陰性B細胞にも作用する | FCRL4 gateが効いていない | affinity/valency再設計 |
| BCR抑制がCD22単独と同じ | FCRL4を入れる意味が弱い | No-Goまたは別標的へpivot |
| FCRL4 bindingでinternalizationのみ | signaling agonismではなく表面除去だけ | ADC/depletion設計以外では弱い |

## 初期評価系
| 評価 | 具体的readout |
|---|---|
| FCRL4発現と局在 | 唾液腺spatial/IHC、flow、FCRL4+CD22+ B細胞頻度、上皮/Tfh/CXCL13近接 |
| BCR近位シグナル | pSyk、pBLNK、pPLCγ2、Ca flux、pERK、pAKT |
| 抑制受容体入力 | CD22 phosphorylation、CD22/SHP-1、FCRL4/SHP-1/SHP-2 recruitment |
| 機能 | Ig産生、自己抗体関連Ig、抗原提示、CD86、HLA-DR、B-T co-culture |
| 逆活性化 | CpG/TLR9、R848/TLR7、CD40L、IL-21条件でのNF-κB、CD86、Ig産生 |
| BsAb必然性 | anti-CD22、anti-FCRL4、2剤併用、Fc-silent BsAb、Fc-active/Fc-tuned BsAbの同一比較 |

## 提案文への反映
短く言うなら次である。

```text
FCRL4は病変B細胞の住所であるだけでなく、BCR抑制性の第二ブレーキ候補である。
FCRL4 x CD22 BsAbは、Sjögren唾液腺のFCRL4+ B細胞にCD22 brakeを届けるだけでなく、
FCRL4 brakeも同時に使うdual inhibitory co-agonistとして設計できる。
```

ただし、プレゼンでは必ず次の但し書きを添える。

```text
FCRL4 agonismが薬理的に抑制を出すか、逆にTLR/Tfh反応を増やすかは未確定であり、
fresh gland B cell assayで最初に切るべきGo/No-Goである。
```
