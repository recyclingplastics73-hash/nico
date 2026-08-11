# Geomembrana HDPE lisa — 1000 µm (1.0 mm) — Tabla de referencia

Referencia para comparar medidas propias contra lo que otras fábricas declaran y publican.
Construida el 2026-08-11 a partir de **11 fabricantes** (Solmax, GSE, AGRU, NAUE, Atarfil,
Sotrafa, Maruplast, GEOSAI, Pavco, Huitex, más la homologación estatal peruana) — ver
[FUENTES.md](FUENTES.md) y el detalle punto por punto en
[datos-extraidos.csv](datos-extraidos.csv).

Dos columnas de referencia, que no hay que mezclar:

- **Mín. fábricas** — lo que los fabricantes *garantizan* (mínimos declarados/MARV, formato GM13).
- **Típicos** — lo que los fabricantes *declaran como valor típico o nominal de producción*.
  Es la columna contra la que comparar tu medida. ⚠ marca filas con una sola fuente (dato débil).

| Propiedad | Método | Unidad | Mín. GM13 | Mín. fábricas (rango) | Típicos (rango) | Típico (mediana) | n | Mi medida | Desvío vs típico |
|---|---|---|---|---|---|---|---|---|---|
| **Espesor y densidad** | | | | | | | | | |
| Espesor promedio | ASTM D5199 | mm | 1.00 | 0.90 – 1.02 ¹ | 1.00 | 1.00 | 2 | | |
| Espesor mínimo individual (de 10 lecturas) | ASTM D5199 | mm | 0.90 | 0.90 – 0.91 | — ² | — | 0 | | |
| Densidad | ASTM D1505 / D792 | g/cm³ | 0.940 | 0.940 – 0.942 | 0.942 ⚠ | 0.942 | 1 | | |
| **Tracción (ASTM D6693 tipo IV)** | | | | | | | | | |
| Resistencia en fluencia | ASTM D6693 | kN/m | 15 | 14.7 – 15.4 | 15 – 16 | 16 | 3 | | |
| Resistencia en rotura | ASTM D6693 | kN/m | 27 | 26.6 – 28 | 27 – 30 | 28 | 3 | | |
| Elongación en fluencia | ASTM D6693 | % | 12 | 12 – 13 | 12 – 13 | 12 | 4 | | |
| Elongación en rotura | ASTM D6693 | % | 700 | 700 – 750 | 700 – 800 | 725 | 4 | | |
| **Desgarre y punzonamiento** | | | | | | | | | |
| Resistencia al desgarre | ASTM D1004 | N | 125 | 125 – 133 | 125 – 145 | 130 | 4 | | |
| Resistencia al punzonamiento | ASTM D4833 | N | 320 | 320 – 378 | 320 – 440 | 320 | 4 | | |
| **Negro de humo, OIT y durabilidad** | | | | | | | | | |
| Contenido de negro de humo | ASTM D4218 | % | 2.0–3.0 (rango) | 2.0 – 3.0 | 2.5 ⚠ ³ | 2.5 | 1 | | |
| Dispersión de negro de humo | ASTM D5596 | categoría | 9 de 10 en Cat. 1–2 | Cat. 1–2 (todas las fichas) | Cat. 1–2 | Cat. 1–2 | 11 | | |
| OIT estándar | ASTM D3895 | min | 100 | 100 – 160 | 100 – 160 | 100 | 2 | | |
| OIT alta presión | ASTM D5885 | min | 400 | 400 – 800 | 800 ⚠ | 800 | 1 | | |
| Envejecimiento en horno 85 °C, 90 d (OIT retenido) | ASTM D5721 + D3895/D5885 | % | 55 (est.) / 80 (AP) | 55 – 80 | 55 ⚠ | 55 | 1 | | |
| Resistencia UV, 1600 h (OIT AP retenido) | ASTM D7238 + D5885 | % | 50 | 50 – 80 | — ⁴ | — | 0 | | |
| Agrietamiento por esfuerzo (SP-NCTL) | ASTM D5397 | h | 500 | 300 – 3000 ⁵ | 400 – 1000 | 500 | 3 | | |

*Desvío vs típico = (mi medida − típico) / típico × 100 %.*

## Notas

1. El rango de mínimos de espesor incluye fichas imperiales (40 mils = 1.016 mm) y una ficha
   que declara 0.90 como promedio mínimo; la mediana declarada es 1.00.
2. Ninguna ficha declara valor típico del espesor mínimo individual; todas usan el −10 %
   normativo (0.90 mm).
3. Negro de humo: solo Sotrafa declara valor de producción (2.25 ± 0.25 %); el resto da el
   rango 2.0–3.0 de norma.
4. Resistencia UV: ningún fabricante publica típico, solo el mínimo (≥50 %, y Sotrafa ≥55 %
   vía UNE-EN 728). Comparar contra el mínimo.
5. SCR: los mínimos declarados van de 300 h (fichas viejas, GM13 anterior) a 3000 h (líneas
   premium); GM13 vigente exige 500 h.

## Advertencias de lectura

- **Sesgo a la baja de los "típicos":** Pavco y Maruplast declaran como típico cifras iguales
  al mínimo GM13 (15/27 kN/m, 125 N, 320 N…). Los típicos de NAUE, Sotrafa y DM están por
  encima. El extremo alto del rango es mejor estimador de una producción sana que el bajo.
- **Métodos EN no comparables:** Sotrafa, Atarfil y GSE (EMEA) publican además valores según
  UNE-EN ISO 527 (p. ej. rotura 33 MPa / 900 % Sotrafa típico), ISO 34-1 (desgarre 150 N típico)
  y EN ISO 12236 (punzonamiento CBR 2.5–3.3 kN, otro ensayo). **No** van en las columnas ASTM;
  están en [datos-extraidos.csv](datos-extraidos.csv) con `comparable_astm=no`.
- Aún sin valores **medidos** de lote (certificados de calidad): los documentos candidatos
  están listados en FUENTES.md §B, pendientes de descarga con cuenta Scribd/Studocu. Al
  incorporarlos, esta tabla pasa de "declarado por fabricantes" a "medido por fábricas".
