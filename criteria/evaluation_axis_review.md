# Evaluation Axis Review

## Summary

これまでの評価軸は、抗体医薬シーズ探索としては妥当だったが、「既存薬や開発品と違う革新的なものを探す」という今回の目的には不十分である。

特に問題だったのは、以下である。

- target biologyやantibody tractabilityを重く見すぎると、臨床開発が進んだ既存標的を高く評価してしまう。
- differentiationを「既存薬より少し良い」程度で許すと、me-too / me-better候補が残ってしまう。
- developabilityを重く見すぎると、真に新しいが難しい候補を早く落としてしまう。
- 競合がいることを「標的妥当性」として評価すると、先行品の後追いになる。

したがって、評価軸を「実現可能性中心」から「革新性・非模倣性中心」に変更する。

## New Priority

新しい優先順位は以下。

| 優先度 | 評価軸 | 方針 |
|---:|---|---|
| 1 | Non-mimicry / 非模倣性 | 既存薬・開発品の後追いを排除する |
| 2 | Conceptual novelty / 概念的新規性 | 疾患の見方を変える仮説を重視する |
| 3 | Mechanistic originality / 機序の独自性 | 抗体でしか作れない新しい薬理を重視する |
| 4 | Competitive whitespace | 競合のいない、または競合と根本的に違う空白を探す |
| 5 | Antibody necessity | 抗体である必然性が表層的でないか見る |
| 6 | Human biology plausibility | 革新的仮説がヒト病態に接続しているか見る |
| 7 | Early falsifiability | 早期に殺せる検証系があるか見る |
| 8 | Unmet need | 必要だが、未充足だけでは不十分 |
| 9 | Safety logic | 主要リスクを早期評価できるか見る |
| 10 | Developability | 重要だが最優先ではない |

## Why Developability Is Downweighted

開発可能性は重要である。しかし、探索初期に開発可能性を重くしすぎると、以下のような候補ばかり残る。

- 既に誰かが臨床開発している標的。
- 通常IgGでblockingするだけの標的。
- 既存MoAの適応拡大。
- 競合薬の少し違う版。

このプロジェクトでは、そうした候補は目的に合わない。

革新的候補は、最初はdevelopabilityが悪く見えることがある。BsAb、masked antibody、conditional agonist、pH-dependent antibody、cell-state selective ADC、tissue-activated antibodyなどは、通常IgGより難しい。しかし、それが新しい薬理を作るなら初期探索で残す価値がある。

ただし、developabilityを無視するわけではない。以下はNo-Goになりうる。

- 正常組織毒性が避けられない。
- 抗原発現が標的疾患に限られず安全域がない。
- 分子設計が薬理を壊す。
- 初期評価系で安全性懸念を確認できない。
- CMCが仮説検証用分子の作製すら妨げる。

## How To Use Existing Drugs And Pipeline Assets

既存薬・開発品は、真似るためではなく、避けるために調べる。

| 使い方 | 良い使い方 | 悪い使い方 |
|---|---|---|
| Target validation | 先行品がどこまで占有しているか確認する | 先行品があるから同じ標的を推す |
| Clinical history | 失敗理由、endpoint、患者選択を学ぶ | 同じ患者・同じMoAで再提案する |
| Safety | class riskを把握する | 少しFcを変えれば差別化できると安易に言う |
| Biomarker | 競合が使えるbiomarkerか確認する | 競合と同じbiomarkerを独自性として扱う |
| Modality | 既存formatの限界を知る | 流行技術を後付けする |

## Required Questions For Every Candidate

候補ごとに必ず以下を問う。

1. 最も近い既存薬・開発品は何か。
2. それと標的は同じか。
3. それとMoAは同じか。
4. それと疾患・患者セグメントは同じか。
5. それと抗体設計思想は同じか。
6. 既存品が成功したら、この候補はまだ必要か。
7. 既存品が失敗したら、この候補は同じ理由で失敗しないか。
8. 差別化は本質的か、それとも表層的か。
9. 抗体フォーマットは新しい薬理を作っているか。
10. 「本当にこれは新しい」と言える一文は何か。

この10問に弱い候補は、開発しやすくても低評価にする。

## Reinterpretation Of Old Axes

従来の軸は以下のように読み替える。

| 旧評価軸 | 新しい読み替え |
|---|---|
| Unmet medical need | unmetが大きくても競合後追いなら低評価 |
| Target biology | biologyが強くても既に占有された標的なら低評価 |
| Antibody tractability | 抗体化しやすいだけでは不十分 |
| Differentiation potential | 「差別化」ではなく「非模倣性」をまず見る |
| Safety window | 安全そうなme-tooより、リスクを明示した革新仮説を優先 |
| Biomarker strategy | 競合も同じbiomarkerを使えるなら弱い |
| Developability | 最終確認項目。初期順位を決める主軸にしない |

## Proposed Reporting Changes

Target Cardやproposalには、以下を必ず追加する。

## Novelty audit

| 項目 | 内容 |
|---|---|
| Nearest existing / pipeline asset | 最も近い既存薬・開発品 |
| Why this is not a copy | どこが根本的に違うか |
| What would make this a copy | どの条件なら後追いと判断するか |
| If competitor succeeds | 先行品成功時に残る価値 |
| If competitor fails | 先行品失敗時に残る理由 |

## Innovation thesis

以下を1文で書く。

```text
この候補は、既存の [標的/MoA/疾患ポジション] ではなく、[新しい病態仮説/抗体薬理/患者定義] を狙う点で新しい。
```

この1文が書けない候補は推奨しない。

## Recommendation

今後の探索では、既存薬・開発品をなぞる候補を早期に落とす。特に、CD19/CD20、BAFF/APRIL、FcRn、CD40L、IL-6、TNF、IL-17、C5など、既に臨床開発が厚い領域では、単なる標的変更やformat変更を革新性として扱わない。

優先すべきは、以下のような候補である。

- 新しい細胞状態を狙う抗体。
- 病変組織だけで活性化する抗体。
- 病的細胞間相互作用を空間的に壊す抗体。
- 免疫抑制ではなく免疫再教育や組織リセットを狙う抗体。
- 既存競合が使えないbiomarkerと薬理が一体化した抗体。
- 先行品が成功しても失敗しても、独立した仮説として残る候補。
