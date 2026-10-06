<!-- ELUCENIA technical documentation · ecog-karnofsky · pt-BR · no clinical/professional/rights approval -->

# ECOG e Karnofsky

[condições, fontes e permissões](https://elucenia.org/pt-br/ferramentas/ecog-karnofsky)

## Como usar

Use a ferramenta no portal ou abra index.html em um servidor HTTP local. Selecione o idioma, preencha os campos e calcule.

## Entradas e unidades

### Escala de Karnofsky

`kps`

- `0` — 0% · Óbito
- `10` — 10% · Moribundo
- `20` — 20% · Muito doente; suporte ativo necessário
- `30` — 30% · Gravemente incapacitado; internação indicada
- `40` — 40% · Incapacitado; precisa de cuidados especiais
- `50` — 50% · Precisa de ajuda considerável e cuidados médicos frequentes
- `60` — 60% · Precisa de ajuda ocasional
- `70` — 70% · Cuida de si, mas não trabalha
- `80` — 80% · Atividade normal com esforço
- `90` — 90% · Atividade normal; sinais ou sintomas mínimos
- `100` — 100% · Normal, sem queixas nem evidência de doença

## Edição do método

ECOG 0–5/Oken 1982; correspondência KPS 90–100/70–80/50–60/30–40/10–20/0 de ECOGACRIN

## Fórmula documentada

Correspondência usada pelo ECOG-ACRIN: Karnofsky 100–90% = ECOG 0; 80–70% = ECOG 1; 60–50% = ECOG 2; 40–30% = ECOG 3; 20–10% = ECOG 4; 0% = ECOG 5 (óbito).

As escalas não são idênticas: a própria tabela do ECOG-ACRIN é apresentada como "uma das formas" de mapear uma na outra.

## Limites e população

A tabela ECOG-ACRIN apresenta uma correspondência comumente usada entre ECOG e Karnofsky, entre várias formas possíveis de mapear as escalas. Elas descrevem capacidade funcional e ajudam a definir populações de ensaios; a conversão não estabelece, sozinha, elegibilidade para um tratamento. A avaliação funcional e os critérios do protocolo clínico devem ser preservados.

## Referências

- [Oken MM et al. Toxicity and response criteria of the Eastern Cooperative Oncology Group. Am J Clin Oncol, 1982.](https://doi.org/10.1097/00000421-198212000-00014)

- [ECOG-ACRIN Cancer Research Group. ECOG Performance Status Scale (comparação com a escala de Karnofsky).](https://ecog-acrin.org/resources/ecog-performance-status/)

## Reproduzir os testes técnicos

Execute node test.cjs na pasta raiz deste repositório para repetir os casos sintéticos registrados. As entradas, expectativas e tolerâncias originais são preservadas. Testes técnicos não constituem validação clínica.

```sh
node test.cjs
```

tool.json contém fontes, edição e escopo de revisão. examples.json conserva as entradas e expectativas sintéticas; results.json registra os resultados obtidos.

[Ficha e referências](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referência](../examples.json) · [results.json](../results.json)

## Revisão e condições de uso

Revisão clínica independente não realizada.

Esta interface é uma tradução autoral, não uma edição oficial ou certificada. Revisão clínica independente, revisão linguística profissional e autorização de direitos de instrumentos não foram realizadas.

Resultado da fórmula ou classificação. Interpretação, conduta e aplicabilidade dependem da avaliação profissional e da fonte selecionada.

## Licença e atribuição

Apache-2.0 aplica-se somente ao código da ELUCENIA. Os instrumentos, publicações, traduções e dados mantêm os direitos dos respectivos titulares. Preserve LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Resultados documentados

As informações abaixo preservam as saídas do método para exemplos sintéticos. Não constituem validação clínica independente.

### 1

Totalmente ativo, sem restrição em relação ao estado anterior à doença

| Detalhes do resultado | |
| --- | --- |
| Karnofsky 90% | Capaz de atividade normal; sinais ou sintomas mínimos da doença |
| Faixa de Karnofsky deste ECOG | 100–90% |


### 2

Restrito em atividade física extenuante, mas deambula e faz trabalho leve ou sedentário

| Detalhes do resultado | |
| --- | --- |
| Karnofsky 70% | Cuida de si, mas é incapaz de atividade normal ou de trabalho ativo |
| Faixa de Karnofsky deste ECOG | 80–70% |


### 3

Deambula e cuida de si, mas não consegue trabalhar; fora do leito mais de 50% do tempo acordado

| Detalhes do resultado | |
| --- | --- |
| Karnofsky 50% | Precisa de ajuda considerável e de cuidados médicos frequentes |
| Faixa de Karnofsky deste ECOG | 60–50% |

ECOG ≥ 2: a maioria dos ensaios de quimioterapia citotóxica incluiu apenas ECOG 0 a 1 (ou 2); pese benefício e toxicidade.


### 4

Autocuidado limitado; no leito ou na cadeira mais de 50% do tempo acordado

| Detalhes do resultado | |
| --- | --- |
| Karnofsky 30% | Gravemente incapacitado; internação indicada, sem morte iminente |
| Faixa de Karnofsky deste ECOG | 40–30% |

ECOG ≥ 2: a maioria dos ensaios de quimioterapia citotóxica incluiu apenas ECOG 0 a 1 (ou 2); pese benefício e toxicidade.

