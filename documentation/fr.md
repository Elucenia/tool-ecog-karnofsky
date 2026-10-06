<!-- ELUCENIA technical documentation · ecog-karnofsky · fr · no clinical/professional/rights approval -->

# ECOG et Karnofsky

[conditions, sources et autorisations](https://elucenia.org/fr/outils/ecog-karnofsky)

## Mode d’emploi

Utilisez l’outil sur le portail ou ouvrez index.html via un serveur HTTP local. Sélectionnez la langue, remplissez les champs et lancez le calcul.

## Données d’entrée et unités

### Indice de Karnofsky

`kps`

- `0` — 0 % · Décédé
- `10` — 10 % · Moribond
- `20` — 20 % · Très malade ; soins de soutien actifs nécessaires
- `30` — 30 % · Gravement handicapé ; hospitalisation indiquée
- `40` — 40 % · Handicapé ; nécessite des soins particuliers
- `50` — 50 % · Aide importante et soins médicaux fréquents nécessaires
- `60` — 60 % · Aide occasionnelle nécessaire
- `70` — 70 % · Se prend en charge, mais ne travaille pas
- `80` — 80 % · Activité normale avec effort
- `90` — 90 % · Activité normale ; signes ou symptômes minimes
- `100` — 100 % · Normal, aucune plainte ni signe de maladie

## Édition de la méthode

ECOG 0–5/Oken 1982 ; correspondance KPS 90–100/70–80/50–60/30–40/10–20/0 d’ECOG-ACRIN

## Formule documentée

Correspondance ECOG-ACRIN : Karnofsky 100–90% = ECOG 0 ; 80–70% = ECOG 1 ; 60–50% = ECOG 2 ; 40–30% = ECOG 3 ; 20–10% = ECOG 4 ; 0% = ECOG 5 (décès).

Les échelles ne sont pas identiques : ECOG-ACRIN présente ce tableau comme « une des façons » de les faire correspondre.

## Limites et population

Le tableau ECOG-ACRIN présente une correspondance couramment utilisée entre ECOG et Karnofsky, parmi plusieurs façons possibles de rapprocher les échelles. Elles décrivent la capacité fonctionnelle et aident à définir les populations d’essais ; la conversion ne permet pas, seule, d’établir l’éligibilité à un traitement. L’évaluation fonctionnelle et les critères du protocole clinique doivent être conservés.

## Références

- [Oken MM et al. Toxicity and response criteria of the Eastern Cooperative Oncology Group. Am J Clin Oncol, 1982.](https://doi.org/10.1097/00000421-198212000-00014)

- [ECOG-ACRIN Cancer Research Group. ECOG Performance Status Scale (comparação com a escala de Karnofsky).](https://ecog-acrin.org/resources/ecog-performance-status/)

## Reproduire les tests techniques

Exécutez node test.cjs dans le répertoire racine de ce dépôt pour reproduire les cas synthétiques enregistrés. Les données d’entrée, les résultats attendus et les tolérances d’origine sont conservés. Les tests techniques ne constituent pas une validation clinique.

```sh
node test.cjs
```

tool.json contient les sources, l’édition et le périmètre de la revue. examples.json conserve les données d’entrée et les résultats attendus des cas synthétiques ; results.json consigne les résultats obtenus.

[Fiche et références](../tool.json) · [Code JavaScript](../calculator.js) · [Cas de référence](../examples.json) · [results.json](../results.json)

## Revue et conditions d’utilisation

Aucune révision clinique indépendante n’a été effectuée.

Cette interface est une traduction réalisée par nos soins, et non une édition officielle ou certifiée. La revue clinique indépendante, la révision linguistique professionnelle et l’autorisation des droits sur les instruments n’ont pas été réalisées.

Résultat de la formule ou de la classification. L’interprétation, la conduite et l’applicabilité dépendent de l’évaluation professionnelle et de la source sélectionnée.

## Licence et attribution

Apache-2.0 s’applique uniquement au code d’ELUCENIA. Les droits sur les instruments, publications, traductions et données restent ceux de leurs titulaires respectifs. Conservez LICENSE et NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Résultats documentés

Les informations ci-dessous conservent les sorties de la méthode pour des exemples synthétiques. Elles ne constituent pas une validation clinique indépendante.

### 1

Entièrement actif, sans restriction par rapport à l’état antérieur à la maladie

| Détails du résultat | |
| --- | --- |
| Karnofsky 90 % | Capable de mener une activité normale ; signes ou symptômes minimes de la maladie |
| Intervalle de Karnofsky pour cet ECOG | 100–90% |


### 2

Limité dans les efforts physiques intenses, mais ambulatoire et capable d’effectuer un travail léger ou sédentaire

| Détails du résultat | |
| --- | --- |
| Karnofsky 70 % | Prend soin de lui-même, mais est incapable d’une activité normale ou d’un travail actif |
| Intervalle de Karnofsky pour cet ECOG | 80–70% |


### 3

Ambulatoire et capable de prendre soin de lui-même, mais incapable de travailler ; hors du lit plus de 50 % du temps d’éveil

| Détails du résultat | |
| --- | --- |
| Karnofsky 50 % | Nécessite une aide importante et des soins médicaux fréquents |
| Intervalle de Karnofsky pour cet ECOG | 60–50% |

ECOG ≥ 2 : la plupart des essais de chimiothérapie cytotoxique n’ont inclus que les ECOG 0 à 1 (ou 2) ; peser le bénéfice et la toxicité.


### 4

Autonomie limitée ; alité ou assis sur une chaise plus de 50 % du temps d’éveil

| Détails du résultat | |
| --- | --- |
| Karnofsky 30 % | Gravement handicapé ; hospitalisation indiquée, sans décès imminent |
| Intervalle de Karnofsky pour cet ECOG | 40–30% |

ECOG ≥ 2 : la plupart des essais de chimiothérapie cytotoxique n’ont inclus que les ECOG 0 à 1 (ou 2) ; peser le bénéfice et la toxicité.

