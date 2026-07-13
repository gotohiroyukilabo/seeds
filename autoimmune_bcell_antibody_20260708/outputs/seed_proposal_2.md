# シーズ提案2: FCRL4 x CD22組織B細胞サイレンサー

## 1文提案
Sjögren病のFCRL4陽性唾液腺B細胞に、CD22 brakeとFCRL4 brakeを同じ膜上で入れるFc-silent FCRL4 x CD22 BsAbを開発する。

## 疾患の壁
Sjögren病には広く使える疾患修飾的治療が乏しく、乾燥、疲労、神経障害、肺病変、低補体、高IgG、リンパ腫リスクを抱える患者が残る。

## 標的の妥当性
FCRL4はSjögren唾液腺の上皮近傍B細胞と関連し、組織常在/粘膜記憶B細胞のstate markerであるだけでなく、文献上はBCR応答を弱める免疫調節分子として扱われている。CD22もB細胞抑制受容体である。したがって、FCRL4を「住所」、CD22を「ブレーキ」と見るだけでなく、FCRL4自体も第二のブレーキとして利用できる可能性がある。

## 抗体である必然性
FCRL4とCD22を同じB細胞上でcis co-ligationする空間薬理が必要である。狙いは、CD22単独刺激ではなく、FCRL4陽性病変B細胞のBCR microcluster近傍にCD22/SHP-1系とFCRL4/SHP系の抑制入力を同時に置くことである。anti-FCRL4とanti-CD22の2剤併用では再現できる保証がない。

## 抗体設計案
主案はFc-silent FCRL4 x CD22 BsAb。これは「Fc依存性trogocytosisを使わない方が必ず正しい」という意味ではなく、まずFCRL4-gated cis co-ligationだけでCD22/SHP-1抑制とFCRL4側のBCR抑制が成立するかをきれいに検証するためである。

並行して、Fc-activeまたはFc-tuned FCRL4 x CD22も比較する。Fc依存性trogocytosisが薬効に必要な場合は、Fc-silent案を主案から下げ、FCRL4-gated Fc-active tissue modulatorとして再設計する。ただし、その場合はepratuzumab様の広いB細胞表面分子strippingではなく、FCRL4陽性病変B細胞に限定されたtrogocytosisであることが必須である。ADCは低優先。

FCRL4共刺激については、活性化刺激ではなく「FCRL4 agonismによる共抑制刺激」として設計する。FCRL4刺激がBCR抑制を強めれば本提案の革新性は上がる。一方で、FCRL4陽性組織B細胞はTLR応答や粘膜記憶B細胞機能とも関係するため、FCRL4 ligationでTLR7/9、CD40、IL-21反応やIg産生が増える場合は危険信号である。

## 抗FCRL4単独との比較
抗FCRL4単独は陰性対照ではなく、独立した候補として扱う。CD22 agonismが弱くても、FCRL4+ disease-state B cellそのものを標的化できるなら、抗FCRL4単独で成立する可能性がある。

比較する単独抗体は3種類である。1つ目はFc-silent agonist型で、FCRL4 signalingだけでBCR/TLR/Tfh反応を抑えられるかを見る。2つ目はFc-active/Fc-tuned型で、FCRL4+病変B細胞に限定したtrogocytosis、ADCP、軽度depletionが可能かを見る。3つ目はnon-blocking anchor型で、内因性IgA/J-chain/FCRL4調節を邪魔せず、FCRL4+ state/niche B細胞に結合するだけで安全なbenchmarkになるかを見る。

抗FCRL4単独がBsAbと同等または上回るなら、BsAbより単純で開発しやすい抗FCRL4単独へpivotする。BsAbを主案として残す条件は、anti-FCRL4単独、anti-CD22単独、2剤併用を明確に上回ることである。

## 既存薬との差別化
rituximab、BAFF阻害、CD40L阻害、FcRn阻害、epratuzumabの焼き直しではない。epratuzumabの教訓は致命傷ではなく、広いSLEでCD22単独modulationが不十分だったという失敗学習である。本提案は疾患文脈、患者選択、抗体geometryを変え、さらにFCRL4を単なる住所ではなくBCR抑制入力として使えるかを問う。

## FcRL4標的の競合
2026-07-12時点の公開情報では、FcRL4/FCRL4/CD307d/FCRH4を直接標的にした臨床段階の抗体薬、BsAb、ADC、CAR-Tは確認できない。ここは競合が薄い一方で、標的biologyが未成熟というリスクもある。

注意すべき隣接競合はFCRL5/FcRH5である。Genentech/RocheのcevostamabはFcRH5 x CD3 T-cell engagerとして多発性骨髄腫で開発され、SLE with/without active LNのPhase Ib試験も2026-07-31開始予定で登録されている。これはFcRL4直接競合ではないが、FCRL familyを自己免疫B細胞薬に使う流れが始まったことを示す。

したがって本提案は、FCRL5 x CD3型の全身性depletionではなく、Sjögren腺内のFcRL4+組織B細胞をFc-silentまたはFc-tunedに沈静化する点で差別化する。

## 腺外症状への位置付け
本提案の主効果は、唾液腺/粘膜B細胞ニッチに最も出やすい。関節痛、神経障害、皮膚紫斑、腎/肺病変への効果は、RF、cryoglobulin、低C4、CXCL13、高IgG、腺腫脹などB-cell-high systemic axisと連動する患者に限定して狙う。疲労、brain fog、慢性疼痛はprimary endpointにしない。

関節症状については、Sjögren関節痛そのものとFcRL4の直接証拠は乏しい。一方でRA滑膜ではFcRL4+ B細胞がRANKL/TNF高発現で、自己抗原反応性も示す報告がある。したがって、FcRL4起点の他疾患展開はRA滑膜B細胞高値患者が最有力である。

## epratuzumab失敗との合致
合致する点は、患者選択、組織ニッチ非選択、CD22単独の弱さをFCRL4 gateとBsAb co-ligationで補う点である。合致しない可能性は、epratuzumabがFc依存trogocytosisに依存していた場合であり、Fc-silent設計では効かないかもしれない。

## 主要リスク
FCRL4がbystander、FCRL4抗体刺激でBCR抑制が再現しない、FCRL4刺激でTLR7/9やTfh help反応が増える、CD22抑制が弱い、Fc-silentで効かない、Fc-active化すると非選択的trogocytosisや組織炎症が出る、FCRL5 x CD3など近縁FCRL family競合が先行する、唾液腺アクセス、粘膜記憶B細胞への影響。

## 最初にやるべき検証
fresh唾液腺サンプルでFCRL4+ B細胞が病態関連であることを示し、anti-FCRL4 Fc-silent agonist、anti-FCRL4 neutral/non-blocking、anti-FCRL4 Fc-active/Fc-tuned、anti-CD22単独、2剤併用、Fc-silent BsAb、Fc-active BsAbを同じ系で比較する。特に、FCRL4 ligation単独またはCD22との共刺激で、pSyk、pBLNK、pPLCγ2、Ca flux、pERK、Ig産生、抗原提示、TLR7/9応答がどう動くかを測る。

腺外症状については、唾液腺FcRL4+ B細胞量とESSDAI domain、CXCL13、BAFF、IL-21、RF、cryoglobulin、C4、高IgGを相関させる。関節症状がある場合は超音波/MRIで滑膜炎を確認し、可能なら滑膜液/滑膜生検でFcRL4+CD22+ B細胞を見る。神経障害はcryoglobulinemic/vasculitic phenotypeと非vasculitic phenotypeを分ける。

## 継続/中止基準
継続条件: FCRL4+ B細胞が明確、Fc-silent BsAbがCD22/SHP-1とFCRL4側の抑制入力を誘導し、anti-CD22単独、anti-FCRL4単独、2剤併用を上回る。または、anti-FCRL4単独が同等以上なら抗FCRL4単独候補へpivotする。Fc-active/Fc-tuned BsAbでのみ効く場合でも、trogocytosisがFCRL4陽性病変B細胞に限定され、正常粘膜B細胞との安全域がある。

中止条件: FCRL4が無関係、FCRL4 ligationがBCR抑制ではなくTLR7/9やIg産生を増やす、BsAbがanti-FCRL4単独/anti-CD22単独/2剤併用を超えない、Fc-active化で非選択的なB細胞表面分子strippingや炎症が出る、汎B細胞除去が必要。
