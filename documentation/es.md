<!-- ELUCENIA technical documentation · ecog-karnofsky · es · no clinical/professional/rights approval -->

# ECOG y Karnofsky

[condiciones, fuentes y permisos](https://elucenia.org/es/herramientas/ecog-karnofsky)

## Cómo usar

Utilice la herramienta en el portal o abra index.html mediante un servidor HTTP local. Seleccione el idioma, complete los campos y calcule.

## Entradas y unidades

### Escala de Karnofsky

`kps`

- `0` — 0% · Fallecido
- `10` — 10% · Moribundo
- `20` — 20% · Muy enfermo; requiere tratamiento de soporte activo
- `30` — 30% · Gravemente incapacitado; hospitalización indicada
- `40` — 40% · Incapacitado; necesita cuidados especiales
- `50` — 50% · Requiere ayuda considerable y atención médica frecuente
- `60` — 60% · Requiere ayuda ocasional
- `70` — 70% · Se cuida solo, pero no trabaja
- `80` — 80% · Actividad normal con esfuerzo
- `90` — 90% · Actividad normal; signos o síntomas mínimos
- `100` — 100% · Normal, sin síntomas ni evidencia de enfermedad

## Edición del método

ECOG 0–5/Oken 1982; correspondencia KPS 90–100/70–80/50–60/30–40/10–20/0 de ECOG-ACRIN

## Fórmula documentada

Correspondencia ECOG-ACRIN: Karnofsky 100–90% = ECOG 0; 80–70% = ECOG 1; 60–50% = ECOG 2; 40–30% = ECOG 3; 20–10% = ECOG 4; 0% = ECOG 5 (fallecimiento).

Las escalas no son idénticas: ECOG-ACRIN presenta la tabla como “una de las formas” de relacionarlas.

## Límites y población

La tabla ECOG-ACRIN presenta una correspondencia habitual entre ECOG y Karnofsky, entre varias formas posibles de relacionar las escalas. Describen la capacidad funcional y ayudan a definir poblaciones de ensayos; la conversión no establece por sí sola la elegibilidad para un tratamiento. Deben conservarse la evaluación funcional y los criterios del protocolo clínico.

## Referencias

- [Oken MM et al. Toxicity and response criteria of the Eastern Cooperative Oncology Group. Am J Clin Oncol, 1982.](https://doi.org/10.1097/00000421-198212000-00014)

- [ECOG-ACRIN Cancer Research Group. ECOG Performance Status Scale (comparação com a escala de Karnofsky).](https://ecog-acrin.org/resources/ecog-performance-status/)

## Reproducir las pruebas técnicas

Ejecute node test.cjs en el directorio raíz de este repositorio para repetir los casos sintéticos registrados. Se conservan las entradas, los resultados esperados y las tolerancias originales. Las pruebas técnicas no constituyen validación clínica.

```sh
node test.cjs
```

tool.json contiene las fuentes, la edición y el alcance de la revisión. examples.json conserva las entradas y los resultados esperados de los casos sintéticos; results.json registra los resultados obtenidos.

[Ficha y referencias](../tool.json) · [Código JavaScript](../calculator.js) · [Casos de referencia](../examples.json) · [results.json](../results.json)

## Revisión y condiciones de uso

No se ha realizado una revisión clínica independiente.

Esta interfaz es una traducción de elaboración propia, no una edición oficial o certificada. No se han realizado la revisión clínica independiente, la revisión lingüística profesional ni la autorización de derechos de los instrumentos.

Resultado de la fórmula o clasificación. La interpretación, la conducta y la aplicabilidad dependen de la evaluación profesional y de la fuente seleccionada.

## Licencia y atribución

Apache-2.0 se aplica únicamente al código de ELUCENIA. Los derechos de los instrumentos, publicaciones, traducciones y datos permanecen en manos de sus respectivos titulares. Conserve LICENSE y NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026
