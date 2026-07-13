# 自己免疫B細胞抗体シーズ探索

作成日: 2026-07-08

## 調査範囲

このフォルダは、過去の自己免疫領域リサーチと混ざらないように独立して作成した。対象は、ステロイド、従来型免疫抑制剤、IVIG、血漿交換、反復B細胞除去、FcRn阻害、補体阻害などにまだ依存している自己免疫疾患・自己免疫隣接疾患である。

今回の中心テーマはB細胞である。具体的には、病的BCRクローン、組織常在記憶B細胞、形質芽細胞/形質細胞、Tfh-B細胞ニッチ、自己抗体産生、B細胞抑制チェックポイントを重視した。

## 革新性フィルター

全候補で次を問い続けた。

```text
これは本当に新しい抗体医薬シーズか。
単なるCD19/CD20/BAFF/CD40L/FcRnの言い換えではないか。
```

汎B細胞除去、BAFF/APRIL阻害、CD40L阻害、FcRn阻害をそのまま繰り返す案は、抗体設計が新しい薬理を作らない限り低く評価した。

## 重要な外部シグナル

- 2026年のIGHV4-34標的CAR-T報告: 疾患関連BCR frameworkを狙うことで、全B細胞ではなく病的B細胞を選択的に狙える可能性が示された。
- 2024-2026年の自己免疫CAR-T経験: 重症SLEなどで深いB細胞resetがdrug-free remissionを生みうる一方、リンパ球除去、感染、CRS/ICANS、費用、製造が障壁になる。
- CD19/FcRn領域の承認・開発: inebilizumab、efgartigimod、nipocalimabなどがB細胞/IgG biologyを強く検証した一方、広い標的は混雑している。
- 失敗学習: SLE/LNでのrituximab、SLEでのepratuzumab、BAFF/APRIL系のtabalumab/atacicept/blisibimod、初期anti-CD40Lの血栓リスクを地雷として扱った。

## 成果物

- `disease_landscape/`: 10疾患領域の調査メモ。
- `analysis/disease_target_matrix.tsv`: 疾患と標的の対応表。
- `targets/target_shortlist.tsv`: 20標的の候補表。
- `targets/target_cards/`: 有望5標的の標的カード。
- `antibodies/design_options/`: 抗体設計案。
- `evidence/clinical_trials/`: 臨床失敗・既存薬限界の調査メモ。
- `outputs/`: 最終3提案とスライド構成案。
- `for_me/`: 自分用に基礎から腹落ちするための詳細メモ。
