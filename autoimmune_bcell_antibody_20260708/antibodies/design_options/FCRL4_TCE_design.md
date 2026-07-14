# FcRL4 T cell engager方向性: CD3/CD8-biased reset設計

作成日: 2026-07-15

## 結論
FcRL4をベースにT cell engagerを考えるなら、主案は `FcRL4 x CD8A` ではなく、**FcRL4 x low-affinity CD3 TCE** として設計する方が現実的である。

理由は単純で、CD8AはT細胞のco-receptorであって、CD3/TCR複合体そのものではないからである。CD8AだけをFcRL4+ B細胞に近づけても、T細胞殺傷が十分に起こる保証は弱い。したがって、CD8方向性は「CD8A-only BsAb」ではなく、CD3 TCEをCD8+ cytotoxic T cell寄りに安全化する設計、またはCD8A x CD3を含むtrispecificの発展形として扱う。

現時点の最も強い提案は次である。

```text
FcRL4+病変組織B細胞を、
低親和性/条件付きCD3 armで短期resetするTCE。
CD19/CD20/BCMA TCEのような汎B細胞/形質細胞除去ではなく、
Sjögren腺内またはRA滑膜のFcRL4+ disease-state B cellに寄せる。
```

## 標的情報
| 項目 | 内容 |
|---|---|
| 標的B細胞側 | FCRL4 / Fc receptor-like protein 4, UniProt Q96PJ5 |
| T細胞側主案 | CD3Eを含むCD3/TCR複合体。CD3E UniProt P07766 |
| T細胞側補助案 | CD8A, UniProt P01732。pure engagerではなくCD8-biased化の補助として扱う |
| 想定format | Fc-silent IgG-like TCE、低親和性CD3 arm、FcRL4 avidity-biased 2+1、masked/prodrug TCE |
| 主目的 | FcRL4+病変B細胞の短期reset/限定的除去 |

## なぜ今TCEを考える価値が上がったか
2024年以降、B細胞/形質細胞をTCEで深く叩く発想が、腫瘍だけでなく自己免疫にも入ってきている。CD19 x CD3 blinatumomabは難治RAの少数例でB細胞resetと臨床改善が報告され、MGでも症例報告と試験が出始めている。BCMA x CD3も難治MGや移植desensitization文脈で探索されている。

さらに、FcRH5 x CD3のcevostamabがSLE with/without lupus nephritisでPhase Ib予定である。これはFcRL4直接競合ではないが、FCRL family x CD3 TCEを自己免疫に持ち込む隣接競合として極めて重要である。

つまり、FcRL4 TCEは時流には乗っている。ただし、TCE競争は急速に濃くなっているため、`FcRL4+組織B細胞stateに限定する` という差別化が出なければ、CD19/CD20/BCMA/FcRH5 TCEに飲み込まれる。

## 競合・先行例
| 競合/先行 | 標的/形式 | 状態 | FcRL4 TCEへの意味 |
|---|---|---|---|
| Blinatumomab in refractory RA | CD19 x CD3 | Nature Medicine 2024、6例compassionate use | 自己免疫TCEのPoC。低用量でRA活動性低下とB細胞resetが報告。 |
| Amgen master protocol | Inebilizumab / blinatumomab | SLE/RA Phase 2、NCT06570798 | 企業主導でCD19 x CD3が自己免疫へ入る。 |
| A-319 | CD19 x CD3 | active/refractory SLE Phase 1、NCT06400537 | SLEでCD19 x CD3競合。 |
| ABO2203 | mRNA encoded CD19/CD3 TCE | refractory autoimmune diseases early Phase 1、NCT06747156 | mRNA TCEという投与制御型の競合。 |
| CC312 | CD19 x CD3 x CD28 TriTE | refractory autoimmune diseases early Phase 1、NCT06888960 | TCEにcostimulationを足す方向。CRSリスクが高く、自己免疫では慎重。 |
| GB261 | CD20 x CD3 | refractory seropositive SLE Phase 1、NCT06945068 | CD20 TCEも自己免疫へ。 |
| Cizutamig | BCMA x CD3 | refractory seropositive RA Phase 1、NCT06946199 | 形質細胞寄りreset競合。 |
| GSK5926371 | CD19/CD20 TCE | B-cell driven autoimmune rheumatic diseases Phase 1、NCT07371468 | 汎B細胞TCEの企業競合。 |
| Blinatumomab in refractory MG | CD19 x CD3 | Phase 2/3予定、NCT06684184/NCT06836973 | 自己抗体神経疾患でTCE探索。 |
| Low-dose blinatumomab in autoimmune encephalitis/cerebellitis | CD19 x CD3 | Phase 4予定、NCT07686042 | 抗体介在性神経疾患にも展開。 |
| BiTE desensitization | CD19 x CD3 or BCMA x CD3 | highly sensitized kidney transplant candidates、NCT07689149 | 自己免疫以外にも深いB/PC depletionが広がる。 |
| Cevostamab | FcRH5 x CD3 | SLE/LN Phase Ib予定、NCT07629583 | FCRL family x CD3の直接隣接競合。 |

## FcRL4 TCEの設計枝
| 設計枝 | 内容 | 評価 |
|---|---|---|
| FcRL4 x low-affinity CD3 1+1 | FcRL4 arm 1価、CD3 arm 1価。CD3親和性を下げてCRSを抑える | 主案。最も素直で検証しやすい。 |
| FcRL4 2+1 x CD3 | FcRL4側を2価にしてFcRL4高発現細胞でavidityを稼ぐ。CD3は1価低親和性 | FcRL4高発現B細胞選択性を上げられる可能性。標的密度依存性を作りやすい。 |
| masked/prodrug FcRL4 x CD3 | CD3 armまたはFcRL4 armをmaskし、炎症組織proteaseなどで解除 | 安全域改善案。ただしSjögrenでmask解除条件を見つける必要。 |
| FcRL4 x CD8A x CD3 trispecific | CD8+ T細胞選択とCD3 activationを両立 | 革新的だがCMC/安全性が重い。CD8A-onlyよりは理屈が通る。 |
| FcRL4 x CD3 x CD28 | TCEにcostimulationを足す | 自己免疫では危険度が高い。初期は原則No-Go寄り。 |
| FcRL4 x CD8A pure BsAb | CD8Aだけで近接させる | 薬理成立性が弱い。探索枝に留める。 |

## 設計原則
### 1. CD3は低親和性から始める
TCEではCD3親和性が高いほどT細胞活性化とcytokine releaseが強くなりやすい。低親和性CD3は、標的細胞依存性を高め、cytokine releaseを下げる設計として複数の前臨床報告がある。FcRL4 TCEは慢性自己免疫で使う可能性があるため、がんTCEよりさらに保守的にCD3 armを弱く始めるべきである。

### 2. FcRL4側は標的密度gateにする
FcRL4は正常粘膜B細胞にも存在する可能性がある。したがって、単にFcRL4に結合するだけでは足りない。FcRL4高発現、病変組織局在、Tfh/CXCL13近接、MALT riskなどを合わせて患者選択し、分子設計でもFcRL4密度依存性を作る。

### 3. CD8A-onlyではなくCD3 TCEとして評価する
CD8Aを使うなら、CD8+ T細胞選択性やcytotoxic T cell biasを上げる補助として使う。CD8A arm単独で薬効が出るかは、低い期待値で検証する。

### 4. 投与は慢性維持ではなく短期resetで考える
CD22/FCGR2B silencerは慢性投与を考えやすい。一方、TCEは深いB細胞reset薬であり、慢性維持よりも短期投与、step-up dosing、休薬、再投与条件で考える方が安全性と差別化が立つ。

### 5. 局所炎症を薬効と毒性の両方で見る
FcRL4+ B細胞が唾液腺上皮近傍にいるなら、TCEは上皮近傍でT細胞殺傷を起こす可能性がある。これは病変B細胞resetにもなりうるが、腺組織傷害にもなりうる。salivary gland organoid/slice assayは必須である。

## FcRL4 TCEが向く患者
| 患者/病態 | 適性 | 理由 |
|---|---|---|
| Sjögren腺内FcRL4+ B細胞高値、腺腫脹、MALT risk | 高 | FcRL4標的の存在と除去の意義が最も強い。 |
| Sjögrenで乾燥のみ、不可逆腺障害中心 | 低 | TCEの強さに見合わない。 |
| Sjögren systemic-high、RF/cryoglobulin/低C4/CXCL13高値 | 中-高 | B-cell-high axisがあれば短期resetの価値がある。 |
| RA滑膜FcRL4+ B細胞高値、難治滑膜炎 | 中-高 | RAではblinatumomab先行PoCがあり、FcRL4で滑膜B細胞に寄せられる可能性。 |
| SLE/LN | 中-低 | CD19/CD20/FcRH5 TCE競合が強い。FcRL4+組織B細胞を示せないと弱い。 |
| MALT lymphoma/前リンパ腫ニッチ | 中 | 腫瘍寄り適応ならTCEの強さが許容されやすいが、自己免疫seedからは別テーマ。 |

## 既存TCEとの差別化
| 既存/競合TCE | 弱点 | FcRL4 TCEで狙う差別化 |
|---|---|---|
| CD19 x CD3 | 広範なB細胞除去、正常B細胞影響 | FcRL4+病変組織B細胞stateへ限定。 |
| CD20 x CD3 | CD20陰性plasmablast/plasma cell、広範B細胞除去 | FcRL4+組織記憶/病変B細胞を狙う。 |
| BCMA x CD3 | 形質細胞/低Ig/感染 | B細胞state側を狙い、全形質細胞除去を避ける。 |
| FcRH5 x CD3/cevostamab | FCRL family隣接競合、SLE/LNで先行 | FcRL4+粘膜/組織B細胞、Sjögren/RA滑膜へ疾患をずらす。 |
| CD19/CD20 TCE | B-cell driven autoimmune全般へ広がる | FcRL4 tissue biomarkerで患者選択を鋭くする。 |

## 安全性リスク
- CRS、発熱、IL-6/TNF/IFNγ上昇。
- ICANS様神経毒性。ただし自己免疫の低用量では未知。
- 唾液腺/粘膜の局所組織傷害。
- 正常粘膜FcRL4+ B細胞の除去による防御免疫低下。
- 低Ig、感染、ワクチン応答低下。
- T細胞疲弊、T細胞減少。
- 標的陰性B細胞/形質細胞が残り、臨床効果が不十分。
- FcRL4発現がMALT lymphoma riskと近い場合、腫瘍化前後の安全性/適応境界が難しい。

## 初期評価系
| 評価 | 実験 |
|---|---|
| 標的密度 | fresh唾液腺/RA滑膜でFcRL4 molecules/cellに相当する定量、IHC/RNAscope/flow。 |
| T細胞近接 | FcRL4+ B細胞とCD3+CD8+ T細胞、Tfh/Tph、CXCL13のspatial解析。 |
| TCE killing | autologous tissue B/T co-cultureでFcRL4+ B細胞選択的killing。 |
| cytokine window | killingが最大化し、IL-6/TNF/IFNγ/GM-CSFが許容されるCD3親和性・formatを探索。 |
| 比較対照 | CD19 x CD3、CD20 x CD3、FcRH5 x CD3、anti-FcRL4単独、FcRL4 x CD22、FcRL4 x FCGR2B。 |
| 正常組織安全性 | 扁桃、腸管/気道/口腔粘膜B細胞、血中B細胞でのkillingとcytokine。 |
| 組織傷害 | 唾液腺slice/organoidで上皮細胞死、barrier、炎症遺伝子を測る。 |
| rechallenge | 短期reset後のB細胞再構成、naive/memory/plasmablast比、自己抗体、感染関連Igを追う。 |

## Go / No-Go
| 判定 | 条件 |
|---|---|
| Go | FcRL4高発現病変B細胞で、CD19 x CD3より低いcytokineで同等以上の病変B細胞killingが出る。 |
| Go | FcRL4陰性B細胞、血中B細胞、正常粘膜B細胞への作用が明確に低い。 |
| Go | Sjögren腺内またはRA滑膜で、FcRL4+ B細胞とT細胞が近接しており、ex vivo tissue assayで炎症/Ig産生が下がる。 |
| No-Go | FcRL4密度依存性がなく、CD19/CD20 TCEと同じ広範B細胞除去になる。 |
| No-Go | killingに必要な濃度でCRS cytokineが高すぎる。 |
| No-Go | 唾液腺上皮傷害が強い。 |
| No-Go | FcRL4+ B細胞が患者群の一部にしかおらず、biomarkerで選べない。 |
| No-Go | FcRH5/CD3やCD19/CD3に対して明確な安全性/患者選択優位が出ない。 |

## 推奨度
**条件付きで中。**

FcRL4 TCEは、CD22/FCGR2B silencerより強いreset薬であり、慢性Sjögrenの標準的な患者には重い。だが、腺腫脹、MALT risk、systemic-high、RA滑膜B細胞高値など、組織B細胞を短期resetする必然性がある患者では魅力がある。

主案は `FcRL4 x low-affinity CD3`、次点は `FcRL4 2+1 x low-affinity CD3`、探索枝として `FcRL4 x CD8A x CD3 trispecific`。`FcRL4 x CD8A pure BsAb` は薬理成立性が弱いため、TCE本流からは下げる。

## 参考リンク
- CD19 x CD3 blinatumomab in refractory RA: https://pubmed.ncbi.nlm.nih.gov/38671240/
- TCE vs CAR-T in autoimmune disease review: https://pubmed.ncbi.nlm.nih.gov/38642912/
- CD19 x CD3 blinatumomab in refractory MG: https://pubmed.ncbi.nlm.nih.gov/40583272/
- BCMA x CD3 teclistamab in refractory MG: https://pubmed.ncbi.nlm.nih.gov/40534130/
- T-cell engagers beyond autoimmunity/transplant: https://pubmed.ncbi.nlm.nih.gov/42167865/
- TCE modality review 2026: https://pubmed.ncbi.nlm.nih.gov/41474966/
- CD3 affinity tuning, PSMA x CD3: https://pubmed.ncbi.nlm.nih.gov/34088740/
- CD3 affinity tuning and biodistribution: https://pubmed.ncbi.nlm.nih.gov/34257348/
- TCE protein geometry/cytokine window: https://pubmed.ncbi.nlm.nih.gov/38455046/
- Low-affinity CD3 CLDN18.2 TCE: https://pubmed.ncbi.nlm.nih.gov/40759445/
- CD3 and target affinity interdependence in 2+1 TCBs: https://pubmed.ncbi.nlm.nih.gov/41196029/
- Masked/prodrug CD3 TCE: https://pubmed.ncbi.nlm.nih.gov/38962811/
- FcRH5/CD3 synapse geometry: https://pubmed.ncbi.nlm.nih.gov/28262555/
- Cevostamab SLE/LN Phase Ib: https://clinicaltrials.gov/study/NCT07629583
- Blinatumomab autoimmune master protocol: https://clinicaltrials.gov/study/NCT06570798
- A-319 CD19 x CD3 in SLE: https://clinicaltrials.gov/study/NCT06400537
- ABO2203 mRNA CD19/CD3 TCE: https://clinicaltrials.gov/study/NCT06747156
- CC312 CD19/CD3/CD28 TriTE: https://clinicaltrials.gov/study/NCT06888960
- GB261 CD20 x CD3 in SLE: https://clinicaltrials.gov/study/NCT06945068
- Cizutamig BCMA x CD3 in RA: https://clinicaltrials.gov/study/NCT06946199
- GSK5926371 CD19/CD20 TCE in autoimmune rheumatic disease: https://clinicaltrials.gov/study/NCT07371468
