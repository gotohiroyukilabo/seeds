# 抗体設計案: IGHV4-34陽性BCR

## 設計仮説
病的BCR選択性を守れない設計は不採用。汎B細胞除去に見えた時点で価値は落ちる。

| 設計 | 作用機序 | 期待利点 | 差別化 | 安全性リスク | 初期評価系 | 中止基準 | 優先度 |
|---|---|---|---|---|---|---|---|
| blocking抗体 | BCR-自己抗原結合を妨げる | 非除去型で安全寄り | CD19/CD20とは異なるが薬効は弱い可能性 | 免疫複合体、BCR crosslinking | serum competition、BCR signaling | BCR活性化抑制なし | 中-低 |
| agonist抗体 | anergy様シグナルを誘導 | 病的クローンを殺さず沈静化 | tolerance誘導なら新規 | 逆活性化 | anergy marker、Ca flux | 活性化が出る | 中 |
| Fc-silent抗体 | Fc effectorを消してBCR binding | 機序確認と安全性評価 | proof-of-biology用 | 効力不足 | FcR panel | 機能効果なし | 中 |
| Fc強化抗体 | ADCC/ADCPでIGHV4-34+ B細胞除去 | off-the-shelf精密depletion | CD19/CD20より選択的 | 正常IGHV4-34喪失 | ADCC/ADCP選択性 | 陰性B細胞との選択性不足 | 中-高 |
| BsAb | IGHV4-34 x CD3/CD16aでeffector recruitment | CAR-T様選択性を抗体化 | 最も革新的 | CRS/ICANS、bystander killing | autologous killing、cytokine | サイトカイン/巻き込み毒性 | 高 |
| ADC | BCR internalizationを利用してpayload送達 | T細胞サイトカインを避ける | 有限clone reset | payload毒性 | internalization、bystander | internalization不足 | 中 |
| masked抗体 | 病変環境でeffector armを解放 | 全身毒性を下げる | 安全域拡張 | 過剰/不十分なunmasking | protease panel | 疾患選択的unmaskなし | 中-高 |
| pH依存recycling抗体 | 血中で結合、endosomeで解離 | Ig sink軽減 | 補助的工学 | 免疫複合体 | pH binding/PK model | PK/PD改善なし | 中 |

## 推奨する初期方針
最初は標的biologyを検証できる最小フォーマットと、差別化を作る本命フォーマットを並行して評価する。流行技術を足すのではなく、単独抗体や2剤併用を超える空間薬理が出るかを最初に確認する。
