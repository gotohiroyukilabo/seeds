# FcRL4抗体作製論文の整理: 取得方法・IgA J-chain競合性・ファミリー特異性

作成日: 2026-08-25

## 一言メッセージ

FcRL4抗体は研究用mAbとして複数報告されているが、治療抗体として十分にde-riskされたクローンは見当たらない。最も重要なのは、`413D12` がIgA結合をブロックする実験的陽性対照、`1A3` がFcRL4/FcRL5識別の比較的信頼できる染色用対照、`2A6` が後年FcRL5交差反応を指摘された注意すべき負の教材である、という整理である。

## 今回の調査範囲

- 「FcRL4抗体を自作・作製・初期特性評価している論文」を中心にした。
- 既存クローンを使っただけの疾患論文は、特異性評価に重要なものだけ補助的に含めた。
- IgA J-chainとの競合性は、論文で直接評価されたかを優先し、直接評価がなければ「不明」とした。
- 2026年の構造論文に基づくJ-chain interfaceとの関係は、直接データではなく「推論」と明記した。

## 結論サマリー

| クローン/抗体 | 主な作製論文 | 取得方法 | IgA/J-chain競合性 | FcRLファミリー特異性 | 開発上の読み |
|---|---|---|---|---|---|
| `2A6` | Ehrhardt et al., J Exp Med 2005 | FcRH4/FcRL4 ECD組換えタンパク質でマウス免疫、ハイブリドーマ | 不明。IgA/J-chain競合スクリーニングではない | 当初はFcRH4特異的とされたが、後年FCRL5にも強く結合することが報告 | 新規抗体開発のベンチマークには不向き。FCRL5交差反応リスクの教材として使う |
| `1A3` | Polson et al., Int Immunol 2006 | His-tag FcRH/IRTA ECDをCHOで発現、Balb/c/Xenomouse免疫、ELISA/FACSで選別 | 不明。リガンドブロック抗体としては選別されていない | FcRH1-5/IRTA1-5安定発現細胞で特異性確認。後年も1A3はFCRL4特異的と再確認 | 染色・患者サンプル層別化の陽性対照候補。治療抗体化にはエピトープ/機能評価が不足 |
| `413D12` | Wilson et al., J Immunol 2012 | FcRL4安定発現P815細胞でBalb/c免疫、FACSでFcRL4発現細胞特異的クローンを選別 | heat-aggregated IgA結合をブロック。J-chain-linked IgAでの直接競合は未評価 | 少なくともFCRL5とは非交差と記載。全FcRL横断の詳細は限定的 | IgA/J-chain結合面を狙う抗体の最重要陽性対照。dIgA-J競合で再評価すべき |
| `418C8` | Wilson et al., J Immunol 2012 | `413D12`と同じ免疫・ハイブリドーマ系 | heat-aggregated IgA結合はブロックしない | 詳細不明 | non-blocking対照として有用。結合だけで細胞除去する設計なら比較対照になる |
| `M-IRTA1` | Falini et al., Blood 2003 | IRTA1/FcRL4の細胞外部分に対するmAb。IHC/WB/IPで検証 | 不明。IgA/J-chain発見前の病理抗体 | IRTA2-5 transfectantではバンドなしと報告 | FFPE病理/IHCに強い可能性。治療抗体候補としては表面細胞結合・リガンド競合が不明 |
| `A1` | 市販抗体/BD・Thermo・Novus/Bio-Techne | DNA immunization後にCD307d/FCRL4/FcRH4/IRTA1 transfectantでboost | 不明。vendor dataではリガンド競合評価なし | FCRL4/CD307d認識抗体として市販。HLDA/CD designationにも使われたと記載。ただしFcRL1-6全体の横断特異性は不明 | `1A3`とは別物。入手しやすいnative-cell staining referenceとして有用 |
| `580810` | 市販抗体/R&D Systems・Thermo | NS0由来recombinant human FCRL4/FcRH4 Gln16-Asp385で作製 | 不明。vendor dataではリガンド競合評価なし | direct ELISAでrecombinant human FCRL1との非交差は記載。他のFCRL2/3/5/6は不明 | Flow/CyTOF用の独立市販binder。413D12/A1とのbinning対照として有用 |

## Reference antibodyの入手性アップデート

前項での「reference antibody」は「論文上の比較対照として有用」という意味であり、4本すべてが通常カタログで簡単に買えるという意味ではない。実務上は以下のように分けて考える。

| クローン | 現時点の入手性 | 根拠/候補ルート | 実験での使い方 |
|---|---|---|---|
| `413D12` | 入手しやすい | BioLegendにpurified品 `340202`、PE/APC/PerCP-Cy5.5/TotalSeqなどの複数formatがある。Thermo/eBioscienceにもAPC `17-3079-42`、PerCP-eFluor 710 `46-3079-42`がある。Washington University OTMにもhybridoma `T-007612`として掲載がある。 | 最優先で入手するreference。blocking assayにはconjugated品ではなくpurified品を使う。 |
| `1A3` | 通常カタログ品としては未確認 | 論文ではGenentech提供品。Genentech/ATCC deposit関連特許ではanti-FcRH4-1A3が記載されるが、一般購入できる保証はない。 | 入手できればFCRL4/FCRL5識別のよい対照。ただし現実的には「要問い合わせ/MTA候補」。 |
| `418C8` | 入手困難 | Wilson 2012でnon-blocking anti-FcRL4として登場するが、通常カタログ品や明確な公開hybridomaルートは未確認。 | 厳密には欲しいが、まずは自前取得抗体の中から413D12 non-competing/non-blocking cloneを作る方が現実的。 |
| `2A6` / `4-2A6` | 入手困難、かつ優先度低 | 論文ではMax Cooper group由来の提供品として使われる例がある。特許上は4-2A6 hybridoma depositが記載されるが、一般購入できる保証はない。 | FCRL5交差反応を示す負の教材。新規抗体開発の実験対照としては必須ではない。 |

### 市販代替クローン

`A1`と`580810`は、ここまでの作製論文で出てきたhistorical cloneとは少し性格が異なる。いずれも市販の研究用抗体で、referenceとしての強みは「実際に買いやすい」「FACS/CyTOF panelに組み込みやすい」ことである。一方で、創薬seedとして重要な可変領域配列、詳細エピトープ、J-chain-linked IgAとの競合性、FcRL family横断特異性は十分には公開されていない。

### `413D12`、`A1`、`580810`の配列公開状況

| クローン | VH/VLまたはCDR配列の公開状況 | 実務上の解釈 |
|---|---|---|
| `413D12` | 公開情報からは確認できず | Wilson 2012、市販vendor、Washington University OTMのhybridoma情報では、clone名、isotype、用途、blocking活性は分かるが、可変領域配列は出ていない。市販抗体はassay controlとして使う。 |
| `A1` | 公開情報からは確認できず | Thermo/Novus/BDの製品情報では、免疫原、host/isotype、用途、CD designation関連情報はあるが、配列は出ていない。`1A3`とは別cloneであり、配列代替にはならない。 |
| `580810` | 公開情報からは確認できず | R&D Systems/Thermoの製品情報では、免疫原、用途、FCRL1非交差情報はあるが、配列は出ていない。創薬seedではなく、binning/染色/competition assay用referenceと考える。 |

したがって、これら3本は「配列を使って抗体を再構築するreference」ではなく、「実物を購入してbinding、binning、blocking、patient sample stainingの基準にするreference」である。配列が必要な場合は、権利者/vendor/寄託機関への問い合わせ、または入手抗体/ハイブリドーマからのsequencingが必要になる。ただし、市販RUO抗体のreverse engineeringやsequencingは契約条件で制限される場合があるため、事前確認が必要である。

#### `A1` clone

| 項目 | 内容 |
|---|---|
| 主な入手先 | Thermo Fisher/Invitrogen `MA574633`、Novus/Bio-Techne `NBP3-11836`、BD Biosciences `566587`など |
| host/isotype | mouse IgG2a, kappa |
| 主な用途 | Flow cytometry、IHC-frozen。BD/Novusでは多数の蛍光標識formatもある |
| 免疫原 | ThermoではDNA immunization後にCD307d-transfected cellsでboost。Novus/Bio-TechneではDNA immunization後にFCRL4/FcRH4/IRTA1-transfected cellsでboost。BDではhuman FCRL4 cDNAと記載 |
| epitope情報 | Novus/Bio-TechneではFCRL4/FcRH4/IRTA1のextracellular domain内epitopeを認識と記載 |
| CD designation | Novus/Bio-Techneでは、clone A1がHLDAによるCD designationに使われたと記載。BD製品にもWorkshop Number `IX 23`の記載がある |
| vendor上の検証 | human lymphocyteでのflow cytometry画像が提示されている |
| J-chain/IgA競合性 | 不明。J-chain-linked IgAやdIgA coreとのcompetition dataは見当たらない |
| FcRL family特異性 | 不明。少なくともvendor page上ではFCRL1/2/3/5/6横断の創薬水準データは確認できない |

`A1`は`1A3`と名前が似ているが別クローンである。`1A3`をGenentech由来のhistorical FcRL4-specific cloneとして扱う一方、`A1`は「入手性のよい市販native-cell staining clone」として分けるべきである。DNA/cDNA immunizationとtransfectant boostで得られた抗体なので、recombinant soluble ECDだけで取った抗体よりも、細胞表面native conformationを認識する可能性は高い。ただし、これをもってJ-chain occupied FcRL4に結合できる、またはFCRL5を含む近縁familyと完全に非交差である、とは言えない。

実験上の使いどころは、`413D12`とは別bin候補の染色対照、FCRL4+ B cellのFACS gating確認、患者検体での抗原検出である。FcRL4 x CD3やFcRL4 x CD22のtargeting arm設計を考える場合、`A1`に近いbinは「ligand blockingではなく表面markerとしてFcRL4を拾う」方向の参考になる可能性がある。最初の評価では、`413D12`とのcompetition、dIgA-J存在下でのbinding維持、FCRL1/2/3/5/6単独発現細胞での交差反応確認を必須にする。

#### `580810` clone

| 項目 | 内容 |
|---|---|
| 主な入手先 | R&D Systems/Bio-Techne `MAB24262`、Thermo Fisher/Invitrogen `MA5-24262`など |
| host/isotype | mouse IgG1 |
| 主な用途 | Flow cytometry、CyTOF-ready。R&D/Bio-Techneではunconjugatedのほか、Alexa Fluor、APC/Cy7、Biotin、CoraFluor、DyLight、HRP、PEなど多数formatがある |
| 免疫原 | NS0-derived recombinant human FCRL4/FcRH4 Gln16-Asp385、accession `NP_112572` |
| vendor上の検証 | RPMI 8226 human multiple myeloma cell lineでflow cytometry画像が提示されている |
| 特異性 | direct ELISAでhuman FCRL4/FcRH4を検出し、recombinant human FCRL1との交差反応なしと記載 |
| J-chain/IgA競合性 | 不明。J-chain-linked IgA、dIgA core、secretory componentとのcompetition dataは見当たらない |
| FcRL family特異性 | FCRL1との非交差は記載あり。ただしFCRL2/3/5/6を含む横断検証は不明 |

`580810`は、recombinant ECD免疫で得られた市販cloneとして扱うのがよい。免疫原のGln16-Asp385はFCRL4の細胞外領域を広く含むため、理屈の上ではJ-chain interface近傍も別領域も取りうるが、epitopeは公開情報からは分からない。`413D12`がligand blockingの陽性対照であるのに対し、`580810`は「別エピトープかもしれない市販binder」としてbinningに使うのが現実的である。

`580810`の利点は、BSA/carrier-freeのunconjugated品やCyTOF-readyの位置づけがあり、多色flowやmass cytometry panelに組み込みやすい点である。一方、recombinant protein免疫由来なので、primary tissueのnative FcRL4、glycoform、ligand-occupied receptor上での結合性は別途確認が必要である。特にFCRL5交差反応は`2A6`の教訓があるため、FCRL5単独発現細胞で潰すべきである。

#### `A1`と`580810`をreferenceに入れる意味

| 比較軸 | `A1` | `580810` | 実務判断 |
|---|---|---|---|
| 入手性 | 高い。BD/Thermo/Novus系で複数format | 高い。R&D/Thermo系で複数format | どちらも`1A3`/`418C8`/`2A6`より現実的 |
| 免疫原の性格 | DNA/cDNA immunization + transfectant boost | recombinant ECD | `A1`はnative-cell staining寄り、`580810`はECD binder寄り |
| ligand blocking reference | 不明 | 不明 | blocking陽性対照は引き続き`413D12` |
| patient sample gating | 有望 | 有望だがRPMI 8226検証中心 | pSS唾液腺/扁桃で両方比較する |
| BsAb/ADC設計への示唆 | non-blocking targeting arm候補bin探索に有用 | 413D12/A1と異なるbin探索に有用 | 直接seedではなくbinning/assay controlとして使う |
| 主な弱点 | family横断特異性とJ-chain競合性が不明 | FCRL1以外のfamily交差反応とJ-chain競合性が不明 | FCRL1-6 cell panelとdIgA-J competitionを必須化 |

### 実務上の推奨reference panel

1. `413D12 purified`: ligand blocking/J-chain competitionの陽性対照。
2. `413D12 conjugated`: FACSでのFcRL4染色対照。
3. `A1`または`580810`: 413D12とは別エピトープ候補の市販anti-FcRL4対照。
4. anti-FCRL5 `509F6`など: FCRL5交差反応を潰すための必須対照。
5. FCRL1/2/3/4/5/6単独発現細胞: 抗体そのものより重要な特異性判定パネル。

### 注意

BioLegendなどの市販RUO抗体は、通常、研究使用に限定され、商用利用、再販、製造利用、reverse engineering、sequencingなどが制限される場合がある。創薬seedの配列・抗体本体として使うのではなく、あくまでbinding/competition assayの実験対照として使う位置づけに留める。

## 論文別メモ

### 1. Ehrhardt et al. 2005: `2A6` anti-FcRH4/FcRL4

文献: Ehrhardt et al. `Expression of the immunoregulatory molecule FcRH4 defines a distinctive tissue-based population of memory B cells.` Journal of Experimental Medicine, 2005. [PMC2212938](https://pmc.ncbi.nlm.nih.gov/articles/PMC2212938/), [PubMed](https://pubmed.ncbi.nlm.nih.gov/16157685/), DOI: [10.1084/jem.20050879](https://doi.org/10.1084/jem.20050879)

#### 取得方法

- 免疫原: baculovirus由来のFcRH4/FcRL4 extracellular domain組換えタンパク質。
- 宿主/方法: マウスをhyperimmunizationし、リンパ節細胞をAg8-653 myeloma variantと融合。
- スクリーニング: 120 hybridoma clone中34 cloneがFcRH4 ECD ELISA陽性、3 cloneが扁桃B細胞サブセットに反応。
- 選抜クローン: `2A6`。ELISA、Western blot、FACS、免疫沈降で検証。
- 使い方: FcRH4+ memory B cellの同定、F(ab')2 fragment化、biotin/Alexa647標識。

#### IgA J-chainとの競合性

- 論文内でIgA結合やJ-chain-linked IgAとの競合は評価されていない。
- 2005年時点ではFcRL4のJ-chain依存IgA受容体機能は未確立であり、`2A6`はリガンドブロック抗体として選別されていない。
- したがって、`2A6`がJ-chain結合面を塞ぐかは不明。

#### ファミリータンパク質との特異性

- 当初論文では、FcRH4 transfectantの選択的染色、recombinant FcRH proteinのIP/WB、FcRH1/2/3/5発現B細胞株への非反応性を根拠にFcRH4特異的と解釈された。
- ただし、本文内でも長時間露光でHA-FcRH5の弱いバンドが見える可能性に触れている。
- 後年のObeng-Adjei et al. 2015では、`2A6`がFCRL4発現細胞だけでなくFCRL5発現細胞にも強く結合することが示された。

#### 開発への示唆

- `2A6`はFcRL4抗体作製の歴史上重要だが、創薬のstarting cloneや患者選択抗体としては危険。
- FcRL4標的B細胞を議論する時、古い2A6ベースのFACSデータはFCRL5混入を疑って読む必要がある。

### 2. Polson et al. 2006: `1A3` anti-FcRH4/IRTA1

文献: Polson et al. `Expression pattern of the human FcRH/IRTA receptors in normal tissue and in B-chronic lymphocytic leukemia.` International Immunology, 2006. [Oxford Academic](https://academic.oup.com/intimm/article/18/9/1363/711889), [PubMed](https://pubmed.ncbi.nlm.nih.gov/16849395/), DOI: [10.1093/intimm/dxl069](https://doi.org/10.1093/intimm/dxl069)

#### 取得方法

- 免疫原: FcRH/IRTA family各メンバーのHis-tag付きECDをCHO細胞に一過性発現させ、Ni columnで精製。
- 宿主: Balb/c mouseまたはXenomouse。
- 免疫: recombinant His-tag ECD protein + Ribi adjuvantでhyperimmunization。
- スクリーニング:
  - direct ELISAで免疫原への抗体価を確認。
  - SVT2 mouse fibroblastにgD-tagまたはuntagged FcRH/IRTAを安定発現させ、FACSで目的FcRH/IRTAへの結合を確認。
  - FcRH1-5/IRTA1-5間のcross-reactivityを評価。
- FcRL4関連クローン: anti-FcRH4/IRTA1 `1A3`、mouse IgG2a。

#### IgA J-chainとの競合性

- 2006年論文では、`1A3`のIgA、dimeric IgA、J-chain-linked IgA、secretory componentとの競合性は評価されていない。
- 著者らはsoluble monomer Igの高親和性リガンド性には否定的で、Ig complex/低親和性相互作用の可能性を残している段階。
- したがって、`1A3`がJ-chain interfaceを塞ぐかは不明。

#### ファミリータンパク質との特異性

- 1A3はFcRH1-5/IRTA1-5を個別に発現する安定細胞株を用いて特異性/交差反応を確認して選ばれている。
- Obeng-Adjei et al. 2015でも、`1A3`はFCRL4発現細胞に特異的で、FCRL5発現細胞には結合しないと再確認された。
- そのため、2A6よりもFcRL4/FcRL5識別の信頼性は高い。

#### 開発への示唆

- `1A3`は「FcRL4を特異的に染める」ための比較的よい陽性対照。
- ただし、創薬抗体としては、エピトープ、親和性、内在化、BCR抑制への影響、dIgA-J競合性が不明。
- 新規抗体取得時には、`1A3`と同じbinを避ける/狙うのどちらがよいかを、FCRL4+ B cell上での機能で決めるべき。

### 3. Wilson et al. 2012: `413D12` blocking anti-FcRL4 と `418C8` non-blocking anti-FcRL4

文献: Wilson et al. `Human FcRL4 and FcRL5 are receptors for IgA and IgG.` Journal of Immunology, 2012. [PMC3634363](https://pmc.ncbi.nlm.nih.gov/articles/PMC3634363/), [PubMed](https://pubmed.ncbi.nlm.nih.gov/22491254/), DOI: [10.4049/jimmunol.1102651](https://doi.org/10.4049/jimmunol.1102651)

#### 取得方法

- 免疫原: FcRL4またはFcRL5を安定発現するmouse P815細胞。paraformaldehyde固定細胞を使用。
- 宿主/免疫:
  - Balb/c mouse。
  - 初回CFA、以後IFA + CpG 1826で2週間間隔、最終免疫は照射細胞をIP投与。
  - SP2/0細胞と融合してhybridoma化。
- スクリーニング:
  - FcRL4/FcRL5発現P815細胞を染め、親P815を染めないクローンをFACSで選抜。
  - FcRL4では、FcRL4発現P815と非発現P815の1:1混合系でanti-FcRL4抗体をpreincubationし、CFSE標識heat-aggregated colostral IgA結合の阻害を評価。
- 選抜クローン:
  - `413D12` IgG2b: FcRL4へのIgA結合をブロック。
  - `418C8` IgG2b: isotype-matched anti-FcRL4だがIgA結合をブロックしない。

#### IgA J-chainとの競合性

- 直接データ: `413D12`はheat-aggregated IgAのFcRL4結合をブロックする。`418C8`はブロックしない。
- 直接未評価: J-chain-linked systemic IgA、recombinant IgA1-J、単離J-chain、2026年構造で示されたFcRL4-dIgA coreとの競合は評価されていない。
- 推論: Liu et al. 2020とSu/Wang/Xiao et al. 2026により、FcRL4の生理的IgAリガンドはJ-chain-containing systemic/dimeric IgAで、FcRL4は主にJ-chainを認識することが示された。したがって、`413D12`はJ-chain interfaceそのもの、またはその近傍を立体的に塞ぐ可能性が高い。ただしこれは推論であり、エピトープマッピングなしに断定できない。

#### ファミリータンパク質との特異性

- Wilson 2012では、選択された抗体が他のFcRLタンパク質への交差反応を調べられ、`413D12`は少なくともFCRL5とは交差しないと記載されている。
- ただし、論文で明示的に深く示されているのは主にFCRL4/FCRL5の相互非交差であり、FCRL1/2/3/6を含む完全な創薬水準のcross-reactivity panelとは別物として扱うべき。

#### 開発への示唆

- `413D12`はFcRL4-J-chain/dIgA blocking antibodyを作る場合の最重要benchmark。
- `418C8`はnon-blocking抗FcRL4抗体として、FcRL4細胞表面結合だけで枯渇/ADC/engagerを作る設計の対照になる。
- ただし治療抗体化には、ヒト化、親和性、エピトープ、FcRL1-6/FCRLA/B近縁性、正常MALT B cellへの影響、dIgA-J結合下での抗体アクセス性を再検証する必要がある。

### 4. Falini et al. 2003: `M-IRTA1` 病理用anti-IRTA1/FcRL4

文献: Falini et al. `Expression of the IRTA1 receptor identifies intraepithelial and subepithelial marginal zone B cells of the mucosa-associated lymphoid tissue (MALT).` Blood, 2003. [ScienceDirect Open archive](https://www.sciencedirect.com/science/article/pii/S0006497120503728), [PubMed](https://pubmed.ncbi.nlm.nih.gov/12881317/), DOI: [10.1182/blood-2003-03-0750](https://doi.org/10.1182/blood-2003-03-0750)

#### 取得方法

- 目的: IRTA1/FcRL4タンパク質の組織分布をIHCで調べるための特異抗体作製。
- 抗体: mouse monoclonal `M-IRTA1` と rabbit polyclonal anti-IRTA1。
- 免疫原: IRTA1/FcRL4の細胞外部分および細胞内部分に対応する組換えタンパク質。`M-IRTA1`は細胞外部分を認識するmAbとして使われている。
- 検証:
  - IRTA1 extracellular portion (amino acids 102-373)を発現するCOS細胞lysateで約50 kDa bandを検出。
  - M-IRTA1でIPし、anti-HAで検出。
  - empty vectorやIRTA2-5 cDNA transfectantではバンドなし。
  - FFPE組織でMALTの上皮内/上皮下B細胞とMALT lymphomaのlymphoepithelial lesion関与腫瘍細胞を染色。

#### IgA J-chainとの競合性

- 評価なし。
- 2003年時点ではFcRL4のIgA/J-chain受容体機能は未確立。
- 免疫原領域がaa102-373とされるため、J-chain interfaceの一部を含むかどうかは構造上の照合が必要。現時点では競合性不明。

#### ファミリータンパク質との特異性

- IRTA2-5 transfectantでは検出バンドなしと報告されており、病理抗体としてのファミリー特異性は一定程度支持される。
- ただし、現代の創薬で要求される全FcRL family、primary immune cell、glycoform、high-sensitivity binding assayでの網羅検証とは別。

#### 開発への示唆

- `M-IRTA1`はFFPE/IHC病理評価には価値がある。
- FcRL4+病変ニッチのpatient selection assayを作る場合、`M-IRTA1`系の知見は参考になる。
- ただし、治療抗体設計に使うには、細胞表面native FcRL4への結合、competition、internalization、Fc機能との相性を再評価する必要がある。

## J-chain競合性をどう読み替えるか

関連文献:

- Wilson et al. 2012: FcRL4はheat-aggregated IgAに結合し、`413D12`でブロックされる。
- Liu et al. `FCRL4 Is an Fc Receptor for Systemic IgA, but Not Mucosal Secretory IgA.` Journal of Immunology, 2020. [PubMed](https://pubmed.ncbi.nlm.nih.gov/32513851/), [Oxford Academic](https://academic.oup.com/jimmunol/article-abstract/205/2/533/7930732), DOI: [10.4049/jimmunol.2000293](https://doi.org/10.4049/jimmunol.2000293)
- Su/Wang/Xiao et al. `FcRL4 is an IgA receptor that primarily binds the joining chain.` PNAS, 2026. [PubMed](https://pubmed.ncbi.nlm.nih.gov/42308047/), [PNAS DOI](https://doi.org/10.1073/pnas.2600183123), [RCSB PDB 9MBZ](https://www.rcsb.org/structure/9MBZ)

### 事実

- FcRL4はJ-chain-linked systemic IgAを認識し、mucosal secretory IgAは認識しにくい。
- secretory componentはFcRL4とJ-chain-linked IgAの結合を阻害する。
- 2026年PNAS/PDB 9MBZでは、FcRL4-dIgA core構造から、FcRL4が主にJ-chainを認識することが示されている。
- `413D12`は古いheat-aggregated IgA結合アッセイではblocking mAbである。

### 推論

- `413D12`は、FcRL4のJ-chain/dIgA結合面またはその近傍に結合する可能性が高い。
- ただし、heat-aggregated IgA blockingは「J-chainそのものとの競合」を意味しない。IgA複合体の立体障害、Fc部分、FcRL4の構造変化を介した阻害でも説明できる。
- 新規抗FcRL4抗体では、`413D12-like blocking` と `418C8-like non-blocking` を明確にbinningし、どちらの薬理を狙うのか分けるべき。

## FcRLファミリー特異性から見た教訓

| 論点 | 重要性 | 根拠 | 開発時の対応 |
|---|---|---|---|
| FCRL4とFCRL5の交差反応 | 非常に高い | `2A6`は当初FCRL4特異的とされたが、後年FCRL5にも強く結合 | FCRL5陰性選択を必須にする。FCRL4/FCRL5共発現細胞ではなく単独発現細胞で評価 |
| recombinant ECDだけでは不十分 | 高い | 2A6はrecombinant ECD/一部細胞株では特異的に見えた | native full-length cell display、primary B cell、glycoform違いで再確認 |
| fixed-cell免疫はnative epitopeを拾いやすい可能性 | 中 | 413D12はP815-FcRL4細胞免疫でblocking cloneを取得 | ligand-binding epitopeを狙うなら細胞免疫/膜タンパク質提示は有利かもしれない |
| FFPE/IHC抗体と治療抗体は別物 | 高い | M-IRTA1は病理で強いがfresh cellへの反応は限定的との記載あり | 患者選択IHC用抗体と治療用抗体を分けて開発する |
| J-chain競合は専用screenが必要 | 非常に高い | 既存作製論文の多くはJ-chain発見前 | fluorescent dIgA-J、secretory component competition、PDB 9MBZ-based mutagenesisを入れる |

## FcRL4抗体開発で最初に組むべき評価系

### 取得screen

1. ヒトFCRL4 full-lengthを安定発現する細胞を作り、native conformationに対するbindersを取る。
2. FCRL1、FCRL2、FCRL3、FCRL5、FCRL6単独発現細胞でnegative selectionする。
3. `413D12`を最優先reference antibodyとして同時に走らせる。
4. 入手できる場合のみ`1A3`、`418C8`、`2A6`を追加する。入手できない場合は、市販`A1`、`580810`、anti-FCRL5 `509F6`を実務上の代替referenceにする。
5. primary tonsil/pSS salivary gland由来FcRL4+ B cellで染色できるかを見る。ただし検体入手性は不明。

### J-chain/dIgA競合screen

1. recombinant IgA1-JまたはdIgA coreを蛍光標識して、FCRL4発現細胞への結合を測定。
2. secretory componentを陽性阻害対照にする。
3. `413D12`をblocking陽性対照、`418C8`をnon-blocking対照にする。
4. 競合結果を、PDB 9MBZのFcRL4-J-chain interface変異体で確認する。

### 機能screen

1. FcRL4+BCR+細胞でBCR刺激時のSyk/PLCγ2/Ca flux/CD69を測る。
2. blocking抗体がIgA-JによるFcRL4占有を外してBCR応答を戻すのか、逆にFcRL4をclusterして抑制を強めるのかを分ける。
3. Fc-enhanced設計ならADCC/ADCP、Fc-silent設計なら純粋なreceptor pharmacology、ADCならinternalizationを測る。

## 今の創薬仮説への反映

### 抗FcRL4単独抗体

- `413D12-like blocking`を狙う場合:
  - 意義: FcRL4-IgA-J axisを遮断し、FcRL4+B cellの慢性抑制/ニッチ滞在/IgA複合体依存状態を変える可能性。
  - リスク: FcRL4はIgAやIgA immune complexを内在化しないという2026年報告があり、ADCには不利な可能性。
  - kill criteria: dIgA-J competitionが弱い、FcRL4+ primary B cellで機能変化がない、FCRL5交差反応が残る。

- `418C8-like non-blocking`を狙う場合:
  - 意義: J-chain結合を邪魔せず、Fc effectorやT cell engager/ADCのターゲティング腕としてFcRL4+細胞に結合できる。
  - リスク: ligand-occupied FcRL4上でも抗体が結合できるか不明。
  - kill criteria: dIgA-J存在下で結合が落ちる、病変FcRL4+ B cell上の抗原密度が低い、正常MALT B cell毒性が許容できない。

### FcRL4 x CD22 / FcRL4 x CD3 への示唆

- FcRL4 armは、`J-chain blocking arm` と `non-blocking targeting arm` を別設計として比較すべき。
- FcRL4 x CD22でCD22 agonismを狙う場合、J-chainを置換/阻害するとFcRL4 biologyを大きく変える可能性がある。CD22共刺激が主目的なら、non-blocking FcRL4 armの方が設計仮説が明瞭かもしれない。
- FcRL4 x CD3でT cell engagerを狙う場合、病変局所FcRL4+ B cell上でJ-chain/dIgAが占有していても結合できるarmが必要。`413D12-like`より`418C8-like`または別binのnon-blocking armが有利な可能性がある。

## 不明点

| 論点 | 状態 |
|---|---|
| `1A3`、`2A6`、`M-IRTA1`、`418C8`のJ-chain-linked IgAに対する直接競合性 | 不明 |
| `413D12`がJ-chain interfaceを直接認識するか | 不明。heat-aggregated IgA blockingからの推論に留まる |
| 既存クローンの可変領域配列 | 論文本文からは不明 |
| `413D12`、`418C8`、`1A3`の詳細エピトープ/bin | 不明 |
| pSS唾液腺FcRL4+ B cell上で、IgA-J占有下でも各抗体が結合できるか | 不明 |
| 治療用ヒト化抗FcRL4抗体/臨床開発品 | 今回の範囲では確認できず |
| `1A3`、`418C8`、`2A6`の実務的入手性 | 通常カタログ品としては未確認。MTA、発明者、企業、ATCC deposit関連ルートの問い合わせが必要 |
| `413D12`、`A1`、`580810`の可変領域配列 | 公開情報からは不明。clone名・免疫原・用途・一部機能は分かるが、VH/VL/CDR配列は確認できない |
| `A1`、`580810`の詳細エピトープ | 公開情報からは不明 |
| `A1`、`580810`のJ-chain-linked IgA競合性 | 不明。blocking referenceとしては扱わない |
| `A1`、`580810`のFCRL1-6横断特異性 | `580810`はFCRL1非交差のみvendor記載あり。`A1`を含め、FCRL2/3/5/6への非交差は自前確認が必要 |

## 参考文献

1. Ehrhardt et al. `Expression of the immunoregulatory molecule FcRH4 defines a distinctive tissue-based population of memory B cells.` Journal of Experimental Medicine, 2005. [PMC2212938](https://pmc.ncbi.nlm.nih.gov/articles/PMC2212938/), DOI: [10.1084/jem.20050879](https://doi.org/10.1084/jem.20050879)
2. Polson et al. `Expression pattern of the human FcRH/IRTA receptors in normal tissue and in B-chronic lymphocytic leukemia.` International Immunology, 2006. [Oxford Academic](https://academic.oup.com/intimm/article/18/9/1363/711889), [PubMed](https://pubmed.ncbi.nlm.nih.gov/16849395/), DOI: [10.1093/intimm/dxl069](https://doi.org/10.1093/intimm/dxl069)
3. Wilson et al. `Human FcRL4 and FcRL5 are receptors for IgA and IgG.` Journal of Immunology, 2012. [PMC3634363](https://pmc.ncbi.nlm.nih.gov/articles/PMC3634363/), [PubMed](https://pubmed.ncbi.nlm.nih.gov/22491254/), DOI: [10.4049/jimmunol.1102651](https://doi.org/10.4049/jimmunol.1102651)
4. Falini et al. `Expression of the IRTA1 receptor identifies intraepithelial and subepithelial marginal zone B cells of the mucosa-associated lymphoid tissue (MALT).` Blood, 2003. [ScienceDirect Open archive](https://www.sciencedirect.com/science/article/pii/S0006497120503728), [PubMed](https://pubmed.ncbi.nlm.nih.gov/12881317/), DOI: [10.1182/blood-2003-03-0750](https://doi.org/10.1182/blood-2003-03-0750)
5. Obeng-Adjei et al. `FCRL5 Delineates Functionally Impaired Memory B Cells Associated with Plasmodium falciparum Exposure.` PLOS Pathogens, 2015. [PMC4438005](https://pmc.ncbi.nlm.nih.gov/articles/PMC4438005/), [PubMed](https://pubmed.ncbi.nlm.nih.gov/25993340/)
6. Liu et al. `FCRL4 Is an Fc Receptor for Systemic IgA, but Not Mucosal Secretory IgA.` Journal of Immunology, 2020. [PubMed](https://pubmed.ncbi.nlm.nih.gov/32513851/), [Oxford Academic](https://academic.oup.com/jimmunol/article-abstract/205/2/533/7930732), DOI: [10.4049/jimmunol.2000293](https://doi.org/10.4049/jimmunol.2000293)
7. Su/Wang/Xiao et al. `FcRL4 is an IgA receptor that primarily binds the joining chain.` PNAS, 2026. [PubMed](https://pubmed.ncbi.nlm.nih.gov/42308047/), DOI: [10.1073/pnas.2600183123](https://doi.org/10.1073/pnas.2600183123), [RCSB PDB 9MBZ](https://www.rcsb.org/structure/9MBZ)
8. BioLegend `PE anti-human CD307d (FcRL4) clone 413D12` and related formats. [BioLegend product page](https://www.biolegend.com/Default.aspx?ID=6664&productid=5701)
9. Thermo Fisher `CD307d (FcRL4) Monoclonal Antibody (413D12), APC, eBioscience`. [Product page](https://www.thermofisher.com/antibody/product/CD307d-FcRL4-Antibody-clone-413D12-Monoclonal/17-3079-42)
10. Washington University Office of Technology Management `Mouse Hybridoma producing IgG2b Monoclonal Antibodies to Human FcRL4`, Tech ID `T-007612`. [Technology summary](https://tech.wustl.edu/tech-summary/mouse-hybridoma-producing-igg2b-monoclonal-antibodies-to-human-fcrl4/)
11. Thermo Fisher/Invitrogen `FCRL4 Monoclonal Antibody (A1)`, `MA574633`. [Product page](https://www.thermofisher.com/antibody/product/FCRL4-Antibody-clone-A1-Monoclonal/MA574633)
12. Novus Biologicals/Bio-Techne `FCRL4/FcRH4/IRTA1 Antibody (A1) - BSA Free`, `NBP3-11836`. [Product page](https://www.novusbio.com/products/fcrl4-fcrh4-irta1-antibody-a1_nbp3-11836)
13. BD Biosciences `Alexa Fluor 647 Mouse Anti-Human CD307d (FCRL4)`, clone `A1`, `566587`. [Product page](https://www.bdbiosciences.com/en-us/products/reagents/flow-cytometry-reagents/research-reagents/single-color-antibodies-ruo/alexa-fluor-647-mouse-anti-human-cd307d-fcrl4.566587)
14. R&D Systems/Bio-Techne `Human FCRL4/FcRH4 Antibody (580810)`, `MAB24262`. [Product page](https://www.rndsystems.com/products/human-fcrl4-fcrh4-antibody-580810_mab24262)
15. Thermo Fisher/Invitrogen `FCRL4 Monoclonal Antibody (580810)`, `MA5-24262`. [Product page](https://www.thermofisher.com/antibody/product/FCRL4-Antibody-clone-580810-Monoclonal/MA5-24262)
