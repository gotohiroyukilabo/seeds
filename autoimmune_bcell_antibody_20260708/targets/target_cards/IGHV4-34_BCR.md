# 標的カード: IGHV4-34陽性病的BCR

## 要約
- 標的: IGHV4-34陽性BCR framework epitope。
- UniProt ID: 該当なし。再構成免疫グロブリン可変領域であり、単一の標準タンパク質ではない。
- 想定疾患: 9G4/IGHV4-34高値の重症SLE/ループス腎炎。
- 推奨モダリティ: maskedまたは低親和性IGHV4-34 x CD3/CD16a BsAb、Fc強化抗体、ADC。
- 推奨度: 高。ただしバイオマーカー選択が必須。
- 仮説: 全B細胞ではなく、自己免疫に関わるBCR frameworkを持つB細胞を選択的にresetする。

## なぜ重要か
2026年のIGHV4-34 CAR-T報告により、CD19/CD20のような汎B細胞マーカーではなく、病的BCR frameworkを標的にする発想が現実味を持った。抗体薬でこれを再現できれば、CAR-Tより実装しやすいprecision B-cell resetになる。

## スコア
| 評価軸 | 点数 | 理由 |
|---|---:|---|
| 未充足ニーズ | 5 | 重症SLE/LNは依然として免疫抑制依存。 |
| 標的biology | 4 | IGHV4-34/9G4とSLE自己反応性の関連は強いが、患者割合の確認が必要。 |
| 抗体適性 | 3 | BCRは表面標的だが、血中Igシンクやepitope heterogeneityが難しい。 |
| 差別化 | 5 | 汎B細胞除去ではなく病的クローン選択。 |
| 安全域 | 3 | CD3/CD16a/ADCはいずれも安全域確認が必要。 |
| バイオマーカー | 5 | 9G4抗体、flow、BCR sequencingで患者選択可能。 |
| 開発容易性 | 3 | 抗idiotype特異性と製造性が課題。 |

## 既存ランドスケープ
CD19 CAR-T、CD19 depletion、FcRn、BAFF、CD40Lは広いB細胞/IgG biologyを狙う。CART4-34は細胞治療であり、同じ標的思想を抗体薬に落とす余地がある。承認済み抗体薬でIGHV4-34 BCRを選択的に狙うものは確認できていない。

## 抗体である必然性
生きたB細胞表面のBCR frameworkを認識し、必要ならT細胞/NK細胞/payloadを同じ細胞へ誘導する必要がある。これは小分子では作りにくい空間薬理である。

## 新規性監査
| 項目 | 判定 |
|---|---|
| 標的新規性 | 新規。承認自己免疫抗体とは異なる。 |
| MoA新規性 | 病的BCR選択的除去/抑制なら新規。汎B細胞除去化すれば失敗。 |
| 疾患ポジション | 9G4/IGHV4-34高値SLE/LNへのsegment shift。 |
| モダリティ新規性 | BsAb/ADCは薬理を作る場合のみ必須。 |
| バイオマーカー | 標的とmechanistically tied。 |
| 競合成功時の生存性 | CD19 CAR-Tが高価/重い限り残る。 |
| 競合失敗時の生存性 | 汎CD19毒性が問題ならむしろ残る。 |

## コピーではない理由
CD19/CD20/BAFF/FcRnではなく、自己反応性BCR frameworkそのものを標的にする。疾患を「B細胞全体の異常」ではなく「病的BCRクローンの異常」として捉える。

## リスク
- 対象患者が少なすぎる可能性。
- 血中Ig/自己抗体が抗原シンクになる可能性。
- CD3 BsAbではCRS/ICANSが問題。
- IGHV4-34陰性の病的クローンが残る可能性。
- 正常IGHV4-34 B細胞の喪失。

## 中止基準
- 重症SLE/LNで明確なIGHV4-34/9G4 biologyを持つ患者が15-20%未満。
- 血清Igにより結合/薬効が失われる。
- IGHV4-34陰性B細胞のbystander killingが強い。
- 患者B細胞培養で自己抗体産生が下がらない。
- CD19 CAR-T/TCEと比べて安全性・実用性で勝てない。

## 最初の実験
1. 重症SLE/LNサンプルでIGHV4-34+ B細胞と9G4抗体を定量。
2. 血清存在下でのbinding/competition評価。
3. IGHV4-34 x CD3、x CD16a、Fc強化、ADCの選択性比較。
4. 全血cytokine release。
5. ex vivo自己抗体産生抑制。

## 競合が成功/失敗した場合
- CD19 CAR-Tが成功した場合: 外来投与、低負荷、低コスト、患者選択性が必要。
- CD19 CAR-Tが毒性/実装で失敗した場合: 抗体薬版precision resetとして価値が上がる。

## 主要根拠
- Cohen et al., Science Translational Medicine, 2026. DOI: 10.1126/scitranslmed.adr9382
- Nature news, 2026-02-04: https://www.nature.com/articles/d41586-026-00358-6
