# Proposal 1 Detailed Report: CD19 x FcGR2B inhibitory bispecific

作成日: 2026-07-05

## 0. このレポートの目的

このレポートは、`outputs/seed_proposal_1.md` にまとめた「CD19 x FcGR2B inhibitory bispecific」について、基礎から理解するための補足資料である。

中心となる問いは以下である。

- なぜB細胞を「殺す」のではなく「抑える」発想なのか
- CD19とFcGR2Bを同時に狙う意味は何か
- なぜbispecific antibodyである必然性があるのか
- 最初に何を確認できれば前に進めるのか

## 1. まず超基礎: 自己免疫疾患とB細胞

自己免疫疾患では、本来は外敵を攻撃するはずの免疫が、自分の体の成分を攻撃してしまう。

このときB細胞は重要な役割を持つ。B細胞は抗体を作る細胞の前段階であり、自己免疫疾患では「自己抗体」を作る方向に進んでしまうことがある。

```text
B細胞
  ↓ 活性化
形質芽細胞
  ↓ 分化
形質細胞
  ↓
抗体を産生
```

問題は、この抗体が病原体ではなく自分の体に反応する場合である。IgG4-related disease、Sjögren disease、SLE、自己免疫性溶血性貧血、天疱瘡などでは、B細胞や自己抗体が病態に関わる。

## 2. 既存のB細胞治療の考え方

B細胞を標的にする代表的な治療は、B細胞を除去する方法である。

| 標的 | 代表的な考え方 | 特徴 |
|---|---|---|
| CD20 | B細胞除去 | rituximabなどで実績が大きい |
| CD19 | より広いB系列細胞の除去 | plasmablast寄りまで狙える可能性 |
| BAFF/BAFF-R | B細胞の生存シグナルを抑える | 比較的ゆっくり効くことが多い |
| FcRn | 病的IgGを減らす | B細胞自体は殺さない |

B細胞除去は強力である一方、慢性疾患では次の課題がある。

- 感染リスク
- 低ガンマグロブリン血症
- ワクチン応答の低下
- 効果が切れた後の再発
- 繰り返し投与による長期安全性

そこで今回の提案は、B細胞を単純に殺すのではなく、「過剰に働いているB細胞を抑制する」方向を狙う。

## 3. CD19とは何か

CD19はB細胞の表面にある膜タンパク質である。

| 項目 | 内容 |
|---|---|
| タンパク質名 | CD19 |
| UniProt ID | P15391 |
| 場所 | B細胞表面 |
| 役割 | B細胞受容体シグナルの調整 |
| 医薬品標的としての意味 | B細胞を見分ける目印になる |

CD19はCD20よりも広いB系列に出るため、plasmablastを含む病的B細胞に届きやすい可能性がある。

ただしCD19を普通に抗体で狙うと、細胞除去に寄りやすい。今回の提案では、CD19を「B細胞に抗体を連れていくための住所」として使う。

## 4. FcGR2Bとは何か

FcGR2Bは免疫細胞にある抑制性受容体である。遺伝子名は `FCGR2B`、UniProt IDは `P31994`。

かなり単純化すると、FcGR2BはB細胞に対してブレーキをかける受容体である。

```text
B細胞が活性化しようとする
  ↓
FcGR2Bが一緒に刺激される
  ↓
「行きすぎるな」という抑制シグナルが入る
```

自己免疫疾患では、B細胞のアクセルが強すぎたり、ブレーキが不十分だったりする。そこでFcGR2Bを意図的に使って、B細胞の活性化を抑えたい。

## 5. なぜCD19 x FcGR2Bのbispecificなのか

ここはこの提案の一番重要な部分である。

結論から言うと、CD19 x FcGR2B bispecificの意味は、単に「B細胞にくっつく抗体を作る」ことではない。B細胞が抗原を認識して活性化しようとする瞬間に、同じ細胞上でFcGR2Bの抑制性ITIMシグナルを同時に入れることで、BCR/CD19系のアクセルに対して人工的にブレーキを踏ませることである。

つまり、この分子は「B細胞を見つけるためのCD19抗体」と「抑制受容体を刺激するFcGR2B抗体」を足し算したものではない。CD19を含むBCR co-receptor側の活性化機構と、FcGR2Bの抑制機構を、同じB細胞膜上の近い空間でリンクさせることが薬理である。

## 5.1 まずBCR/CD19はB細胞のアクセル側である

B細胞が抗原を認識するとき、中心にあるのはBCRである。BCRは抗原を認識し、細胞内へ活性化シグナルを送る。

CD19はBCRそのものではないが、BCRシグナルを増幅するco-receptor complexの重要な構成要素である。CD19が関わると、B細胞は抗原刺激に対してより反応しやすくなる。

かなり単純化すると、以下のようになる。

```text
自己抗原または抗原
  ↓
BCRが認識
  ↓
CD19を含むco-receptorがシグナルを増幅
  ↓
Ca flux、PI3K/AKT、MAPKなどが動く
  ↓
B細胞の活性化、増殖、抗原提示、抗体産生方向への分化
```

自己免疫疾患では、このアクセルが自己抗原に対して動いてしまうことが問題になる。

## 5.2 FcGR2BはB細胞のブレーキ側である

FcGR2Bは抑制性Fc受容体であり、細胞内にITIMという抑制性モチーフを持つ。

FcGR2BがBCR活性化の近くで共架橋されると、FcGR2BのITIMがリン酸化され、SHIP1/SHIP2などの phosphatase が動員される。これにより、BCR下流のシグナルが弱まる。

抑えられる代表的な反応は以下である。

| 抑制される反応 | 意味 |
|---|---|
| Ca mobilization | BCR刺激直後の活性化シグナルが弱まる |
| B細胞増殖 | 抗原反応性B細胞の拡大が抑えられる |
| costimulatory molecule発現 | T細胞を助ける能力が落ちる |
| 抗原取り込み | BCRを介した抗原捕捉が弱まる |
| 抗原提示 | cognate T cell helpを受けにくくなる |
| plasmablast/抗体産生方向 | 自己抗体産生へ進みにくくなる可能性 |

ここで大事なのは、FcGR2Bの抑制は「どこでも適当に刺激すればよい」わけではない点である。BCR/CD19活性化複合体の近くで、同じB細胞上で、適切なタイミングと距離で入るからこそ、B細胞活性化の閾値を上げるブレーキになる。

## 5.3 CD19とFcGR2Bを同時認識する意味

CD19 x FcGR2B bispecificの意味は、次の4つに分解できる。

| 意味 | 内容 | なぜ重要か |
|---|---|---|
| 1. B細胞選択性 | CD19を使ってB-lineage細胞に局在する | FcGR2Bは他の免疫細胞にもあるため、B細胞上に作用を寄せる |
| 2. 抑制シグナルの空間制御 | 同じB細胞膜上でFcGR2BをCD19/BCR signaling domainへ近づける | ITIM/SHIP系ブレーキをBCR活性化の近くで入れられる |
| 3. 非除去型の機能抑制 | ADCC/CDCではなくB細胞機能を落とす | 慢性自己免疫で低Ig・感染リスクを下げる仮説が立つ |
| 4. T細胞依存性応答の遮断 | BCR-mediated antigen uptakeとantigen presentationを抑える | germinal center、plasmablast、自己抗体産生を上流で弱められる可能性 |

単にCD19に結合するだけなら、B細胞を見つけるだけである。単にFcGR2Bに結合するだけなら、B細胞以外にも作用しうるし、BCR活性化と同期した抑制になるとは限らない。

CD19とFcGR2Bを同時に認識することで、「病的B細胞に薬を届ける」と「そのB細胞の活性化ブレーキを入れる」を1つの分子で結びつける。

## 5.4 なぜanti-CD19とanti-FcGR2Bの併用では不十分なのか

直感的には、anti-CD19抗体とanti-FcGR2B抗体を2剤併用してもよさそうに見える。しかし、それではこの提案の薬理を再現しにくい。

理由は、必要なのが単なる同時投与ではなく、同一B細胞上でのco-engagementだからである。

| 方法 | 何が起こるか | 問題 |
|---|---|---|
| anti-CD19単独 | B細胞に結合する | 抑制性FcGR2Bシグナルを入れられない |
| anti-FcGR2B単独 | FcGR2Bに結合する | B細胞選択性が弱く、BCR/CD19活性化と空間的に結びつかない |
| anti-CD19 + anti-FcGR2B併用 | 両標的を別々に占有する | 2つの受容体を同じ膜ドメインで共架橋する保証がない |
| CD19 x FcGR2B bispecific | 1分子が両者を物理的に橋渡しする | B細胞上で抑制性co-engagementを設計できる |

このため、bispecificは「便利だから2標的にした」のではなく、FcGR2Bの抑制回路をCD19陽性B細胞に選択的に持ち込むための分子設計である。

## 5.5 既存データから見える作用機序

この考え方は、XmAb5871/obexelimab系の文献で支持されている。

2011年のXmAb5871報告では、抗CD19抗体のFcをFcγRIIb高親和性に設計し、FcγRIIbとBCR complexのcoengagementを促した。その結果、FcγRIIb ITIM phosphorylation、BCR誘導Ca mobilization低下、B細胞増殖低下、costimulatory molecule発現低下が示されている。SLE患者由来B細胞でも抑制が見られ、anti-CD20とは異なりB細胞除去を起こさない非除去型アプローチとして位置づけられた。

2026年のobexelimab関連報告では、CD19/FcγRIIb co-engagementがBCR-mediated antigen uptakeを抑え、B細胞によるT細胞への抗原提示を弱め、T細胞増殖やCD25/CD44発現を低下させた。さらに、抗原特異的germinal center応答の抑制や、開始後のGC dissolutionも示されている。

IgG4-RDのphase 2 pilotでは、obexelimabはCD19とFcγRIIbに結合する非細胞傷害性抗体として評価され、15例中12例がday 169の主要反応基準を達成した。循環B細胞とplasmablastの低下が観察された一方で、治療終了後にB細胞が比較的速く回復したことから、単純なB細胞殺傷ではなく、B細胞のsequestrationまたは機能抑制を含む作用が示唆された。

## 5.6 この提案で狙っている薬理を一言で言うと

このbispecificは、B細胞を殺す薬ではなく、抗原に反応しようとするB細胞に対して「その反応は進めるな」という抑制性文脈を人工的に与える薬である。

```text
病的B細胞が自己抗原を認識
  ↓
BCR/CD19側のアクセルが入る
  ↓
CD19 x FcGR2B bispecificが同じB細胞上でFcGR2Bを共架橋
  ↓
ITIM/SHIP系ブレーキが入る
  ↓
Ca flux、増殖、抗原取り込み、抗原提示、T細胞ヘルプ、plasmablast化が弱まる
  ↓
自己抗体・再発性B細胞応答を抑える
```

したがって、「なぜBsAbなのか」への答えは、2標的を同時に認識することがB細胞抑制シグナルの空間的・細胞選択的な発火条件そのものだからである。

## 6. 想定疾患: IgG4-related diseaseとSjögren disease

## 6.1 IgG4-related disease

IgG4-related diseaseは、複数の臓器に炎症と線維化を起こす疾患である。ステロイドが効くことは多いが、再発とステロイド毒性が問題になる。

この疾患ではplasmablastやB細胞が重要とされ、CD19標的の治療やCD19 x FcGR2B型の治療開発が進んでいる。

狙うべき患者像は以下。

- 再発を繰り返す
- ステロイド依存
- plasmablast高値
- IgG4、IgE、好酸球などが高く、活動性炎症が残る
- すでに不可逆的な線維化だけになっていない

## 6.2 Sjögren disease

Sjögren diseaseでは、唾液腺・涙腺の障害に加えて、全身病変を持つ患者がいる。B細胞活性化、自己抗体、IgG高値、CXCL13などが関わる。

ただし乾燥症状や疲労だけを主要評価にすると、薬効判定が難しい。最初はB-cell-highで全身活動性がある患者に絞る方がよい。

## 7. 既存薬との差別化

この提案の差別化は「B細胞除去ではなくB細胞抑制」である。

| 既存/競合アプローチ | 課題 | 本提案の差別化仮説 |
|---|---|---|
| CD20除去 | 強いが低IgG・感染が問題 | 除去せずに抑える |
| CD19除去 | plasmablastまで届くが抑制ではない | CD19を住所として使う |
| BAFF/BAFF-R | 生存シグナル制御で遅い可能性 | 活性化シグナルそのものを抑える |
| FcRn | IgGを下げるがB細胞は残る | B細胞側の病的活性を抑える |

ただし、obexelimabという近い考え方の薬剤がすでに開発中である。したがって、FTOと差別化は大きな論点である。

## 8. 抗体設計案

基本設計は以下。

| 設計要素 | 方針 |
|---|---|
| 分子形式 | CD19 x FcGR2B bispecific antibody |
| Fc | Fc-silent |
| 作用 | B細胞抑制、非除去 |
| 避けたい作用 | ADCC、CDC、強いサイトカイン放出 |
| 最重要パラメータ | CD19/FcGR2Bを近づける幾何、結合強度、標的密度依存性 |

「強く結合すればよい」わけではない。CD19とFcGR2Bの距離、角度、結合価数が、抑制シグナルの強さに関わる可能性がある。

## 9. 主なリスク

| リスク | 内容 |
|---|---|
| 効力不足 | B細胞を殺さないため、重症例では抑制が足りない可能性 |
| 競合 | obexelimabが先行している |
| 安全性 | FcGR2BやFc受容体まわりの予期しない免疫作用 |
| 患者選択 | B-cell-high患者をどう定義するか |
| developability | bispecificのCMC、安定性、凝集、発現量 |

## 10. 最初にやるべき検証

最初の実験は、動物モデルよりもヒト細胞を優先したい。

| 実験 | 見たいこと |
|---|---|
| IgG4-RD/Sjögren患者PBMC | 患者B細胞で本当に抑制が起きるか |
| BCR刺激アッセイ | pSYK、pBTK、Ca fluxなどが下がるか |
| plasmablast分化アッセイ | 抗体産生方向への分化を抑えるか |
| Ig産生測定 | IgG/IgG4/自己抗体が下がるか |
| ADCC/CDC確認 | 意図せず細胞を殺していないか |
| cytokine release | 免疫活性化が起きないか |

## 11. Go / No-Go

Go条件:

- 患者由来B細胞で、BCRシグナルとIg産生を明確に抑える
- 細胞除去やサイトカイン放出が目立たない
- obexelimab類似品ではない差別化点が見える
- biomarkerで対象患者を定義できる

No-Go条件:

- 抑制作用が弱い
- 効果にADCC/CDCが必要になる
- target density依存が強すぎ、実患者で効く見込みが低い
- 競合との差別化/FTOが立たない

## 12. 最終コメント

この提案は、3件の中で最も「抗体である必然性」が強い。bispecificでCD19とFcGR2Bを同じB細胞上に近づけることが薬効そのものだからである。

一方で、競合がすでに存在するため、単なる後追いでは成立しない。最初の勝負は、ヒト患者細胞で「非除去でも十分に抑えられる」ことと、「既存のCD19/FcGR2B型と違う理由」を示せるかである。

## 13. もう一段深い背景: B細胞を「消す」治療と「調律する」治療

B細胞標的治療を考えるとき、最初に整理すべきなのは、B細胞をどの程度まで消すべきかである。

自己免疫疾患では、病的B細胞だけを選択的に消せれば理想的である。しかし実際には、CD20やCD19のような汎B細胞マーカーを狙うと、正常なB細胞も一緒に影響を受ける。

このため、B細胞除去療法は強力だが、慢性疾患の維持療法としては以下のトレードオフがある。

| 項目 | B細胞除去療法の強み | B細胞除去療法の弱み |
|---|---|---|
| 効果 | 強い免疫リセットが期待できる | 病的B細胞だけでなく正常B細胞も減る |
| 発症機序への近さ | 自己抗体疾患では合理的 | 長寿命形質細胞には届きにくい場合がある |
| 安全性 | 短期では管理可能なことが多い | 感染、低Ig、ワクチン応答低下が累積する |
| 慢性投与 | 再発時に再投与できる | 繰り返すほど免疫能低下が問題になる |
| 患者心理 | 「原因細胞を消す」納得感がある | 長期の免疫低下に不安が残る |

CD19 x FcGR2Bの提案は、このトレードオフを少し変えようとするものである。

つまり、「B細胞を減らす」のではなく、「過剰に活性化したB細胞にブレーキをかける」。この発想が成立すれば、慢性自己免疫疾患において、より長く使いやすいB細胞制御薬になる可能性がある。

## 14. FcGR2Bを使うことの生物学的な意味

FcGR2Bは免疫抑制性のFc受容体である。B細胞上では、BCRシグナルに対するブレーキとして働く。

BCRはB-cell receptorの略で、B細胞が抗原を認識するための受容体である。自己免疫疾患では、自己抗原に反応するBCRを持つB細胞が問題になる。

正常な免疫制御では、BCRが刺激されても、同時に抑制性シグナルが入ればB細胞の活性化は弱まる。

```text
BCR刺激だけ:
自己抗原を認識
  ↓
B細胞活性化
  ↓
増殖・分化・抗体産生

BCR刺激 + FcGR2B刺激:
自己抗原を認識
  ↓
同時に抑制シグナル
  ↓
活性化が弱まる
```

CD19 x FcGR2B bispecificでは、CD19を使ってB細胞表面、より正確にはBCR/CD19 co-receptorの活性化文脈に分子を局在させ、同じ細胞上のFcGR2Bを共架橋する。これにより、BCR刺激時にFcGR2B ITIMがリン酸化され、SHIP系の抑制シグナルが入りやすい状態を作る。

ここで重要なのは、FcGR2Bを単独で刺激すればよいわけではない点である。FcGR2Bはさまざまな免疫細胞にも関係するため、広く刺激すると予期しない免疫抑制や免疫複合体様の作用が出る可能性がある。

CD19と組み合わせることで、「B細胞上で抑制シグナルを作る」だけでなく、「B細胞が抗原を取り込み、T細胞に提示し、germinal center/plasmablast応答へ進む流れ」を上流で弱める方向に寄せるのがこの設計の狙いである。

## 15. なぜIgG4-RDが最初の疾患候補になるのか

IgG4-related diseaseは、CD19 x FcGR2Bのような非除去型B細胞制御を試す疾患としてかなり理にかなっている。

理由は4つある。

## 15.1 ステロイド依存・再発が明確な課題である

IgG4-RDでは、ステロイドで良くなる患者が多い。しかし、減量や中止で再発することがある。長期ステロイドは糖尿病、骨粗鬆症、感染、体重増加、精神症状などの毒性が問題になる。

つまり、疾患活動性を抑えながらステロイドを減らせる薬には明確な価値がある。

## 15.2 B細胞/plasmablast biologyが見えやすい

IgG4-RDでは、plasmablastが疾患活動性と関連することがある。これは、薬効を血液中の細胞や抗体で追いやすいという意味で重要である。

自己免疫疾患の臨床試験では、何をもって効いていると判断するかが難しい。IgG4-RDでは、臓器画像や症状に加えて、plasmablast、IgG4、IgE、好酸球、補体などの指標を組み合わせやすい。

## 15.3 CD19標的の臨床妥当性がある

CD19陽性B細胞を狙う治療は、IgG4-RDで臨床的に妥当性が示されつつある。これはCD19という住所が疾患に関係する細胞集団へ届く可能性を示す。

ただし、本提案はCD19除去そのものではない。CD19を使って、FcGR2B抑制シグナルを病的B細胞に入れることが目的である。

## 15.4 非除去型であることの意味が出やすい

IgG4-RDは慢性・再発性である。したがって、一度だけ強く免疫を叩くよりも、長期に安全に疾患活動性を抑える薬の価値が出やすい。

ここで非除去型の差別化仮説が立つ。

```text
除去型:
強く効く可能性
  ↓
感染・低Ig・再投与時の懸念

非除去型:
効き方はマイルドかもしれない
  ↓
長期維持に向く可能性
```

## 16. Sjögren diseaseでの位置づけ

Sjögren diseaseは魅力的だが、臨床開発は難しい。

乾燥、疲労、疼痛は患者にとって非常に重要である一方、臨床試験ではプラセボ効果や不可逆的組織障害の影響が大きい。

そのため、CD19 x FcGR2BをSjögrenで狙う場合は、初期から「全Sjögren患者」ではなく、次のような患者に絞るべきである。

| 患者セグメント | 理由 |
|---|---|
| ESSDAI高値の全身活動性あり | 客観的な疾患活動性を追いやすい |
| 高IgG / RF陽性 / SSA陽性 | B細胞活性化が強い可能性 |
| CXCL13高値 | ectopic lymphoid structureやB細胞集積の示唆 |
| plasmablast高値 | B細胞抑制の薬効が出やすい可能性 |
| 低補体/cryoglobulinあり | B細胞・免疫複合体病態が強い可能性 |

逆に、唾液腺がすでに不可逆的に破壊されている患者では、B細胞を抑えても乾燥症状は戻りにくいかもしれない。

この点を間違えると、「標的が悪い」のではなく「患者選択が悪い」ために失敗する可能性がある。

## 17. 設計上の論点: bispecific geometry

この提案では、bispecific antibodyの形が非常に重要である。

なぜなら、CD19とFcGR2Bをただ結合すればよいわけではなく、細胞膜上で適切な距離と向きに配置する必要があるからである。

検討すべき設計要素は以下。

| 設計要素 | 論点 |
|---|---|
| CD19 arm affinity | 強すぎると標的占有は良いが内在化/分布に影響する可能性 |
| FcGR2B arm affinity | 弱すぎると抑制が入らず、強すぎると非特異的作用が懸念 |
| Valency | 1+1か2+1かで架橋・シグナルが変わる |
| Fc設計 | effector functionを消す必要がある |
| Linker/format | 距離と角度が抑制シグナルを左右する可能性 |
| Developability | 凝集、発現量、熱安定性、精製しやすさ |

初期探索では、1つの分子に賭けるよりも、複数geometryの小パネルを作り、一次ヒトB細胞で比較する方がよい。

## 18. 安全性をどう見るか

非除去型とはいえ、安全とは限らない。見落としやすい安全性論点を整理する。

| 安全性論点 | 見るべき理由 | 初期評価 |
|---|---|---|
| ADCC/CDC | 意図せずB細胞除去になると差別化が消える | NK細胞/補体存在下で細胞傷害を見る |
| Cytokine release | Fc受容体やB細胞架橋で免疫活性化が起こる可能性 | 全血/PBMC cytokine panel |
| Myeloid FcγR作用 | FcGR2B以外のFcγRに影響しないか | Fc receptor binding panel |
| Platelet/血栓 | FcγRIIAとの予期しない関係は一応見る | 血小板活性化 assay |
| 感染リスク | 長期B細胞抑制で抗体応答が弱まる | in vitro vaccine-like recall response |
| 低Ig | Ig産生抑制が強すぎると問題 | 長期培養IgG/IgM/IgA測定 |

特に重要なのは、「非除去型だから安全」という雑な説明をしないことである。安全性は、非除去であること、Fc-silentであること、cytokine releaseがないこと、正常B細胞機能を完全には潰さないことを別々に示す必要がある。

## 19. 競合に対する勝ち筋

この領域にはobexelimabが存在する。したがって、提案時には必ず「なぜ今からやるのか」と聞かれる。

まず率直に言うと、CD19 x FcGR2Bというコンセプトそのものでは、obexelimabとの差別化はほぼない。

obexelimabは、まさにCD19とFcγRIIbを同時に利用してB細胞を非細胞傷害的に抑える薬剤である。IgG4-RDではphase 3、warm AIHAではphase 3、SLEやMSでもphase 2が進んでいる。さらにIgG4-RDではCD19 depleterであるinebilizumab/Upliznaがすでに承認されている。したがって、IgG4-RDを先頭にして「CD19 x FcGR2Bで非除去型B細胞制御をします」と言うだけでは、後追いである。

勝ち筋は大きく4つしかない。

| 勝ち筋 | 内容 |
|---|---|
| Geometry差別化 | より強い抑制、より少ない活性化、より良い物性 |
| 疾患選択 | obexelimabが弱い/未開拓の患者セグメントに入る |
| Biomarker戦略 | responderをより鋭く選ぶ |
| 投与/製剤 | SC化、低頻度投与、製造しやすさ |

逆に、標的と形式が近く、疾患も同じで、バイオマーカーも同じなら、後追いになる。

この提案を進める場合、研究テーマとしては「CD19 x FcGR2Bを作る」ではなく、「obexelimab時代にまだ意味のあるCD19 x FcGR2Bを作れるか」を最初から問うべきである。

## 19.1 勝ち筋1: obexelimabより良いgeometryを作れるか

最も科学的な勝ち筋は、obexelimabとは異なるgeometryで、より良いB細胞抑制プロファイルを出すことである。

ここで言う「良い」とは、単純に結合が強いという意味ではない。

| 改良仮説 | 具体的に見るべきこと |
|---|---|
| より強いFcGR2B ITIM/SHIP engagement | ITIM phosphorylation、SHIP recruitment、Ca flux抑制がobexelimab様benchmarkを上回る |
| より少ないB細胞sequestration | 循環B細胞の急な低下ではなく、機能抑制中心にできる |
| より良いantigen uptake/presentation抑制 | BCR-mediated antigen uptake、T-cell co-cultureで優位 |
| より低いcytokine/FcγR off-target | myeloid FcγR、platelet、PBMC cytokineでクリーン |
| より良いSC developability | 高濃度製剤、低粘度、安定性、低凝集 |

ただし、これはかなり難しい。obexelimab/XmAb5871はこの領域の先行設計であり、単なるaffinity tuningでは優位性を示しにくい。

したがって、最初からobexelimab-like moleculeを社内benchmarkとして置き、それに勝てないならNo-Goにするべきである。

## 19.2 勝ち筋2: IgG4-RDを捨てる

IgG4-RDは生物学的には非常に魅力的だが、競争環境としてはもう厳しい。

理由は2つある。

1. obexelimabがIgG4-RD phase 3で先行している。
2. inebilizumab/UpliznaがIgG4-RDで承認され、CD19陽性細胞を狙う治療の標準的ポジションを取りに行っている。

つまり、IgG4-RDで新規CD19 x FcGR2Bを出すと、以下の2方向から挟まれる。

```text
強いCD19 depletion:
inebilizumab / Uplizna

非除去型CD19 x FcGR2B:
obexelimab

新規CD19 x FcGR2B:
どこで勝つのかが見えにくい
```

IgG4-RDで勝つなら、よほど明確な差が必要である。

- SC自己注射で圧倒的に使いやすい
- 感染/低Igリスクが明確に低い
- 高齢・感染リスク高い患者で特別に使いやすい
- treatment holiday後の再燃制御が優れる
- organ-threateningではなくmaintenance専用で安全性に振り切る

しかし、これは臨床・商業的には可能性があっても、初期シーズ探索としては差別化検証に時間がかかる。

したがって、研究シーズとしてはIgG4-RDをlead indicationにしない方がよい。

## 19.3 勝ち筋3: obexelimabが深く入っていない疾患/患者セグメントに絞る

次の勝ち筋は、疾患をずらすことである。

候補になりうるのは、B細胞を完全に枯らすほどではないが、BCR/T-cell dependent B-cell responseが病態維持に重要なセグメントである。

| 疾患/セグメント | 勝ち筋 | 懸念 |
|---|---|---|
| Sjögren systemic B-cell-high | B細胞活性化、CXCL13、IgG、RF、低補体などで選べる | ianalumab、dazodalibep、FcRnなど競合が多い |
| SLE B-cell/GC-high subset | BCR/T-cell help/GC signatureで選べれば理にかなう | obexelimab phase 2あり、SLE試験はノイズが大きい |
| Autoimmune cytopenia maintenance | B細胞抑制の安全性価値が出る可能性 | wAIHAはobexelimab phase 3で先行 |
| Pemphigus maintenance | rituximab後の再発予防で非除去型の意味 | FcRn/CD20が強い、自己抗体低下速度が課題 |
| Transplant/alloantibody prevention | T-cell dependent B-cell response抑制が理にかなう | 自己免疫から外れる、規制/開発設計が別物 |

ただし、obexelimabはSLE、wAIHA、MSにも展開しているため、「疾患をずらす」だけでは不十分である。疾患内の患者セグメントまで絞る必要がある。

## 19.4 勝ち筋4: biomarker-first drugにする

obexelimabとの差別化で最も現実的なのは、標的ではなく患者選択で勝つことである。

つまり、「CD19 x FcGR2Bが効きそうな患者」を先に定義し、その患者だけを狙う。

候補になるbiomarker:

| Biomarker | 意味 |
|---|---|
| BCR signaling high | BCR依存性が高い |
| CXCL13 high | GC/ectopic follicle/B-cell recruitmentの示唆 |
| plasmablast high | B細胞分化が進んでいる |
| FcGR2B expression preserved | ブレーキ受容体が残っている |
| CD19 density high | 分子が作用する足場がある |
| Tfh/GC signature high | T-cell dependent B-cell responseが動いている |
| autoantibody titer dynamic | B細胞応答が現在進行形 |

この戦略では、薬の差別化は「分子が全く新しい」ことではなく、「効く患者を見つける能力」にある。

ただし、これもobexelimab側が同じbiomarkerを使える可能性がある。したがって、単なる後付けbiomarkerでは弱い。自社分子のgeometryや薬効プロファイルと結びついたbiomarkerである必要がある。

## 19.5 勝ち筋5: 投与・製剤で勝つ

biologicで実際に大きな差になるのは、投与利便性である。

特に慢性自己免疫では、以下が重要になる。

- 皮下注射できる
- 自己注射できる
- 投与間隔が長い
- infusion reactionが少ない
- treatment holidayがしやすい
- B細胞回復が速く、感染時に戻しやすい

obexelimabがIV q2wのような投与負荷を持つなら、SC monthlyやless frequent dosingにできる分子には商業的余地がある。

しかし、これは創薬初期の勝ち筋としては弱い。なぜなら、先行品もSC化や投与最適化を進められるからである。

したがって、投与・製剤だけでGoにするのではなく、biology/geometryで少なくとも同等以上、かつ製剤で明確に優れる場合に限る。

## 19.6 現実的な結論

現時点での結論は以下である。

| 問い | 判断 |
|---|---|
| CD19 x FcGR2Bという標的組み合わせ自体に新規性はあるか | ない。obexelimabが先行している |
| IgG4-RD leadで勝てるか | かなり厳しい。obexelimabとUpliznaに挟まれる |
| 同じMoAでme-betterを狙えるか | 可能性はあるが、obexelimab-like benchmarkに勝つ実験データが必須 |
| 研究シーズとして優先すべきか | 現時点では優先度を下げるべき |
| 進める条件 | geometry、SC developability、biomarker-selected segmentのいずれかで明確な差が出ること |

したがって、proposal 1は「High推奨」ではなく、「conditional / benchmark-driven」に落とすのが妥当である。

社内での扱いとしては、以下がよい。

```text
CD19 x FcGR2Bはbiologyとしては強い。
しかしobexelimabがいるため、標的/MoAとしての新規性は低い。
進めるなら、obexelimab-like benchmarkに勝つformat差別化または疾患セグメント差別化を最初の3-6か月で示す。
示せなければNo-Go。
```

## 20. 推奨する初期研究パッケージ

## 20.1 0-3か月: ヒト生物学の確認

- IgG4-RD、Sjögren、SLEの公開データでCD19、FCGR2B、B-cell activation signatureを確認する。
- 可能なら患者血液でplasmablast、FcGR2B発現、CD19密度を測る。
- 健常人B細胞と患者B細胞でBCR刺激応答の差を見る。

## 20.2 3-6か月: 分子format探索

- 複数のbispecific geometryを設計する。
- Fc-silentの完全性を確認する。
- BCR signaling、plasmablast differentiation、Ig secretionを比較する。
- ADCC/CDC/cytokine releaseを早期に見る。

## 20.3 6-12か月: 疾患別PoC

- IgG4-RD plasmablast-highサンプルで抑制を見る。
- Sjögren B-cell-highサンプルでCXCL13/IgG/autoantibody関連指標を見る。
- ex vivoで既存B細胞標的薬との差を比較する。
- PK/PDモデルを作り、必要投与量が現実的か確認する。

## 21. 根拠文献メモ

| 論点 | 文献/情報 | この提案への意味 |
|---|---|---|
| FcγRIIbとBCR complexのcoengagementでB細胞活性化が抑えられる | Horton et al., Journal of Immunology, 2011, PMID: 21357255 | XmAb5871でFcγRIIb ITIM phosphorylation、Ca mobilization、B細胞増殖、costimulatory molecule発現、humoral immunity低下が示された |
| CD19/FcγRIIb co-engagementでT細胞依存性B細胞応答が抑えられる | Journal of Immunology, 2026, PMID: 40977622 | 抗原取り込み、抗原提示、T細胞活性化、germinal center応答まで抑えうることを支持 |
| IgG4-RDでobexelimabの臨床・PD効果が探索された | Perugino et al., Lancet Rheumatology, 2023, PMID: 38251576 | active IgG4-RDで臨床反応、B細胞/plasmablast低下、治療後回復が報告され、非除去型B細胞制御の臨床妥当性を示唆 |

注意点: これらはCD19 x FcGR2Bの機序妥当性を支えるが、自社で同じ標的を狙う場合のFTO、format差別化、疾患選択、長期安全性を保証するものではない。

## 22. 社内提案での一言

この候補は「B細胞を枯らす薬」ではなく、「病的B細胞にブレーキを戻す薬」として説明すると分かりやすい。

ただし、夢を見すぎないためには、最初から以下を明確に置くべきである。

- 非除去で本当に効くのか
- 競合との差は何か
- どの患者なら効くのか
- 安全性の優位性をどう証明するのか

この4点に答えられれば、シーズとしての説得力はかなり上がる。
