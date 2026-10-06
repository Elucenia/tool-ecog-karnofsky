<!-- ELUCENIA technical documentation · ecog-karnofsky · it · no clinical/professional/rights approval -->

# ECOG e Karnofsky

[condizioni, fonti e autorizzazioni](https://elucenia.org/it/strumenti/ecog-karnofsky)

## Come usare

Usi lo strumento nel portale oppure apra index.html tramite un server HTTP locale. Selezioni la lingua, compili i campi ed esegua il calcolo.

## Dati di ingresso e unità

### Indice di Karnofsky

`kps`

- `0` — 0% · Deceduto
- `10` — 10% · Moribondo
- `20` — 20% · Molto malato; necessita di supporto attivo
- `30` — 30% · Gravemente disabile; ricovero indicato
- `40` — 40% · Disabile; necessita di cure speciali
- `50` — 50% · Necessita di aiuto considerevole e cure mediche frequenti
- `60` — 60% · Necessita di aiuto occasionale
- `70` — 70% · Si prende cura di sé, ma non lavora
- `80` — 80% · Attività normale con sforzo
- `90` — 90% · Attività normale; segni o sintomi minimi
- `100` — 100% · Normale, nessun disturbo o evidenza di malattia

## Edizione del metodo

ECOG 0–5/Oken 1982; corrispondenza KPS 90–100/70–80/50–60/30–40/10–20/0 di ECOG-ACRIN

## Formula documentata

Corrispondenza ECOG-ACRIN: Karnofsky 100–90% = ECOG 0; 80–70% = ECOG 1; 60–50% = ECOG 2; 40–30% = ECOG 3; 20–10% = ECOG 4; 0% = ECOG 5 (decesso).

Le scale non sono identiche: ECOG-ACRIN presenta la tabella come “uno dei modi” per associarle.

## Limiti e popolazione

La tabella ECOG-ACRIN presenta una corrispondenza comunemente usata tra ECOG e Karnofsky, tra diversi modi possibili di mettere in relazione le scale. Descrivono la capacità funzionale e aiutano a definire le popolazioni degli studi; la conversione da sola non stabilisce l’ammissibilità a un trattamento. La valutazione funzionale e i criteri del protocollo clinico devono essere preservati.

## Riferimenti

- [Oken MM et al. Toxicity and response criteria of the Eastern Cooperative Oncology Group. Am J Clin Oncol, 1982.](https://doi.org/10.1097/00000421-198212000-00014)

- [ECOG-ACRIN Cancer Research Group. ECOG Performance Status Scale (comparação com a escala de Karnofsky).](https://ecog-acrin.org/resources/ecog-performance-status/)

## Riprodurre i test tecnici

Esegua node test.cjs nella cartella principale di questo repository per ripetere i casi sintetici registrati. Gli input, i risultati attesi e le tolleranze originali sono conservati. I test tecnici non costituiscono validazione clinica.

```sh
node test.cjs
```

tool.json contiene le fonti, l’edizione e l’ambito della revisione. examples.json conserva gli input e i risultati attesi dei casi sintetici; results.json registra i risultati ottenuti.

[Scheda e riferimenti](../tool.json) · [Codice JavaScript](../calculator.js) · [Casi di riferimento](../examples.json) · [results.json](../results.json)

## Revisione e condizioni d’uso

Non è stata effettuata una revisione clinica indipendente.

Questa interfaccia è una traduzione realizzata dagli autori, non un’edizione ufficiale o certificata. Non sono state eseguite la revisione clinica indipendente, la revisione linguistica professionale né la verifica delle autorizzazioni relative ai diritti sugli strumenti.

Risultato della formula o classificazione. Interpretazione, condotta e applicabilità dipendono dalla valutazione professionale e dalla fonte selezionata.

## Licenza e attribuzione

Apache-2.0 si applica solo al codice di ELUCENIA. I diritti su strumenti, pubblicazioni, traduzioni e dati restano ai rispettivi titolari. Conservi LICENSE e NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Risultati documentati

Le informazioni seguenti conservano gli output del metodo per esempi sintetici. Non costituiscono una validazione clinica indipendente.

### 1

Completamente attivo, senza restrizioni rispetto allo stato precedente la malattia

| Dettagli del risultato | |
| --- | --- |
| Karnofsky 90% | In grado di svolgere un’attività normale; segni o sintomi minimi della malattia |
| Intervallo di Karnofsky di questo ECOG | 100–90% |


### 2

Limitato nell’attività fisica intensa, ma deambula ed è in grado di svolgere lavoro leggero o sedentario

| Dettagli del risultato | |
| --- | --- |
| Karnofsky 70% | Si prende cura di sé, ma è incapace di svolgere le normali attività o di lavorare attivamente |
| Intervallo di Karnofsky di questo ECOG | 80–70% |


### 3

Deambula ed è in grado di prendersi cura di sé, ma non può lavorare; fuori dal letto per più del 50% del tempo di veglia

| Dettagli del risultato | |
| --- | --- |
| Karnofsky 50% | Necessita di notevole assistenza e di cure mediche frequenti |
| Intervallo di Karnofsky di questo ECOG | 60–50% |

ECOG ≥ 2: la maggior parte degli studi di chemioterapia citotossica ha incluso solo ECOG 0 a 1 (o 2); valutare beneficio e tossicità.


### 4

Autocura limitata; a letto o seduto sulla sedia per più del 50% del tempo di veglia

| Dettagli del risultato | |
| --- | --- |
| Karnofsky 30% | Gravemente disabilitato; è indicato il ricovero, senza morte imminente |
| Intervallo di Karnofsky di questo ECOG | 40–30% |

ECOG ≥ 2: la maggior parte degli studi di chemioterapia citotossica ha incluso solo ECOG 0 a 1 (o 2); valutare beneficio e tossicità.

