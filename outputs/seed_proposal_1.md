# Seed Proposal 1: BAFF-R選択的B細胞制御抗体

## 1文での提案

Sjogren diseaseを中心とするB-cell-high自己免疫疾患に対し、BAFF-Rを選択的に阻害し、必要に応じて限定的にB細胞を制御する抗体を提案する。

## 疾患の壁

- Sjogren diseaseでは乾燥症状、疲労、疼痛、全身臓器病変が残り、疾患修飾的な治療選択肢が限定的。
- SLE/LNや自己免疫性肝炎などにもB細胞・自己抗体軸があるが、既存治療では再燃、ステロイド依存、感染リスクが残る。
- 広い患者集団では臨床効果が希釈されやすく、B-cell-highサブセットを定義する必要がある。

## 標的の妥当性

- BAFF-R/TNFRSF13CはB細胞表面受容体で、BAFF依存性の成熟B細胞生存に関わる。
- BAFF軸はSLE/Sjogren病態と整合し、belimumabなどで経路妥当性が一定程度示されている。
- ただし、BAFF/APRIL軸ではtabalumabのefficacy不足、ataciceptの疾患悪化例など、臨床失敗パターンもある。

## 抗体である必然性

- BAFF-Rは膜タンパク質で、抗体によりリガンド結合阻害とFc機能調整を両立できる。
- BAFF ligand阻害ではなく受容体を直接狙うことで、BAFF-R陽性B細胞への選択性と作用強度を設計できる。
- 小分子よりも細胞表面受容体占有、Fc-silent/Fc-enabled設計、B細胞サブセット制御の自由度が高い。

## 抗体設計案

- 主案: Fc-silent blocking antibody
  - BAFF-RへのBAFF結合を阻害しつつ、ADCC/CDCを抑えて慢性投与の安全性を重視する。
- 副案: Moderately Fc-enabled blocking/depleting antibody
  - 高活動性B-cell-high患者で、限定的なBAFF-R陽性B細胞除去を狙う。
- 非推奨: Agonistic antibody、ADC
  - 自己免疫悪化または過剰B細胞毒性の懸念が大きい。

## 既存薬との差別化

- BelimumabなどBAFF ligand阻害に対して、BAFF-R陽性B細胞を直接制御できる。
- CD20/CD19枯渇に対して、よりB細胞生存軸に寄せた選択的・調整可能な設計が可能。
- Ianalumab競合に対しては、Fc-silent安全性、患者選択、投与設計、または特定疾患サブセットで差別化する必要がある。

## 競合品の患者選択状況

公開情報ベースでは、BAFF-R依存的にB細胞活性が維持されている患者サブセットを明示的に対象化した競合品・開発中止品は確認できていない。

| 薬剤/試験 | 標的 | 患者選択 | BAFF-R依存サブセットか |
|---|---|---|---|
| ianalumab / VAY736 | BAFF-R | active Sjogren、anti-Ro/SSA陽性または唾液腺生検陽性、ESSDAI、唾液分泌など | いいえ。BAFF-R標的薬だが、BAFF-R依存性では選んでいない |
| ianalumab biopsy MoA study | BAFF-R | anti-Ro/SSA陽性、ESSPRI高値など | いいえ。機序理解に近いが、BAFF-R依存性選択ではない |
| sibeprenlimab | APRIL | Sjogren、IgG高値、anti-Ro52/60陽性など | 近いが違う。B-cell/抗体high寄りだがBAFF-R依存ではない |
| belimumab | BAFF | autoantibody-positive SLE、anti-dsDNA/低補体など | BAFF軸だがBAFF-R依存ではない |
| atacicept | BAFF/APRIL | active SLE、ANA/anti-dsDNA陽性など | BAFF/APRIL軸だがBAFF-R依存ではない |
| tabalumab | BAFF | active SLE、ANA陽性など | BAFF阻害だがBAFF-R依存ではない |

このため、単なるanti-BAFF-R抗体では競合性が高いが、BAFF-R依存性を機能的に定義して患者選択する戦略には、まだ差別化余地がある。

## ianalumabで未解決になりうる課題と狙える余地

Ianalumabは最も近い競合であり、BAFF-R標的として先行している。したがって、ianalumabが承認・標準化された場合、同じBAFF-R抗体を後追いで出すだけではファーストインクラスにはならない。狙うべき余地は、ianalumabの公開試験設計から見てまだ残りうる以下の課題である。

| 未解決になりうる課題 | ianalumabでの状況 | 本提案で解決を狙う方向 |
|---|---|---|
| 反応患者の予測 | NEPTUNUS試験はanti-Ro/SSA、ESSDAI、唾液分泌などで選択しており、BAFF-R依存性そのものでは選んでいない | BAFF-R dependency scoreとex vivo機能アッセイで反応患者を濃縮する |
| 乾燥・疲労など患者報告アウトカム | SSSD、ESSPRI、FACIT-Fなどは評価されているが、臨床的に十分な改善が得られるかは公開情報だけでは不明 | B-cell-highかつ腺機能が残る患者に絞り、症状改善可能性を高める |
| 腺機能回復 | stimulated salivary flowは評価項目に入っているが、構造的に壊れた腺は戻りにくい可能性 | 唾液腺B細胞浸潤、BAFF/BAFF-R発現、残存唾液分泌を組み合わせ、可逆性がある患者を狙う |
| 慢性安全性 | BAFF-R標的はB細胞抑制/除去により感染、低IgG、ワクチン応答低下が懸念される | Fc-silent blockingを主案にし、過剰なB細胞depletionを避ける |
| 既存薬との差別化 | BAFF-Rを直接標的とする点はianalumabと同じ | 「非depleting寄り」「機能的患者選択」「腺局所/全身活動性サブタイプ」で差別化する |

## ファーストインクラスになるために必要なプロファイル

厳密には、ianalumabがBAFF-R抗体として承認されれば、単純なBAFF-R抗体はファーストインクラスではない。ファーストインクラスを主張するには、単なる標的名ではなく、以下のような新しい治療コンセプトとして成立させる必要がある。

| 必要プロファイル | 内容 |
|---|---|
| 新しい患者定義 | `BAFF-R依存B-cell-high Sjogren` という機能的サブセットを定義する |
| Companion-like biomarker | BAFF-R発現、BAFF応答性、抗BAFF-R ex vivo抑制を組み合わせた患者選択法を持つ |
| Non-depleting BAFF-R modulation | B細胞を広く枯渇させるのではなく、BAFF-R survival signalを選択的に抑える |
| 慢性安全性 | 低IgG、感染、ワクチン応答低下がianalumab型depleting抗体より軽い |
| 症状または腺機能への明確な価値 | ESSDAIだけでなく、乾燥、疲労、唾液腺機能など患者価値に近いreadoutで優位性を示す |
| 既存BAFF/BAFF-R薬との差別化 | BAFF ligand阻害、BAFF/APRIL阻害、depleting BAFF-R抗体と比較して、PD/安全性/患者選択で明確に異なる |

現実的には、標的ベースのファーストインクラスよりも、`precision BAFF-R modulator` または `first biomarker-defined BAFF-R therapy` としての差別化を狙う方が妥当である。

## BAFF-R依存患者を知るためのバイオマーカー案

単一の確定バイオマーカーは不明。現実的には、血液・組織・機能アッセイを組み合わせて `BAFF-R dependency score` のような複合指標を作る。

| Category | Marker / assay | 意味 |
|---|---|---|
| Ligand | serum BAFF、唾液腺BAFF/TNFSF13B発現 | BAFF環境が強いか |
| Receptor | CD19+ B細胞上BAFF-R MFI、BAFF-R+ B細胞割合 | 標的細胞が存在するか |
| B-cell activation | plasmablast、CD21low B cells、activated naive B cells | B細胞が活性化しているか |
| Humoral activity | IgG高値、RF、anti-SSA/Ro、free light chains | 抗体産生系が強いか |
| Systemic activity | ESSDAI、低補体、cryoglobulin | 全身性B細胞病態があるか |
| Tissue biology | 唾液腺B細胞浸潤、CXCL13、ectopic GC-like structure | 局所B細胞反応があるか |
| Functional dependency | BAFF刺激でB細胞が生存/活性化し、抗BAFF-R抗体で抑制される | BAFF-R依存性の直接証拠に近い |

最重要はfunctional dependencyである。serum BAFF高値、anti-SSA陽性、IgG高値だけではBAFF-R依存とは言えない。

## 主要リスク

- ianalumabなど競合が進んでおり、後発性が出やすい。
- B細胞PD変化が乾燥症状や疲労など臨床アウトカムに直結しない可能性。
- 感染、低IgG、ワクチン応答低下。
- APRIL、CD40L、組織内B細胞ニッチなどによる冗長性。
- BAFF-R依存性を定義する複合バイオマーカーが作れない場合、競合との差別化が弱くなる。

## 最初にやるべき検証実験

1. Sjogren/SLE患者PBMCまたはB細胞で、BAFF依存B細胞生存を阻害できるか確認する。
2. B-cell-high患者サンプルで、自己抗体産生、plasmablast、B-cell activation signatureを抑制できるか測る。
3. BAFF ligand阻害、CD20/CD19系の既存作用様式とex vivoで比較する。
4. Fc-silent案とFc-enabled案で、ADCC/ADCP、IgG低下予測、安全性マージンを比較する。
5. BAFF-R dependency score候補を作り、反応性と相関するか検証する。

## Go / No-Go基準

| 判定 | 基準 |
|---|---|
| Go | B-cell-high患者サンプルでBAFF-R依存性が示され、BAFF ligand阻害より明確なPD差がある。 |
| Go | Fc-silent案で十分なB細胞機能抑制が得られ、Ig低下・感染リスクを抑えられる見込みがある。 |
| Go | BAFF-R dependency scoreまたは機能アッセイにより、反応患者を事前に濃縮できる。 |
| No-Go | BAFF-R blockadeがBAFF ligand阻害と同質で、差別化が見えない。 |
| No-Go | B細胞PDは動くが、疾患関連readoutに結びつかない。 |
| No-Go | 低IgG、広範B細胞毒性、または慢性投与に不適な安全性シグナルが出る。 |
| No-Go | serum BAFFや自己抗体などの相関マーカーしかなく、BAFF-R依存性を機能的に示せない。 |
