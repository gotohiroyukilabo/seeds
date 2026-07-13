# Scoring Rubric

このrubricは、抗体医薬シーズ候補を「開発しやすそうか」ではなく、「本当に新しいか」を中心に評価するためのものである。

最重要ルール:

```text
開発可能性が高くても、既存薬・開発品の後追いなら低評価。
開発可能性が不確実でも、革新的で早期検証可能なら高評価候補として残す。
```

各候補を以下の観点で 1〜5 点で評価する。

## 1. Non-mimicry / 非模倣性

- 5: 既存薬・臨床開発品と標的、MoA、疾患ポジション、患者選択、抗体設計思想が明確に異なる。
- 3: 一部は既存品に近いが、疾患セグメント、抗体設計、作用機序に意味のあるズレがある。
- 1: 既存薬・開発品のme-too / me-better / 言い換えに近い。

## 2. Conceptual novelty / 概念的新規性

- 5: 疾患の見方を変える新しい病態仮説、細胞間相互作用、組織ニッチ、時間軸、患者状態を提示している。
- 3: 既存概念を組み合わせた新規性はあるが、根本的に新しいとは言いにくい。
- 1: 既存のサイトカイン阻害、B細胞阻害、補体阻害、FcRn阻害などの延長。

## 3. Mechanistic originality / 機序の独自性

- 5: 抗体だから作れる新しい薬理がある。単なるblocking/depletionではない。
- 3: 既存MoAに近いが、抗体フォーマットや条件付き活性化により新しい作用が一部ある。
- 1: ligand blockade、receptor blockade、cell depletionなど既存MoAと同質。

## 4. Competitive whitespace / 競合空白

- 5: 競合が少ない、または競合と明確に違う病態・患者・技術領域にいる。
- 3: 競合はあるが、避けられるセグメントや設計余地がある。
- 1: 競合密集。先行品が成功したら候補価値が消える。

## 5. Antibody necessity / 抗体である必然性

- 5: 抗体でなければ実現しにくい空間制御、細胞間架橋、条件付き活性、選択的輸送、標的分子制御がある。
- 3: 抗体が適しているが、他モダリティでも代替可能。
- 1: 抗体にする理由が半減期、特異性、慣れた開発形式だけ。

## 6. Human biology plausibility / ヒト病態妥当性

- 5: ヒト疾患組織、single-cell/spatial data、遺伝学、患者サンプル、臨床観察が整合する。
- 3: 限定的なヒトデータと前臨床仮説がある。
- 1: 主に動物モデル、一般論、推測に依存する。

## 7. Early falsifiability / 早期反証可能性

- 5: 3〜6か月でGo/No-Goを判断できる明確なヒトサンプル・機能 assay・kill criteriaがある。
- 3: 評価系はあるが、患者PoCへの橋渡しが弱い。
- 1: 何を見れば仮説が否定されるか不明。

## 8. Unmet medical need

- 5: 既存治療で十分に制御できず、重症度または患者負担が大きい。
- 3: 既存治療はあるが一部に不十分。
- 1: 既存治療でかなり充足されている。

## 9. Target biology

- 5: 疾患因果との関係が強く、かつ既存の切り口とは異なる。
- 3: 関連はあるが因果性または新規性が限定的。
- 1: 相関レベル、または既に十分に薬剤化された標的。

## 10. Biomarker originality / バイオマーカー独自性

- 5: 提案MoAと機械的に結びついた患者選択があり、競合が簡単にコピーできない。
- 3: 患者選択候補はあるが、競合も同じ指標を使える。
- 1: ほぼ不明、または既存品と同じ患者選択。

## 11. Safety logic

- 5: 新規MoAに対する主要安全性リスクが明確で、早期評価系がある。
- 3: 注意すべき毒性はあるが、評価計画は立てられる。
- 1: on-target toxicityが強く懸念される、または安全性評価が曖昧。

## 12. Developability

- 5: 革新性を損なわずに実装可能性がある。
- 3: bispecific、masked、ADC、Fc改変などの難度はあるが検討可能。
- 1: CMC、物性、投与、免疫原性の難度が極めて高い。

注意: Developabilityは最終項目であり、革新性項目より重く扱わない。

## 推奨度の決め方

### High

以下を満たす候補:

- Non-mimicry、Conceptual novelty、Mechanistic originalityのいずれかが5点。
- 既存薬・開発品の後追いではない。
- 早期反証可能性がある。
- 開発可能性に不確実性があってもよい。

### Medium

以下の候補:

- 新規性はあるが、既存品との距離がまだ十分ではない。
- 明確な患者セグメントや抗体設計で差別化できる可能性がある。
- 追加調査でHighまたはLowに振り分ける。

### Low

以下の候補:

- 既存薬・開発品と同じ標的/MoA/疾患ポジション。
- 差別化が「少し安全」「少し便利」「少し効くかも」に留まる。
- 競合が成功したら不要になる。
- 開発しやすくてもLowにする。

### Conditional

以下の候補:

- Biologyは強いが、先行品に近すぎる。
- benchmarkに勝つ、FTOが取れる、疾患セグメントをずらす、独自biomarkerがあるなどの条件付きでのみ検討する。

## Novelty audit template

各候補には以下を必ず記載する。

| 項目 | 判定 | コメント |
|---|---|---|
| Existing / pipeline nearest neighbor |  | 最も近い既存薬・開発品 |
| Target novelty | Same / Adjacent / New |  |
| MoA novelty | Same / Modified / New |  |
| Disease-position novelty | Same / Segment-shifted / New |  |
| Modality novelty | Cosmetic / Useful / Essential |  |
| Biomarker novelty | Copyable / Partly unique / Mechanistically tied |  |
| If nearest competitor succeeds | Candidate survives? Yes / Maybe / No |  |
| If nearest competitor fails | Candidate survives? Yes / Maybe / No |  |
| Why this is not a copy |  |  |
| What would make this No-Go immediately |  |  |
