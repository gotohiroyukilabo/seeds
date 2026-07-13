# Antibody Design Options: CD40 ligand / CD154 / TNFSF5

Target Card: `targets/target_cards/CD40LG.md`

## Design summary

推奨設計: `Fc-silent blocking antibody` または抗体断片/PEG化断片。CD40Lは血小板関連安全性が最大論点のため、Fc活性を持つ設計は原則避ける。

| Design | Initial fit | Mechanism of action | Expected benefit | Differentiation vs existing drugs | Safety risk | Developability risk | Initial assays | Kill criteria |
|---|---|---|---|---|---|---|---|---|
| Blocking antibody | Medium | CD40L-CD40結合を阻害し、T-B cell helpとAPC活性化を抑える。 | 自己抗体産生と炎症の上流を抑える。 | B細胞枯渇やBAFF阻害より上流のcostimulationを狙う。 | Fcが残ると血小板活性化/血栓リスク。感染。 | 結合価・Fc設計が安全性に直結。 | CD40L-CD40 blockade、T-B co-culture、platelet activation assay。 | 血小板活性化、凝集、またはCD40L immune complex形成。 |
| Agonistic antibody | Low | CD40Lを架橋/刺激する。 | 自己免疫では通常不要。 | なし。病態悪化リスクが高い。 | T/B細胞活性化、炎症増悪、血栓。 | アゴニズム制御困難。 | T-cell/B-cell activation assay。 | 免疫活性化が検出される。 |
| Fc-silent antibody | High | CD40Lを中和しつつFcγR/補体を介した血小板クロスリンクを避ける。 | CD40Lの強い生物学を安全に再利用できる可能性。 | 旧世代anti-CD40Lの血栓リスクを設計で回避する点。 | 完全には血小板リスクを排除できない可能性。感染、ワクチン応答低下。 | Fc silenceの完全性、半減期、免疫複合体。 | FcγR binding陰性、C1q陰性、platelet activation、T-B co-culture。 | Fc-silentでも血小板活性化または凝固マーカー上昇。 |
| Fc-enhanced antibody | Low | CD40L陽性細胞をADCC/ADCPで除去。 | 理論上は病原性活性化T細胞を除去。 | 安全性上の差別化は困難。 | 血小板、活性化T細胞、広範免疫毒性、血栓。 | Effector機能が標的安全性と相反。 | ADCC、platelet/T-cell crosslinking。 | いずれかの血小板/凝固リスクが出る。 |
| Bispecific antibody | Medium | CD40L blockadeに加え、疾患関連細胞/抑制受容体を同時標的化。 | 特定患者で効果を高める可能性。 | CD40L単独より作用選択性を高める仮説。 | 二重標的による免疫抑制、予期せぬ細胞架橋。 | CMC、結合価設計、血小板架橋リスク。 | Dual blockade、cell bridging、cytokine release、platelet assay。 | 細胞架橋や血小板活性化が避けられない。 |
| ADC | Low | CD40L発現細胞へpayload送達。 | 自己免疫では適さない。 | なし。 | 活性化T細胞/血小板毒性、全身毒性。 | ADC CMC、payload毒性。 | Internalization、payload toxicity。 | 正常免疫細胞/血小板毒性。 |
| Masked antibody | Medium | 炎症組織でのみCD40L blockerを活性化。 | 全身CD40L阻害と血小板リスクを下げる仮説。 | 旧世代/競合CD40L薬との差別化余地。 | 不完全masking、循環中活性化、効果不足。 | Protease-cleavable mask設計、活性化部位検証。 | Plasma stability、disease tissue cleavage、platelet assay after cleavage。 | 血中で活性化、または疾患組織で活性化しない。 |
| pH-dependent recycling antibody | Medium-Low | CD40L結合をpH依存化し、抗体再利用や抗原処理を改善。 | 高発現/可溶性CD40L環境で投与量を下げる可能性。 | 投与頻度・抗原sinkで差別化。 | 持続的免疫抑制、PK/PD予測の難しさ。 | pH依存性と中性結合の両立。 | pH binding、soluble CD40L sink model、PK/PD。 | pH設計が安全性・投与量に寄与しない。 |

## Initial recommendation

主案は `Fc-silent blocking antibody`。最初のgo/no-goは、CD40L-CD40 blockadeの強さではなく、血小板活性化・凝固関連シグナルを完全に避けられるかで判断する。
