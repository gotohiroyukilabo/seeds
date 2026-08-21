# FcRL4構造におけるファミリー特異的ループ候補

作成日: 2026-08-21

## 一言メッセージ

FcRL4には、FCRL5やFCRL3と比べて特異性を出しやすそうなループ候補がある。特にD2の`HRRRKEK`周辺と`DENDVFRSNFKIIK`周辺は、配列差が大きくJ鎖にも接触するため、FcRL4-specificかつIgA/J鎖blocking抗体のエピトープ候補になり得る。一方、non-blocking anchorを狙うなら、J鎖接触面から離れたD3の露出ループを優先すべき。

## 結論

現時点での候補順位は以下。

| 優先 | FcRL4領域 | 位置づけ | 期待する抗体クラス | コメント |
|---:|---|---|---|---|
| 1 | D2 `124-130 HRRRKEK`周辺 | FcRL4らしいpolybasic loop | IgA/J鎖blocking、構造誘導blocking | FCRL5相同部位は`RAKAET`、FCRL3は`QGKDNK`に近く、FcRL4特異性が出しやすい。J鎖接触残基を含むためblocking寄り。 |
| 2 | D2 `172-185 DENDVFRSNFKIIK`周辺 | D2 C末端/J鎖接触ループ | IgA/J鎖blocking、413D12-like epitope候補 | FCRL5では`KESCCPVSSNTVKI`に対応し、かなり違う。J鎖接触が密で、blocking抗体候補として強い。 |
| 3 | D1-D2境界 `97-104 RLLFSSDS` | ligand-proximal junction | blockingまたはpartial blocking | FcRL5にも`FSS`様モチーフがあり、単独では特異性が弱い。周辺残基込みの立体エピトープなら可能性。 |
| 4 | D3 `250-269 TVWRENSGSYWCGAETVRGN` | ligand-distal露出面 | non-blocking anchor | `GSYWC`は保存的で危険だが、`WREN`や`GAETVRGN`周辺はFcRL4らしさがある。IgA非競合アーム候補。 |
| 5 | D3 `196-204 KATDSQPTE` | D3 N末端露出面 | non-blocking anchor | FCRL5は`RASSFQPIS`、FCRL3は`RASSSTPIE`で違う。J鎖から遠く、anchor向きだが抗体エピトープとして十分露出するかは要検証。 |
| 6 | D1 `57-66 WYHRHYWGEK` | aromatic ligand-contact ridge | blocking候補だが交差リスクあり | FcRL5が`WYHRYLGKEI`でかなり似ている。ここだけを狙うとFCRL5交差リスクが残る。 |

最も重要な判断は、`D2 124-130`と`D2 172-185`は「FcRL4特異性が高そう」だが、同時にJ鎖接触面なので、non-blocking FcRL4 x CD22のアームには向きにくい点である。これらはむしろ、IgA-blocking FcRL4抗体、またはIgA-blocking FcRL4 x CD22のbackup案に接続するのがよい。

## 解析の範囲

使った情報:

- FcRL4-dIgA/J鎖複合体構造: PDB `9MBZ`, 3.3 Å cryo-EM。
- FCRL5-IgG複合体構造: PDB `9LOC`, 3.56 Å cryo-EM。
- UniProt canonical sequences: FCRL1, FCRL2, FCRL3, FCRL4, FCRL5, FCRL6。
- FcRL4 domain annotation: UniProt Q96PJ5ではIg-like domain 1が23-97、domain 2が102-183、domain 3が193-271、domain 4が275-374。

重要な制約:

- 9MBZで実験的に見えているFcRL4は主に22-275で、D1-D3までである。D4全体は構造内で確認できないため、D4の特異的ループはこのメモでは結論しない。
- ここでの「表面露出」は、Cα近傍数と構造上の位置からの簡易判定であり、厳密なSASA計算ではない。
- Ig様ドメインのstrand/loop命名は厳密なIMGT annotationではなく、9MBZの二次構造注釈と残基接触クラスターからの実務的な呼び方である。
- 413D12/418C8の正確なエピトープは不明。候補ループとの対応は仮説である。

## 9MBZでのFcRL4-J鎖/IgA接触クラスター

9MBZ座標で、FcRL4 chain FとJ鎖またはIgA heavy chainの原子間距離が4.5 Å以下だったFcRL4残基を拾うと、主に以下のクラスターに分かれる。

| クラスター | FcRL4残基 | 接触相手 | 解釈 |
|---|---|---|---|
| D1 N末端側小ループ | K36 | J鎖 | 小さい接触点。単独エピトープとしては弱い。 |
| D1 aromatic ridge | R60, H61, Y62, W63, L82 | J鎖/IgA | ligand contactの中心の一部。ただしFCRL5にも似た配列があり、特異性は低め。 |
| D1-D2境界 | R97, L99, F100, S101, S102, D103, S104 | J鎖 | IgA/J鎖blocking抗体の候補領域。 |
| D2 polybasic loop | R125, R126, E129 | J鎖 | FcRL4特異性が高そうな最有力候補。 |
| D2 C末端/J鎖接触ループ | Y170, N174, D175, V176, F177, R178, F181, K182, I183, K185 | J鎖/IgA | もう一つの最有力候補。blocking寄り。 |

補足として、FCRL5-IgG構造9LOCでも、FCRL5 D1-D3の相同表面がIgG Fcに接触している。FCRL5ではR60、D99/S101/A103/S104/I106、C173-C174-P175-V176-S177-S178-N179、Q184-V185-Q186-E187などがIgGに近い。つまり、FCRL4とFCRL5は「同じようなIg様ドメイン面」を使って異なるIgリガンドを認識している可能性がある。抗体開発上は、この面を狙うならFCRL5への交差反応を特に厳密に見る必要がある。

## 候補ループ詳細

### 候補1: D2 polybasic loop `124-130 HRRRKEK`

FcRL4配列:

```text
122-130 RCHRRRKEK
        ^ ^  ^
        J J  J
```

9MBZでの接触:

- R125、R126、E129がJ鎖4.5 Å以内に入る。
- R127、K128も表面側に出ており、polybasic patchとして抗体から見える可能性がある。

ファミリー比較:

| タンパク質 | 相同領域の例 |
|---|---|
| FcRL4 | `RCHRRRKEK` |
| FcRL5 | `RC-RAKAET` |
| FcRL3 | `RC...QGKDNK`に近い |
| FcRL2 | `KCQGEQNWK`に近い |
| FcRL6 | `RCQGWKNTP`に近い |

評価:

- FcRL4特異性: 高い。
- J鎖blocking可能性: 高い。
- non-blocking anchor適性: 低〜中。J鎖接触面なのでIgA占有下では結合が落ちる可能性がある。
- developability懸念: polybasic patchは非特異結合、凝集、ヘパリン様分子/酸性タンパク質との相互作用リスクがある。

抗体開発への使い方:

- 413D12-like blocking antibodyの構造誘導候補。
- D2 loop swap mutantで、FcRL4 `HRRRKEK`をFCRL5-like `RAKAET`へ置換し、抗体結合とdIgA/J結合が落ちるかを確認する。
- このループを狙う抗体は、IgA競合性を最初から評価する。

### 候補2: D2 C末端/J鎖接触ループ `172-185 DENDVFRSNFKIIK`

FcRL4配列:

```text
170-185 YGDENDVFRSNFKIIK
      ^  ^^^^^ ^^^ ^
      J  JJJJJ JJJ J
```

9MBZでの接触:

- N174、D175、V176、F177、R178、F181、K182、I183、K185がJ鎖に近い。
- R178、F181はIgA heavy chainにも近い。

ファミリー比較:

| タンパク質 | 相同領域の例 |
|---|---|
| FcRL4 | `YGDENDVFRSNFKIIK` |
| FcRL5 | `YGKESCCPVSSNTVKI` |
| FcRL3 | `AYRKFYILDIEVTSK` |
| FcRL2 | D2対応は弱く、別repeatとの類似に注意 |
| FcRL6 | D2対応は弱い |

評価:

- FcRL4特異性: 高い。
- J鎖blocking可能性: 高い。
- non-blocking anchor適性: 低。リガンド接触面そのもの。
- 抗体取得可能性: 高め。表面に露出し、配列差も大きい。

抗体開発への使い方:

- IgA-blocking FcRL4抗体の本命エピトープ候補。
- 413D12がこの近傍を認識するかは不明だが、413D12と新規抗体のepitope binningで最初に見るべき。
- このループをFCRL5-like sequenceへ置換し、dIgA/J結合・413D12結合・新規抗体結合を比較する。

### 候補3: D1-D2境界 `97-104 RLLFSSDS`

FcRL4配列:

```text
92-104 RSNPVRLLFSSDS
      ^ ^^*****
      J JJ JJJ
```

9MBZでの接触:

- R97、L99、F100、S101、S102、D103、S104がJ鎖に近い。

ファミリー比較:

| タンパク質 | 相同/近傍領域 |
|---|---|
| FcRL4 | `RSNPVRLLFSSDS` |
| FcRL5 | `LSSPVHLDFSSAS` |
| FcRL3 | `LSDAVHVEFSPD` |
| FcRL2 | `LWDKTSNIVKI...` |

評価:

- FcRL4特異性: 中。
- J鎖blocking可能性: 中〜高。
- FCRL5交差リスク: 中。`FSS`周辺が似ている。
- 抗体エピトープとしては、単独短ループではなくD1-D2の立体境界として狙う必要がある。

抗体開発への使い方:

- 413D12-like blocking epitope候補の一つ。
- D1-D2境界は構造依存性が高いので、短い線状ペプチド免疫ではなく、D1-D2 folded antigenまたは全長ECDで取得する。

### 候補4: D3 distal loop `250-269 TVWRENSGSYWCGAETVRGN`

FcRL4配列:

```text
250-269 TVWRENSGSYWCGAETVRGN
```

9MBZでの位置:

- J鎖/IgAから20 Å以上離れたligand-distal側。
- D3の表面露出領域に見える。

ファミリー比較:

| タンパク質 | 相同領域の例 |
|---|---|
| FcRL4 | `TVWRENSGSYWCGAETVRGN` |
| FcRL5 | `AMWSKDSGFYWCKAAT...` |
| FcRL3 | `AMWTEDSGSYWCEVETV` |
| FcRL2 | `AVWSEDTGSYWCKAETV` |

評価:

- FcRL4特異性: 中。`GSYWC`は保存的で、フランキング残基を含めて初めて特異性が出る。
- J鎖blocking可能性: 低。
- non-blocking anchor適性: 中〜高。
- FCRL5交差リスク: 中。FCRL5のD3遠位側は9LOCでIgGに近い残基もあるため、交差反応とFcRL5機能阻害を確認する。

抗体開発への使い方:

- non-blocking FcRL4 x CD22のアーム候補。
- 抗体は`GSYWC`保存コアだけでなく、FcRL4特異的な`WREN`、`GAETVRGN`側を含む立体エピトープへ寄せる。
- FcRL3/FcRL5発現細胞でのカウンタースクリーニングを強める。

### 候補5: D3 N末端露出面 `196-204 KATDSQPTE`

FcRL4配列:

```text
196-204 KATDSQPTE
```

9MBZでの位置:

- J鎖/IgAから遠い。
- 近傍Cα数が低く、表面露出している可能性がある。

ファミリー比較:

| タンパク質 | 相同領域の例 |
|---|---|
| FcRL4 | `KATDSQPTE` |
| FcRL5 | `RASSFQPIS` |
| FcRL3 | `RASSSTPIE` |
| FcRL2 | `TASSFQPIE` |
| FcRL6 | `SAIPSEPRE` |

評価:

- FcRL4特異性: 中。
- J鎖blocking可能性: 低。
- non-blocking anchor適性: 中。
- 懸念: loop単独が十分な抗体エピトープ面積を持つか不明。

抗体開発への使い方:

- non-blocking anchor探索時の候補。
- D3単独抗原またはD2-D3抗原で、この領域を含む抗体を拾えるか確認する。

### 候補6: D1 aromatic ridge `57-66 WYHRHYWGEK`

FcRL4配列:

```text
57-66 WYHRHYWGEK
```

9MBZでの接触:

- R60、H61、Y62、W63がJ鎖/IgAに近い。

ファミリー比較:

| タンパク質 | 相同領域の例 |
|---|---|
| FcRL4 | `WYHRHYWGEK` |
| FcRL5 | `WYHRYLGKEI` |
| FcRL3 | `WY--H--DEK` |

評価:

- J鎖blocking可能性: 高。
- FcRL4特異性: 低〜中。FCRL5とかなり似る。
- 抗体開発での優先度: 低め。ここだけを狙うとFCRL5交差反応リスクが高い。

抗体開発への使い方:

- 単独エピトープとしては避ける。
- D1-D2境界やD2 loopと連続した立体エピトープの一部として拾うなら検討可能。

## 抗体設計への含意

### IgA-blocking抗体を狙うなら

優先するループ:

1. D2 `HRRRKEK`周辺。
2. D2 `DENDVFRSNFKIIK`周辺。
3. D1-D2境界 `RLLFSSDS`。

設計仮説:

- 413D12-like抗体は、これらのJ鎖接触ループのどこか、または複数をまたぐ可能性がある。
- 2026年構造を使えば、単なるrandom screeningではなく、J鎖接触面に寄せたepitope binningができる。
- IgA-blocking FcRL4 x CD22では、blockingによりFcRL4内因性ブレーキを外すリスクをCD22 agonismで補うという設計が可能。

Kill criteria:

- blocking抗体がnative dIgA/J結合を阻害しない。
- blockingによりBCR/TLR9応答が増え、CD22併用でも抑えられない。
- FCRL5にも実用濃度で結合する。

### non-blocking anchorを狙うなら

優先するループ:

1. D3 `TVWRENSGSYWCGAETVRGN`のFcRL4特異的フランキング領域。
2. D3 `KATDSQPTE`。
3. D3 `DTPLHFNFFRDGEVILSDW`のうち、保存的`FRD/GW`コアを避けた部分。

設計仮説:

- D1/D2のJ鎖接触面を避け、D3 ligand-distal面を狙うことで、内因性IgA占有下でもFcRL4+細胞に結合しやすくなる。
- FcRL4 x CD22主案では、こちらの方が合理的。

Kill criteria:

- dIgA/J存在下で抗体結合が低下する。
- FCRL3/FCRL5に交差反応する。
- pSS唾液腺またはRA滑膜のFcRL4+CD22+細胞を染められない。

## 推奨する実験

| 優先 | 実験 | 目的 | Go基準 | No-Go基準 |
|---:|---|---|---|---|
| 1 | FcRL4/FCRL5/FCRL3全長発現細胞パネルで413D12/418C8/新規抗体を比較 | 交差反応と既存cloneの位置づけ | FcRL4選択的に結合 | FCRL5またはFCRL3へ実用濃度で結合 |
| 2 | D2 `HRRRKEK` loop swap | 最有力ループの寄与確認 | swapでdIgA/J結合またはblocking抗体結合が落ちる | 変化なし |
| 3 | D2 `DENDVFRSNFKIIK` loop swap | D2 C末端ループの寄与確認 | swapで413D12-like抗体またはdIgA/J結合が落ちる | 変化なし |
| 4 | D3 distal loop swap | non-blocking anchor候補の確認 | non-blocking抗体結合だけが落ち、dIgA/J結合は残る | dIgA/J結合も落ちる、または抗体が結合しない |
| 5 | dIgA/J存在下での抗体結合 | IgA占有下で使えるか確認 | anchor抗体は結合維持、blocking抗体は競合性を示す | すべての抗体がIgA占有で結合喪失 |
| 6 | pSS唾液腺/RA滑膜切片でIHC/IF | 病変組織での実用性確認 | FcRL4+CD22+病変B細胞を低背景で染色 | 背景染色または目的細胞染色不足 |

## 開発上のまとめ

FcRL4のファミリー特異的ループは「ある」と考えてよい。ただし、目的によって狙う場所を変えるべき。

- IgA/J鎖blocking抗体: D2 `HRRRKEK`、D2 `DENDVFRSNFKIIK`が強い。
- non-blocking FcRL4 x CD22 anchor: D3 distal側がよい。
- D1 aromatic ridgeはJ鎖接触として重要だが、FCRL5に似ているため単独エピトープとしては優先しない。
- D4は9MBZで未解決のため不明。AlphaFoldなどで候補は出せるが、治療抗体エピトープとしては実験構造または抗体結合データが必要。

この整理により、抗FcRL4抗体開発は「ファミリー相同性が高いから難しい」で止めず、構造に基づいて2つの抗体探索キャンペーンに分けられる。

1. `D2 ligand-interface campaign`: 413D12-like blocking抗体、IgA-blocking FcRL4 x CD22 backup用。
2. `D3 ligand-distal campaign`: non-blocking FcRL4 x CD22/CD3 anchor用。

## 参考文献・データ

| 論点 | 文献・リンク | メモ |
|---|---|---|
| FcRL4-dIgA/J鎖構造 | RCSB PDB [9MBZ](https://www.rcsb.org/structure/9MBZ), PDB DOI [10.2210/pdb9MBZ/pdb](https://doi.org/10.2210/pdb9MBZ/pdb) | human FcRL4 bound to IgA-Fc/J。2026-06-10 released、3.3 Å cryo-EM。 |
| FcRL4はJ鎖を主に認識 | Su/Wang et al., PNAS 2026. PMID: [42308047](https://pubmed.ncbi.nlm.nih.gov/42308047/), DOI: [10.1073/pnas.2600183123](https://doi.org/10.1073/pnas.2600183123) | FcRL4-dIgA/J鎖結合の構造・機能解析。 |
| FcRL4 domain annotation | UniProt Q96PJ5 [FCRL4_HUMAN](https://www.uniprot.org/uniprotkb/Q96PJ5/entry) | FcRL4は4つのIg-like C2-type domainを持つ。D1 23-97、D2 102-183、D3 193-271、D4 275-374。 |
| FCRL5-IgG構造 | RCSB PDB [9LOC](https://www.rcsb.org/structure/9LOC), PDB DOI [10.2210/pdb9LOC/pdb](https://doi.org/10.2210/pdb9LOC/pdb) | FCRL5 bound to IgG-Fc。FcRL4と近い比較対象。 |
| FCRL5はIgG receptor | Chen et al., Sci Adv 2026. PMID: [41477863](https://pubmed.ncbi.nlm.nih.gov/41477863/), DOI: [10.1126/sciadv.aeb8865](https://doi.org/10.1126/sciadv.aeb8865) | FCRL5 D1-D3がIgG Fcを認識する構造・機能解析。 |
| FcRL4/FcRL5のIg結合とblocking抗体 | Wilson et al., J Immunol 2012. PMID: [22491254](https://pubmed.ncbi.nlm.nih.gov/22491254/), PMC: [PMC3634363](https://pmc.ncbi.nlm.nih.gov/articles/PMC3634363/) | FcRL4-IgA結合、413D12 blocking、418C8 non-blockingの根拠。 |
