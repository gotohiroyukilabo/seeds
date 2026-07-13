# 提案3 詳細メモ: CD72 B細胞チェックポイントagonist

作成日: 2026-07-08

## 0. このレポートの目的
`outputs/seed_proposal_3.md` の内容を、自分で説明できるレベルまで噛み砕くためのメモである。

中心の問いは、なぜB細胞を殺さず抑えるのか、CD72 agonistは何が難しいのか、どの実験で早期判断できるかである。

## 1. B細胞にはアクセルとブレーキがある
B細胞はBCRで抗原を認識すると活性化する。一方で、FcGR2B、CD22、CD72などの抑制系が過剰反応を抑える。

自己免疫では、自己抗原に対するアクセルが強すぎる、またはブレーキが十分に効かない。

## 2. CD72とは何か
CD72はB細胞表面にある抑制性受容体で、UniProt IDはP21854である。細胞内に抑制性motifを持ち、SHP-1などの抑制系を動かす可能性がある。

## 3. なぜSLE/LNで面白いのか
SLEでは核酸/核タンパク自己抗原をBCRで取り込み、endosome内TLR7/TLR9が刺激されることで強いB細胞活性化が起きる。

```text
核酸自己抗原 → BCR取り込み → TLR7/TLR9刺激 → 形質芽細胞化 → 自己抗体
```

CD72がこの反応にブレーキをかけられるなら、BAFF/CD20/FcRnとは異なる介入になる。

## 4. なぜB細胞を殺さないのか
B細胞除去は強いが、感染、低Ig、ワクチン応答低下、再増殖後再燃がある。CD72 agonistは、B細胞を消すのではなく、自己反応性B細胞が反応しにくい状態を作る。

## 5. agonist抗体の難しさ
agonist抗体は標的を止めるのではなく働かせる。epitope、valency、Fc、細胞状態で作用が大きく変わる。CD72では逆活性化を避ける必要がある。

## 6. 抗体設計
| 設計 | 位置づけ |
|---|---|
| Fc-silent CD72 agonist | 主案。FcR依存の不確実な架橋を避ける。 |
| engineered multivalent agonist | 2価で弱い場合のbackup。 |
| CD72 x IGHV4-34 BsAb | 病的BCR陽性B細胞に限定する。 |
| CD72 x FCRL4 BsAb | 組織B細胞に限定する。 |
| Fc強化/ADC | 原則避ける。提案の意味が消える。 |

## 7. 既存薬との差
rituximab/CD20やinebilizumab/CD19はB細胞を減らす。belimumabは生存因子を抑える。FcRn阻害はIgGを減らす。CD72はB細胞活性化の閾値を上げる。

## 8. 患者選択
anti-dsDNA高値、低補体、IFN signature、形質芽細胞高値、CD72発現/リン酸化、ex vivo BCR/TLR応答を使う。

## 9. 主なリスク
human CD72 biologyが弱い、正しいagonist geometryが作れない、逆に活性化する、正常B細胞防御を落とす、biomarkerがない。

## 10. 最初にやるべき検証
SLE患者B細胞でCD72発現、SHP-1 recruitment、BCR/TLR7/TLR9抑制、形質芽細胞分化抑制、自己抗体産生低下、vaccine recall保持を確認する。

## 11. 継続/中止基準
継続条件: human SLE B細胞で抑制シグナルが入り、自己抗体方向が下がり、防御的recall応答が保たれる。

中止条件: 抑制シグナルなし、逆活性化、広範B細胞抑制、CD22/FCGR2B benchmarkに劣る。

## 12. 最終コメント
CD72は高リスクだが、当たれば非常に新しい。臨床に急がず、ヒトSLE B細胞で早く判断する候補である。
