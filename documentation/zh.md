<!-- ELUCENIA technical documentation · ecog-karnofsky · zh · no clinical/professional/rights approval -->

# ECOG 与 Karnofsky

[条件、来源与许可](https://elucenia.org/zh/tools/ecog-karnofsky)

## 使用方法

在门户中使用工具，或通过本地 HTTP 服务器打开 index.html。选择语言，填写各字段，然后计算。

## 输入与单位

### Karnofsky 评分

`kps`

- `0` — 0% · 死亡
- `10` — 10% · 濒死
- `20` — 20% · 病情极重；需积极支持
- `30` — 30% · 严重功能障碍；应住院
- `40` — 40% · 功能障碍；需特殊照护
- `50` — 50% · 需大量帮助及经常性医疗护理
- `60` — 60% · 偶尔需要帮助
- `70` — 70% · 可自理，但不能工作
- `80` — 80% · 需努力才能维持正常活动
- `90` — 90% · 活动正常；症状或体征轻微
- `100` — 100% · 正常，无主诉或疾病证据

## 方法版本

ECOG 0–5/Oken 1982；ECOG-ACRIN的KPS对应90–100/70–80/50–60/30–40/10–20/0

## 已记录的公式

ECOG-ACRIN对应：Karnofsky 100–90% = ECOG 0；80–70% = ECOG 1；60–50% = ECOG 2；40–30% = ECOG 3；20–10% = ECOG 4；0% = ECOG 5（死亡）。

两种量表并不相同：ECOG-ACRIN将此表说明为相互对应的“方法之一”。

## 限制与适用人群

ECOG-ACRIN表列出ECOG与Karnofsky之间常用的对应关系，它只是两种量表之间多种可能映射方式之一。量表描述功能能力，并有助于界定试验人群；单独的换算不能确定接受某种治疗的资格。应保留功能评估和临床方案的标准。

## 参考文献

- [Oken MM et al. Toxicity and response criteria of the Eastern Cooperative Oncology Group. Am J Clin Oncol, 1982.](https://doi.org/10.1097/00000421-198212000-00014)

- [ECOG-ACRIN Cancer Research Group. ECOG Performance Status Scale (comparação com a escala de Karnofsky).](https://ecog-acrin.org/resources/ecog-performance-status/)

## 复现技术测试

在此仓库的根目录中运行 node test.cjs，以重复已记录的合成案例。原始输入、预期结果和容差保持不变。技术测试不构成临床验证。

```sh
node test.cjs
```

tool.json 包含来源、版本和审查范围。examples.json 保留合成输入与预期结果；results.json 记录实际得到的结果。

[记录与参考文献](../tool.json) · [JavaScript代码](../calculator.js) · [参考案例](../examples.json) · [results.json](../results.json)

## 审查与使用条件

尚未开展独立临床审查。

此界面为自主编写的翻译，并非官方或认证版本。尚未完成独立临床审查、专业语言审查或工具权利授权。

公式或分类结果。解释、处理及适用性须结合专业评估和所选来源。

## 许可与署名

Apache-2.0 仅适用于 ELUCENIA 代码。工具、出版物、翻译和数据的权利仍归各自权利人所有。请保留 LICENSE 和 NOTICE。

ELUCENIA · Felipe Guedes · Copyright © 2026
