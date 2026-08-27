# FcRL4 MoA検証に使用できる市販抗体・特許抗体の調査

作成日: 2026-08-28

対象: FcRL4陽性B細胞の除去（抗FcRL4抗体によるADCC/CDC、またはFcRL4 × CD3 TCE）

今回のスコープ: **IgA結合の阻害・競合性は選定条件に含めない。**

## 1. 結論

### 市販抗体で直ちにできること

市販抗体を使って、以下の初期MoA検証は開始できる。

- 生細胞表面のFcRL4への結合
- FcRL4発現量、標的占有率、結合依存性の確認
- 複数cloneを用いたepitope依存性の比較
- intact抗体、Fab/F(ab')2、二次抗体による架橋条件を比較したFcRL4シグナルの探索
- 抗体・TCE候補の競合flow assay用の検出抗体

優先順位は、**580810、413D12、A1**の3 cloneである。なかでも、R&D Systems/Bio-Techneの**580810（MAB24262）**はcarrier-freeの非標識抗体であり、直接標識や初期の細胞実験に最も扱いやすい。**413D12**は論文での生細胞結合実績が最も厚く、**A1**は別の免疫法で得られた独立cloneとして有用である。

### 市販抗体だけではできないこと

一方、有力な生細胞表面binding用の市販品はマウス抗体または検出用標識抗体であり、次の問いにはそのままでは答えられない。

- ヒトIgG FcによるADCC/ADCP/CDCが成立するか
- FcRL4を標的とした除去に十分な抗原密度があるか
- FcRL4 × CD3 TCEとして選択的なT細胞依存性殺傷が成立するか
- Fc形式を除いたFab結合だけでFcRL4シグナルが変わるか

したがって、市販抗体は**標的結合・発現・受容体シグナルを確認するreference binder**としては使えるが、**治療抗体の完成したsurrogateではない**。

### 特許抗体を含めた最も実用的な経路

治療形式へ組み替えるための入口としては、Genentechの**1A3（1A3.1.1、ATCC PTA-6339）**が最も有望である。生細胞表面FcRL4への結合とFcRL1–5発現細胞を用いた選択性評価の履歴があり、後続論文でもFcRL4特異性が支持されている。ただし、公開特許には**1A3のVH/VL配列が記載されていない**。寄託hybridomaの入手、権利者との契約、または別途sequencingが必要である。

現時点で、公開配列とFcRL4依存性の機能データを併せ持つ「そのまま合成できる抗FcRL4抗体」や、公開されたFcRL4 × CD3 TCEは確認できなかった。

## 2. 市販抗体の比較

| clone / 製品 | 形式・入手性 | 生細胞表面結合 | MoA検証での推奨用途 | 主な限界 |
|---|---|---:|---|---|
| **580810** / R&D Systems MAB24262 | mouse IgG1、unconjugated、carrier-free | あり。RPMI 8226 flow data | 最優先。直接標識、発現量、標的占有、競合flow、epitope比較 | 免疫原はrecombinant ECD。FcRL1との非交差のみが示され、FcRL2/3/5/6は未評価。ヒトADCC/CDCには使えない |
| **413D12** / BioLegend 340202 | mouse IgG2b、purified、100 µg | あり。FcRL4発現P815および扁桃B細胞で論文実績 | 最も文献実績のあるreference。発現、占有、受容体架橋screen | BSA・sodium azideを含むため生細胞機能試験前にbuffer exchangeが必要。VH/VL非公開。マウスFc |
| **413D12** / Thermo Fisher 17-3079-42、46-3079-42 | APCまたはPerCP-eFluor標識、mouse IgG2b | あり | 検出・gating、非標識候補抗体の競合 assay | 標識済みであり、機能抗体やTCE構築には不向き |
| **A1** / Thermo Fisher MA574633 | mouse IgG2a kappa、unconjugated、100 µg | あり。flow validated | 580810/413D12とは独立した第3のbinding clone、epitope binning、架橋screen | sodium azideを含むためbuffer exchangeが必要。公開機能データとVH/VL配列がない。マウスFc |
| **A1** / BD 566587 | Alexa Fluor 647標識、mouse IgG2a kappa | あり | 検出・gating | BSA・azide含有、標識済み。機能検証用ではない |
| **3I6** / Creative Diagnostics CABT-BL1507 | APC標識、mouse IgG2b、inquiry品 | vendor上はFC対応 | 主要3 cloneで不足した場合の探索候補 | 独立した論文検証、非標識品、family panelデータが乏しい。広い動物種反応性の主張も要確認 |
| **EPR21961** / Abcam ab239754 | recombinant rabbit mAb、BSA/azide-free | 未確認 | FFPE組織IHC | IHC-P中心で、生細胞表面binderとしての根拠がない |
| **QM005** / Quartett | mouse mAb | 未確認 | 病理IHC | 生細胞MoA用ではない |

### 市販品の選び方

初回購入は、以下の組み合わせが合理的である。

1. **580810/MAB24262**: carrier-freeの主作業抗体
2. **413D12/340202**: 論文実績のあるreference binder
3. **A1/MA574633**: 独立cloneによる再現性・epitope依存性確認
4. **蛍光標識413D12またはA1**: 発現・占有・競合flow用

413D12とA1の非標識品はazideを含む。生細胞の長時間培養、シグナル測定、細胞傷害試験へ用いる前に、desaltingまたはbuffer exchangeを行う必要がある。413D12のBioLegend製品に含まれるBSAは、抗体の直接標識や定量にも影響し得る。

## 3. 特許・寄託hybridoma由来抗体

| clone | 入手経路・公開情報 | FcRL4特異性 | 治療形式への展開可能性 | 評価 |
|---|---|---|---|---|
| **1A3 / 1A3.1.1** | Genentech特許、hybridoma ATCC **PTA-6339** | FcRL1–5発現細胞でscreen。後続研究でもFcRL4選択性を支持 | hybridomaを入手してVH/VLを決定できれば、human IgG1、Fc-silent対照、Fc-enhanced抗体、scFv型TCEへ展開可能 | **最優先の特許抗体候補**。ただしVH/VL配列非公開、material accessと権利確認が必要 |
| **Wilson研究に対応するIgG2b hybridoma technology** | Washington University OTM、Technology T-007612。license/MTA相談 | FcRL4発現細胞を用いた生細胞screen由来 | hybridomaが提供され、clone identityを確認できればsequencing・reformat可能 | 有力な第2経路。ただしOTMページだけでは413D12/418C8等のclone内訳を確定できないため要問い合わせ |
| **4-2A6 / 2A6** | UAB特許、hybridoma ATCC **PTA-6236** | 当初FcRL4抗体として報告されたが、後続研究で**FCRL5にも強く結合** | 配列化は可能でも、FcRL4選択的depleter/TCEの出発点として不適 | **推奨しない**。family specificityのnegative lessonとしては有用 |
| **418C8** | Wilsonらの論文clone、mouse IgG2b | 生細胞FcRL4結合 | hybridoma入手時に配列化可能 | 通常カタログ品・公開配列なし。413D12より入手性が低い |
| **M-IRTA1** | Faliniらの病理用抗体 | IRTA1/FcRL4陽性組織を検出 | IHC reference | 生細胞除去MoAの検証には不向き。通常の治療抗体開発経路なし |

### 特許を読む際の注意点

- Genentech特許のFcRL4抗原配列（例: SEQ ID NO: 10）を、**1A3抗体のVH/VL配列と誤認してはいけない**。
- FcRL4 × CD3を候補標的の一つとして列挙する多重特異性抗体特許は存在するが、FcRL4結合armの配列、FcRL4依存性殺傷、選択性データがないものは「使用可能な特許抗体」には数えられない。
- 旧名の**IRTA-4はFcRL2**を指す場合がある。FcRL4の旧名はIRTA1/FcRH4/CD307dであり、「IRTA-4 antibody」という名称だけでFcRL4抗体と判断してはいけない。
- 特許の満了・放棄表示と、寄託細胞の取得条件、抗体の実施自由度は別問題である。本調査はFTOの法的意見ではない。

## 4. 既存抗体で実施できるMoA検証

### 4.1 標的結合とfamily specificity

最初に、full-length human FcRL4安定発現細胞、親細胞、FcRL1/2/3/5/6発現細胞を同一条件で比較する。580810、413D12、A1の濃度依存的結合を測定し、以下を得る。

- EC50と最大結合量
- 抗原密度の異なる細胞での結合
- FcRL family間の交差反応性
- clone間の相互競合による簡易epitope bin
- internalizationの有無と速度

特に580810はvendor data上、FcRL1非交差しか直接確認されていないため、全family panelでの確認が必要である。

### 4.2 FcRL4受容体シグナル

FcRL4によるBCR抑制は、抗FcRL4抗体を用いて確立された現象ではなく、FcRL4発現系やFcRL4細胞質領域を用いた研究が中心である。そのため、既存市販cloneを「既知のagonist」とは扱わず、3 cloneすべてをscreenする。

比較条件:

- intact mouse IgG
- FabまたはF(ab')2
- Fc-silentなF(ab')2二次抗体による制御された架橋
- 抗体なし、isotype、FcRL4陰性細胞

主なreadout:

- FcRL4のtyrosine phosphorylation
- SHP-1/SHP-2のrecruitment
- BCR刺激後のpSYK、pPLCγ2、Ca flux、pERK、NF-κB
- TLR7/9刺激後の増殖、生存、CD69/CD86、サイトカイン

これにより、「Fabの結合だけ」「FcRL4の架橋」「Fc受容体を介した見かけの作用」を分けられる。

### 4.3 ADCC/ADCP/CDC

市販のmouse IgG1/IgG2a/IgG2bで得た細胞傷害活性は、ヒト治療抗体のFc MoAを直接予測しない。Fabを同一に保ち、少なくとも次のrecombinant formatを比較する必要がある。

- human IgG1 WT
- Fc-silent control（N297AまたはLALA-PG等）
- FcγRIIIa活性を高めたformat、またはafucosylated IgG1
- CDCを重視する場合のcomplement-active format

FcRL4発現細胞と親細胞を用いた標的依存性を確認した後、ヒトNK/PBMC、macrophage、ヒト補体を用いる。1A3等のhybridoma配列を取得できれば、この比較が最短経路になる。

### 4.4 FcRL4 × CD3 TCE

公開情報から、使用可能なFcRL4 arm配列とFcRL4依存性殺傷dataを持つ既製TCEは確認できなかった。したがって、次のいずれかが必要である。

1. 1A3、413D12、418C8等のhybridomaを入手してVH/VLを決定する
2. 市販抗体をreference/competition reagentとして用い、新規抗体を取得する
3. 取得binderをscFv、FabまたはIgG-like bispecificに変換し、CD3 armと組み合わせる

評価時にはFcRL4発現量の異なる標的、FcRL family発現細胞、FcRL4陰性B細胞を含め、T-cell activationとkillingのwindowを同時に確認する。

## 5. 推奨する開発順序

### Phase 0: 市販3-cloneで標的を固める

- 580810、413D12、A1を購入
- FcRL1–6発現細胞panelでfamily specificityを再確認
- FcRL4発現量、結合EC50、internalization、epitope binを取得
- pSS由来FcRL4陽性B細胞または病態を模した誘導細胞で結合を確認

### Phase 1: receptor signalingをscreenする

- intact、Fab/F(ab')2、架橋条件を比較
- BCR抑制とTLR7/9応答の変化を同じclone間で比較
- 強いagonism、antagonism、または無作用のcloneを分類

この段階は、将来のdepleterが標的細胞を殺し切れない低濃度条件で、FcRL4シグナルを望ましくない方向へ変えないかを見る意味もある。

### Phase 2: 治療formatへ進めるbinderを配列化する

- 第一候補: 1A3/PTA-6339のmaterial accessを照会
- 第二候補: Washington University T-007612の提供cloneと条件を照会
- 並行して、新規抗FcRL4抗体取得のbackupを進める

### Phase 3: 同一FabでADCC/CDCとTCEを比較する

- human IgG1 WT対Fc-silent controlでFc依存性を証明
- Fc-enhanced/afucosylated抗体でeffector活性を最適化
- 同じbinder由来のFcRL4 × CD3 TCEを作製
- FcRL4陰性細胞とFcRL family発現細胞を含め、標的依存性と安全域を比較

## 6. Go / No-goの判断

| 問い | Goの目安 | No-goまたは再設計 |
|---|---|---|
| native FcRL4へ結合するか | 2 clone以上で濃度依存的に結合 | recombinant ECDのみへの結合 |
| family specificityがあるか | FcRL1/2/3/5/6への有意結合なし | 特にFcRL5へ強く交差（2A6型） |
| 病態細胞を認識するか | pSS病態由来FcRL4+細胞で十分な占有 | transfectantでは結合するが病態細胞で弱い |
| depleterとして成立するか | FcRL4依存的ADCC/ADCP/CDC、Fc-silentで消失 | FcRL4陰性細胞も同程度に殺傷 |
| TCEとして成立するか | FcRL4依存的killingと許容可能なT-cell activation window | FcRL4低発現またはfamily交差細胞も殺傷 |
| 受容体シグナルのリスク | sub-saturating条件で病的TLR応答を増強しない | 残存細胞のTLR応答・生存を強く増強 |

## 7. 総合判断

**MoA検証を開始できる市販抗体はある。** 580810、413D12、A1を用いれば、標的結合、発現、family specificity、internalization、受容体架橋によるシグナル変化まで調べられる。

ただし、**ADCC/CDCまたはFcRL4 × CD3 TCEによる除去MoAを直接検証できる既製抗体はない。** この段階にはVH/VL配列とヒト治療formatが必要である。最も短い経路は1A3/PTA-6339またはWilson研究由来hybridomaの入手・sequencingであり、それが難しければ市販3 cloneをreferenceとして新規抗体を取得する必要がある。

IgA結合の阻害・競合性は、今回のclone順位付けおよびGo/No-go条件には含めていない。

## 8. 主要情報源

### 市販品

- [BioLegend: Purified anti-human CD307d (FcRL4), clone 413D12, 340202](https://punchproduction-biolegend.dw-demo2.com/Default.aspx?GroupID=BLG6397&ID=10059&productid=5701)
- [Thermo Fisher: CD307d/FcRL4 antibody, clone 413D12, APC](https://www.thermofisher.com/antibody/product/CD307d-FcRL4-Antibody-clone-413D12-Monoclonal/17-3079-42)
- [Thermo Fisher: FCRL4 antibody, clone A1, MA574633](https://www.thermofisher.com/antibody/product/FCRL4-Antibody-clone-A1-Monoclonal/MA574633)
- [BD Biosciences: Alexa Fluor 647 mouse anti-human CD307d/FcRL4, clone A1, 566587](https://www.bdbiosciences.com/en-us/products/reagents/flow-cytometry-reagents/research-reagents/single-color-antibodies-ruo/alexa-fluor-647-mouse-anti-human-cd307d-fcrl4.566587)
- [R&D Systems/Bio-Techne: Human FCRL4/FcRH4 antibody, clone 580810, MAB24262](https://www.rndsystems.com/products/human-fcrl4-fcrh4-antibody-580810_mab24262)
- [Creative Diagnostics: clone 3I6, CABT-BL1507](https://www.creative-diagnostics.com/FCRL4-antibody-250237-144.htm)
- [Abcam: FCRL4 antibody EPR21961, ab239754](https://www.abcam.com/en-us/products/primary-antibodies/fcrl4-antibody-epr21961-bsa-and-azide-free-ab239754)
- [Quartett: IRTA1 clone QM005](https://www.quartett.com/en/irta1-qm005)

### 特許・hybridoma

- [US7888478B2: Antibodies to FcRH4 and uses thereof（1A3/PTA-6339）](https://patents.google.com/patent/US7888478B2/en)
- [Cellosaurus: 1A3.1.1, CVCL_U720, ATCC PTA-6339](https://www.cellosaurus.org/CVCL_U720)
- [US20080131433A1: FCRL4 monoclonal antibodies and methods of treatment（4-2A6/PTA-6236）](https://patents.google.com/patent/US20080131433A1/en)
- [Washington University OTM: Mouse hybridoma producing IgG2b monoclonal antibodies to human FcRL4, T-007612](https://tech.wustl.edu/tech-summary/mouse-hybridoma-producing-igg2b-monoclonal-antibodies-to-human-fcrl4/)
- [US10584181B2: Anti-CD3 multispecific antibodies（FCRL4は候補標的としての列挙）](https://patents.google.com/patent/US10584181B2/en)

### 一次文献

- [Wilson et al., FCRL4 differentially regulates TLR-mediated responses in human B cells, 2012](https://pmc.ncbi.nlm.nih.gov/articles/PMC3634363/)
- [Obeng-Adjei et al., Malaria-induced interferon-γ drives expansion of Tbethi atypical memory B cells, 2015（1A3と2A6の交差性比較を含む）](https://pmc.ncbi.nlm.nih.gov/articles/PMC4438005/)
- [Thompson et al., An adaptable high throughput flow cytometry screen for therapeutic antibody discovery, 2018（1A3/4-2A6比較）](https://pmc.ncbi.nlm.nih.gov/articles/PMC5988966/)
- [Ehrhardt et al., Fc receptor-like 4 negatively regulates the B cell receptor signaling pathway, 2003](https://pmc.ncbi.nlm.nih.gov/articles/PMC263841/)
- [Sohn et al., FcRL4 acts as an adaptive to innate molecular switch dampening BCR signaling and enhancing TLR signaling, 2011](https://pmc.ncbi.nlm.nih.gov/articles/PMC3236118/)
