<!-- ELUCENIA technical documentation · ecog-karnofsky · de · no clinical/professional/rights approval -->

# ECOG und Karnofsky

[Bedingungen, Quellen und Berechtigungen](https://elucenia.org/de/werkzeuge/ecog-karnofsky)

## Verwendung

Verwenden Sie das Werkzeug im Portal oder öffnen Sie index.html über einen lokalen HTTP-Server. Wählen Sie die Sprache, füllen Sie die Felder aus und berechnen Sie das Ergebnis.

## Eingaben und Einheiten

### Karnofsky-Index

`kps`

- `0` — 0 % · Verstorben
- `10` — 10 % · Moribund
- `20` — 20 % · Schwer krank; aktive unterstützende Behandlung erforderlich
- `30` — 30 % · Schwer beeinträchtigt; Krankenhausaufnahme angezeigt
- `40` — 40 % · Behindert; benötigt spezielle Versorgung
- `50` — 50 % · Benötigt erhebliche Hilfe und häufige medizinische Betreuung
- `60` — 60 % · Benötigt gelegentliche Hilfe
- `70` — 70 % · Versorgt sich selbst, arbeitet aber nicht
- `80` — 80 % · Normale Aktivität mit Anstrengung
- `90` — 90 % · Normale Aktivität; minimale Zeichen oder Symptome
- `100` — 100 % · Normal, keine Beschwerden oder Krankheitszeichen

## Fassung der Methode

ECOG 0–5/Oken 1982; KPS-Zuordnung 90–100/70–80/50–60/30–40/10–20/0 nach ECOG-ACRIN

## Dokumentierte Formel

ECOG-ACRIN-Zuordnung: Karnofsky 100–90% = ECOG 0; 80–70% = ECOG 1; 60–50% = ECOG 2; 40–30% = ECOG 3; 20–10% = ECOG 4; 0% = ECOG 5 (Tod).

Die Skalen sind nicht identisch: ECOG-ACRIN stellt die Tabelle selbst als „eine Möglichkeit“ der Zuordnung dar.

## Grenzen und Population

Die ECOG-ACRIN-Tabelle zeigt eine häufig verwendete Zuordnung zwischen ECOG und Karnofsky unter mehreren möglichen Skalenabbildungen. Die Skalen beschreiben Funktionsfähigkeit und helfen, Studienpopulationen festzulegen; die Umrechnung allein bestimmt keine Behandlungseignung. Funktionelle Beurteilung und Kriterien des klinischen Protokolls müssen erhalten bleiben.

## Referenzen

- [Oken MM et al. Toxicity and response criteria of the Eastern Cooperative Oncology Group. Am J Clin Oncol, 1982.](https://doi.org/10.1097/00000421-198212000-00014)

- [ECOG-ACRIN Cancer Research Group. ECOG Performance Status Scale (comparação com a escala de Karnofsky).](https://ecog-acrin.org/resources/ecog-performance-status/)

## Technische Tests reproduzieren

Führen Sie node test.cjs im Stammverzeichnis dieses Repositorys aus, um die dokumentierten synthetischen Fälle zu wiederholen. Ursprüngliche Eingaben, erwartete Ergebnisse und Toleranzen bleiben erhalten. Technische Tests stellen keine klinische Validierung dar.

```sh
node test.cjs
```

tool.json enthält Quellen, Ausgabe und Umfang der Überprüfung. examples.json bewahrt die synthetischen Eingaben und erwarteten Ergebnisse; results.json dokumentiert die tatsächlich erhaltenen Ergebnisse.

[Eintrag und Referenzen](../tool.json) · [JavaScript-Code](../calculator.js) · [Referenzfälle](../examples.json) · [results.json](../results.json)

## Überprüfung und Nutzungsbedingungen

Eine unabhängige klinische Prüfung wurde nicht durchgeführt.

Diese Benutzeroberfläche ist eine selbst erstellte Übersetzung und keine offizielle oder zertifizierte Ausgabe. Eine unabhängige klinische Überprüfung, eine professionelle sprachliche Prüfung und eine Klärung der Rechte an den Instrumenten wurden nicht durchgeführt.

Ergebnis der Formel oder Klassifikation. Interpretation, Vorgehen und Anwendbarkeit hängen von der fachlichen Beurteilung und der ausgewählten Quelle ab.

## Lizenz und Urheberangaben

Apache-2.0 gilt nur für den ELUCENIA-Code. Die Rechte an Instrumenten, Veröffentlichungen, Übersetzungen und Daten verbleiben bei den jeweiligen Rechteinhabern. Bewahren Sie LICENSE und NOTICE auf.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Dokumentierte Ergebnisse

Die folgenden Angaben bewahren die Ausgaben der Methode für synthetische Beispiele. Sie stellen keine unabhängige klinische Validierung dar.

### 1

Voll aktiv, ohne Einschränkung gegenüber dem Zustand vor der Erkrankung

| Ergebnisdetails | |
| --- | --- |
| Karnofsky 90% | Zu normaler Aktivität fähig; minimale Anzeichen oder Symptome der Erkrankung |
| Karnofsky-Bereich dieses ECOG | 100–90% |


### 2

Eingeschränkt bei anstrengender körperlicher Aktivität, aber gehfähig und fähig zu leichter oder sitzender Arbeit

| Ergebnisdetails | |
| --- | --- |
| Karnofsky 70% | Kann sich selbst versorgen, ist aber unfähig zu normaler Aktivität oder aktiver Arbeit |
| Karnofsky-Bereich dieses ECOG | 80–70% |


### 3

Gehfähig und in der Lage, sich selbst zu versorgen, aber nicht arbeitsfähig; mehr als 50% der wachen Zeit außerhalb des Bettes

| Ergebnisdetails | |
| --- | --- |
| Karnofsky 50% | Benötigt erhebliche Unterstützung und häufige medizinische Versorgung |
| Karnofsky-Bereich dieses ECOG | 60–50% |

ECOG ≥ 2: Die meisten Studien zur zytotoxischen Chemotherapie schlossen nur ECOG 0 bis 1 (oder 2) ein; Nutzen und Toxizität abwägen.


### 4

Eingeschränkte Selbstversorgung; mehr als 50% der wachen Zeit im Bett oder im Stuhl

| Ergebnisdetails | |
| --- | --- |
| Karnofsky 30% | Schwer behindert; Krankenhausaufnahme angezeigt, jedoch kein unmittelbar bevorstehender Tod |
| Karnofsky-Bereich dieses ECOG | 40–30% |

ECOG ≥ 2: Die meisten Studien zur zytotoxischen Chemotherapie schlossen nur ECOG 0 bis 1 (oder 2) ein; Nutzen und Toxizität abwägen.

