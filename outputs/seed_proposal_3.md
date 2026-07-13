# Seed Proposal 3: 線維化自己免疫疾患向けCCL24中和抗体

## 1文での提案

Systemic sclerosisなど進行性線維化を伴う自己免疫疾患に対し、CCL24を中和して炎症細胞動員と線維化シグナルを抑える抗体を提案する。

## 疾患の壁

- Systemic sclerosisは皮膚線維化、間質性肺疾患、血管障害を伴い、不可逆的な臓器障害につながる。
- 既存の免疫抑制薬や抗線維化薬では、線維化の反転や進行抑制が十分でない患者が残る。
- 疾患が異質で、炎症優位、線維化優位、血管障害優位の患者が混在する。

## 標的の妥当性

- CCL24/eotaxin-2は分泌ケモカインで、CCR3を介した好酸球/炎症細胞動員に関与する。
- 炎症と線維化をつなぐ標的候補として、SScや線維化疾患での開発仮説がある。
- ただし、CCL24が疾患ドライバーか、単なる炎症/線維化マーカーかは未確定。

## 抗体である必然性

- CCL24は分泌タンパク質で、抗体中和に適している。
- 高選択的にCCL24を中和でき、CCR3下流の細胞遊走と組織炎症を抑える仮説を検証しやすい。
- 抗原sinkが問題になる場合、pH-dependent recycling antibodyでPK/PD差別化を狙える。

## 抗体設計案

- 主案: Neutralizing blocking antibody
  - CCL24を中和し、CCR3依存のchemotaxisと線維化関連readoutを抑える。
- 副案: pH-dependent recycling antibody
  - 分泌ケモカインの抗原sinkに対応し、投与量・持続性で差別化を狙う。
- 条件付き案: Bispecific antibody
  - CCL11/CCL26など冗長ケモカインが強い場合のみ検討。ただし安全性とCMCが重くなる。

## 既存薬との差別化

- IL-6、B細胞、TGF-beta/integrin、nintedanib系とは異なるchemokine-fibrosis軸を狙う。
- SScの炎症-線維化サブセットに絞ることで、広い抗線維化薬より精密な患者選択を提案できる。
- 競合過密度はCD20、IL-6、FcRn、IL-17などより低い可能性がある。

## 主要リスク

- CCL24が線維化の原因ではなく、二次的マーカーである可能性。
- CCL11/CCL26など他のCCR3 ligandによる冗長性。
- 好酸球/宿主防御、アレルギー応答、組織修復への影響。
- 分泌ケモカインの抗原sinkにより、実用的な投与量が高くなる可能性。
- CM-101様プログラムが進む場合、後発性が出る。

## 最初にやるべき検証実験

1. SSc皮膚、肺、血清でCCL24、CCR3+細胞、線維化マーカーの発現を確認する。
2. SSc skin/lung explantまたはfibroblast-immune cell co-cultureで、CCL24中和がCOL1A1、ACTA2、炎症性chemokine、myeloid/eosinophil migrationを抑えるか確認する。
3. CCL11/CCL26添加または患者サンプル比較で、冗長性により効果が消えるか検証する。
4. 通常中和抗体とpH-dependent recycling案で、抗原sinkモデル、pH結合、neutralization potency、PK/PDを比較する。

## Go / No-Go基準

| 判定 | 基準 |
|---|---|
| Go | CCL24-highかつCCR3-cell-richのSSc/線維化自己免疫サブセットが確認できる。 |
| Go | CCL24中和によりヒト疾患組織で線維化・炎症readoutが低下する。 |
| Go | CCL11/CCL26冗長性を超える、または患者選択で回避できる。 |
| No-Go | CCL24発現が疾患組織で弱い、または血清マーカーに留まる。 |
| No-Go | CCL24中和で機能readoutが動かない。 |
| No-Go | 抗原sink/PKにより実用的な投与量が成立しない。 |
