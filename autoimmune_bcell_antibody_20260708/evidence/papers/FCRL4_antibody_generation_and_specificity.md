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
3. `1A3`、`413D12`、`418C8`、`2A6`をreference antibodyとして同時に走らせる。
4. primary tonsil/pSS salivary gland由来FcRL4+ B cellで染色できるかを見る。ただし検体入手性は不明。

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

## 参考文献

1. Ehrhardt et al. `Expression of the immunoregulatory molecule FcRH4 defines a distinctive tissue-based population of memory B cells.` Journal of Experimental Medicine, 2005. [PMC2212938](https://pmc.ncbi.nlm.nih.gov/articles/PMC2212938/), DOI: [10.1084/jem.20050879](https://doi.org/10.1084/jem.20050879)
2. Polson et al. `Expression pattern of the human FcRH/IRTA receptors in normal tissue and in B-chronic lymphocytic leukemia.` International Immunology, 2006. [Oxford Academic](https://academic.oup.com/intimm/article/18/9/1363/711889), [PubMed](https://pubmed.ncbi.nlm.nih.gov/16849395/), DOI: [10.1093/intimm/dxl069](https://doi.org/10.1093/intimm/dxl069)
3. Wilson et al. `Human FcRL4 and FcRL5 are receptors for IgA and IgG.` Journal of Immunology, 2012. [PMC3634363](https://pmc.ncbi.nlm.nih.gov/articles/PMC3634363/), [PubMed](https://pubmed.ncbi.nlm.nih.gov/22491254/), DOI: [10.4049/jimmunol.1102651](https://doi.org/10.4049/jimmunol.1102651)
4. Falini et al. `Expression of the IRTA1 receptor identifies intraepithelial and subepithelial marginal zone B cells of the mucosa-associated lymphoid tissue (MALT).` Blood, 2003. [ScienceDirect Open archive](https://www.sciencedirect.com/science/article/pii/S0006497120503728), [PubMed](https://pubmed.ncbi.nlm.nih.gov/12881317/), DOI: [10.1182/blood-2003-03-0750](https://doi.org/10.1182/blood-2003-03-0750)
5. Obeng-Adjei et al. `FCRL5 Delineates Functionally Impaired Memory B Cells Associated with Plasmodium falciparum Exposure.` PLOS Pathogens, 2015. [PMC4438005](https://pmc.ncbi.nlm.nih.gov/articles/PMC4438005/), [PubMed](https://pubmed.ncbi.nlm.nih.gov/25993340/)
6. Liu et al. `FCRL4 Is an Fc Receptor for Systemic IgA, but Not Mucosal Secretory IgA.` Journal of Immunology, 2020. [PubMed](https://pubmed.ncbi.nlm.nih.gov/32513851/), [Oxford Academic](https://academic.oup.com/jimmunol/article-abstract/205/2/533/7930732), DOI: [10.4049/jimmunol.2000293](https://doi.org/10.4049/jimmunol.2000293)
7. Su/Wang/Xiao et al. `FcRL4 is an IgA receptor that primarily binds the joining chain.` PNAS, 2026. [PubMed](https://pubmed.ncbi.nlm.nih.gov/42308047/), DOI: [10.1073/pnas.2600183123](https://doi.org/10.1073/pnas.2600183123), [RCSB PDB 9MBZ](https://www.rcsb.org/structure/9MBZ)
