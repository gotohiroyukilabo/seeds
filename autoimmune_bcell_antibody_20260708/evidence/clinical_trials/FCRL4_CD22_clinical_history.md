# 臨床履歴: FCRL4 x CD22

## 直接の臨床履歴
FCRL4標的の自己免疫抗体薬の臨床開発は確認していない。CD22にはepratuzumabという先行例があり、SLE Phase IIIで失敗した。

2026-07-12時点でClinicalTrials.govを `FCRL4`、`FcRL4`、`FCRH4`、`FcRH4`、`CD307d` で検索した範囲では、FcRL4直撃の治療介入試験は0件だった。`IRTA1` では `NCT06424379` が出るが、非ホジキンリンパ腫の病理・分子解析であり治療薬ではない。

ただし近縁のFCRL5/FcRH5では、Genentech/Rocheのcevostamab/FcRH5 x CD3が多発性骨髄腫で複数試験を持ち、SLE with/without active lupus nephritisのPhase Ib試験 `NCT07629583` が2026-07-31開始予定で登録されている。FcRL4直接競合ではないが、FCRL family自己免疫競合としてwatchする。

## epratuzumabで何が失敗したか
「CD22が完全に失敗した」と読むのは不正確である。より正確には、広いmoderate-to-severe非腎/非CNS SLEで、標準治療上乗せのCD22 modulationがplaceboと明確に差をつけられなかった。

- Phase IIb EMBLEMでは2400 mg cumulative doseに探索的signalがあった。
- Phase III EMBODY 1/2では各試験約790例がrandomizedされ、week 48の主要評価で有意差なし。
- 大きな新規安全性signalはなく、主問題はefficacy separationだった。
- 作用機序研究では、epratuzumabがFc依存trogocytosisによりCD22/CD19/CD21/CD79bを低下させることが報告されている。

## Fc依存性trogocytosisとは何か
Fc依存性trogocytosisは、抗体が結合した標的細胞の膜成分を、FcγR陽性細胞が接触依存的に取り込む現象である。epratuzumabでは、CD22に結合した抗体のFcが単球、NK細胞、顆粒球などのFcγRに認識され、CD22だけでなくCD19、CD21、CD79bなどのBCR関連表面分子もB細胞表面から低下する。これは典型的な細胞殺傷ではなく、B細胞表面の受容体構成を変えることでBCR反応性を下げる可能性がある。

この作用が重要だった場合、Fc-silent FCRL4 x CD22は効力不足になる可能性がある。一方で、Fc-activeにすると非選択的なB細胞表面分子strippingや局所炎症のリスクが出る。そのため本提案では、Fc-silentを機序検証の主案としつつ、Fc-active/Fc-tuned型を初期から並行比較する。

## FCRL4 x CD22で救える点/救えない点
| epratuzumabの問題 | FCRL4 x CD22の返答 | 解釈 |
|---|---|---|
| 病的B細胞stateの選択なし | FCRL4+ gland B-cell-highに絞る | 強く合致 |
| 組織ニッチ非選択 | FCRL4を唾液腺B細胞住所にする | 強く合致 |
| CD22単独modulationが弱い | cis co-ligationで強める仮説 | 実験必須 |
| Fc依存trogocytosisが作用に関与 | Fc-silent設計では失う可能性。Fc-active/Fc-tunedでFCRL4-gated trogocytosisを評価 | 残リスクだが設計分岐可能 |
| 臨床endpoint/placebo response | 初期はex vivo機能で判定 | 後期では残る課題 |

## 失敗モード
FCRL4がbystander、CD22/SHP-1抑制が弱い、Fc-silentでは効かない、Fc-active化で非選択的trogocytosisや局所炎症が出る、組織到達不足、血液biomarkerが組織を反映しない、粘膜記憶B細胞毒性。

## 開発上の示唆
peripheral bloodだけで進めない。fresh唾液腺B細胞で、FCRL4 x CD22がanti-CD22単独およびanti-FCRL4 + anti-CD22併用を上回ることが最重要。Fc-silentとFc-active/Fc-tunedを同時に比較し、薬効がCD22/SHP-1抑制なのか、FcγR依存trogocytosisなのか、両方なのかを分けて判断する。

FCRL5 x CD3がSLE/LNで先行する可能性を考えると、Proposal 2はSLEに無理に寄せず、Sjögren腺内FcRL4+ B細胞のtissue silencerとして差別化する方がよい。競合詳細は [FCRL4_competitor_landscape.md](../competitive_landscape/FCRL4_competitor_landscape.md) を参照。

## 参考文献
- Epratuzumab Phase III EMBODY: https://doi.org/10.1002/art.39856
- Epratuzumab Phase IIb EMBLEM: https://doi.org/10.1136/annrheumdis-2012-202760
- Epratuzumab trogocytosis: https://doi.org/10.1182/blood-2012-12-473744
- FcRL4+ B cells in Sjögren salivary glands: https://doi.org/10.1016/j.jaut.2017.03.012
- Cevostamab SLE/LN Phase Ib: https://clinicaltrials.gov/study/NCT07629583
- Cevostamab MM Phase I: https://clinicaltrials.gov/study/NCT03275103
