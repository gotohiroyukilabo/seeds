# エグゼクティブサマリー

## 調査範囲
自己免疫疾患の中でも、ステロイド、従来型免疫抑制剤、IVIG、血漿交換、反復B細胞除去、FcRn/補体阻害などに依存する患者集団を対象にした。成果物はすべて `autoimmune_bcell_antibody_20260708/` に分離した。

## 主結論
新規B細胞抗体シーズは、CD19/CD20/BAFF/CD40L/FcRnの後追いでは弱い。革新的に見える上位テーマは次の3つである。

1. 病的BCR frameworkそのものを狙う。
2. 組織常在/病変組織B細胞stateを狙う。
3. B細胞抑制チェックポイントを文脈依存的に作動させる。

## 探索した疾患領域
SLE/ループス腎炎、Sjögren病、IgG4関連疾患、ANCA関連血管炎、自己免疫性水疱症、重症筋無力症、自己免疫性血球減少症、原発性膜性腎症、自己免疫性脳炎、B細胞活性化型全身性強皮症。

## 最終3候補
| 順位 | シーズ | 初期適応 | 中核モダリティ | 採択理由 |
|---:|---|---|---|---|
| 1 | IGHV4-34病的BCR選択的engager | 9G4/IGHV4-34高値重症SLE/LN | maskedまたは低親和性IGHV4-34 x CD3/CD16a BsAb、ADC backup | 疾患クローンを狙う発想が最も新しい。 |
| 2 | FCRL4 x CD22組織B細胞サイレンサー | 腺内B細胞高値Sjögren病 | 抗FCRL4単独またはFc-silent FCRL4 x CD22 inhibitory BsAb | epratuzumab失敗を踏まえ、CD22を組織B細胞stateへretargetし、FCRL4も第二のBCR brake候補として使う。FcRL4直撃の公開臨床競合は見当たらない一方、FCRL5 x CD3/cevostamabがSLE/LNへ進むため、tissue silencerとして差別化する。抗FCRL4単独が同等なら単独案へpivotする。腺外症状はB-cell-high systemic axis連動例に限定して狙い、RA滑膜B細胞高値への横展開余地がある。 |
| 3 | CD72チェックポイントagonist | 核酸自己抗原反応型SLE/LN | Fc-silent agonist、context-gated BsAb backup | 非除去型tolerance restorationで新規性が高い。 |

## バックアップ候補
- CXCL13 pH-recycling抗体: B細胞ニッチ仮説とバイオマーカー性が強い。
- CD38 x BCMA gated plasma-cell reset: 強力だが安全性と競合が重い。

## ダウングレードした領域
CD19、CD20、BAFF/APRIL、CD40L、FcRnはbiologyとしては強いが混雑している。新規seedの中心ではなく比較対照として扱う。

## 初期実験の共通方針
1. ヒト患者サンプルで標的陽性患者割合を確認。
2. ex vivoで疾患機能が動くか確認。
3. cytokine、protective humoral immunity、安全域を早期に確認。
4. 既存MoAや単独抗体/2剤併用と直接比較。
5. 汎B細胞除去に崩れる候補は早く止める。
