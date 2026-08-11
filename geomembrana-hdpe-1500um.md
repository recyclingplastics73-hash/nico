# Geomembrana HDPE lisa — 1500 µm (1.5 mm) — Tabla de referencia

Referencia para comparar medidas propias contra lo que otras fábricas declaran y publican.
Construida el 2026-08-11 a partir de **12 fabricantes** (Solmax, GSE, AGRU, NAUE, Atarfil,
Sotrafa, Maruplast, DM Geosintéticos, Pavco, Huitex, Layfield y la homologación peruana) —
ver [FUENTES.md](FUENTES.md) y el detalle punto por punto en
[datos-extraidos.csv](datos-extraidos.csv).

Dos columnas de referencia, que no hay que mezclar:

- **Mín. fábricas** — lo que los fabricantes *garantizan* (mínimos declarados/MARV, formato GM13).
- **Típicos** — lo que los fabricantes *declaran como valor típico o nominal de producción*.
  Es la columna contra la que comparar tu medida. ⚠ marca filas con una sola fuente (dato débil).

| Propiedad | Método | Unidad | Mín. GM13 | Mín. fábricas (rango) | Típicos (rango) | Típico (mediana) | n | Mi medida | Desvío vs típico |
|---|---|---|---|---|---|---|---|---|---|
| **Espesor y densidad** | | | | | | | | | |
| Espesor promedio | ASTM D5199 | mm | 1.50 | 1.35 – 1.52 ¹ | 1.50 | 1.50 | 2 | | |
| Espesor mínimo individual (de 10 lecturas) | ASTM D5199 | mm | 1.35 | 1.35 – 1.37 | — ² | — | 0 | | |
| Densidad | ASTM D1505 / D792 | g/cm³ | 0.940 | 0.940 – 0.942 | 0.940 – 0.942 | 0.941 | 2 | | |
| **Tracción (ASTM D6693 tipo IV)** | | | | | | | | | |
| Resistencia en fluencia | ASTM D6693 | kN/m | 22 | 20 – 27 | 22 – 25 | 23.5 | 4 | | |
| Resistencia en rotura | ASTM D6693 | kN/m | 40 | 30 – 43 ³ | 40 – 45 | 43 | 4 | | |
| Elongación en fluencia | ASTM D6693 | % | 12 | 12 – 13 | 12 – 15 | 12 | 5 | | |
| Elongación en rotura | ASTM D6693 | % | 700 | 600 – 800 | 700 – 800 | 750 | 5 | | |
| **Desgarre y punzonamiento** | | | | | | | | | |
| Resistencia al desgarre | ASTM D1004 | N | 187 | 180 – 249 | 187 – 215 | 195 | 5 | | |
| Resistencia al punzonamiento | ASTM D4833 | N | 480 | 400 – 640 | 480 – 550 | 480 | 5 | | |
| **Negro de humo, OIT y durabilidad** | | | | | | | | | |
| Contenido de negro de humo | ASTM D4218 | % | 2.0–3.0 (rango) | 2.0 – 3.0 | 2.5 ⚠ ⁴ | 2.5 | 1 | | |
| Dispersión de negro de humo | ASTM D5596 | categoría | 9 de 10 en Cat. 1–2 | Cat. 1–2 (todas las fichas) | Cat. 1–2 | Cat. 1–2 | 11 | | |
| OIT estándar | ASTM D3895 | min | 100 | 100 – 160 | 100 – 160 | 130 | 2 | | |
| OIT alta presión | ASTM D5885 | min | 400 | 400 – 800 | 800 ⚠ | 800 | 1 | | |
| Envejecimiento en horno 85 °C, 90 d (OIT retenido) | ASTM D5721 + D3895/D5885 | % | 55 (est.) / 80 (AP) | 55 – 80 | 55 ⚠ | 55 | 1 | | |
| Resistencia UV, 1600 h (OIT AP retenido) | ASTM D7238 + D5885 | % | 50 | 50 – 80 | — ⁵ | — | 0 | | |
| Agrietamiento por esfuerzo (SP-NCTL) | ASTM D5397 | h | 500 | 300 – 3000 ⁶ | 400 – 1000 | 500 | 3 | | |

*Desvío vs típico = (mi medida − típico) / típico × 100 %.*

## Notas

1. El rango de mínimos incluye fichas imperiales (60 mils = 1.524 mm) y una ficha que declara
   1.35 como promedio; la mediana declarada es 1.50.
2. Ninguna ficha declara valor típico del espesor mínimo individual; todas usan el −10 %
   normativo (1.35 mm).
3. El mínimo de 30 kN/m en rotura es de una ficha con GM13 antiguo; la mediana de mínimos
   declarados es 41 kN/m, alineada con GM13 vigente (40).
4. Negro de humo: solo Sotrafa declara valor de producción (2.25 ± 0.25 %); el resto da el
   rango 2.0–3.0 de norma.
5. Resistencia UV: ningún fabricante publica típico, solo el mínimo (≥50 %, y Sotrafa ≥55 %
   vía UNE-EN 728). Comparar contra el mínimo.
6. SCR: mínimos declarados de 300 h (fichas viejas) a 3000 h (líneas premium); GM13 vigente
   exige 500 h.

## Chequeo de coherencia contra la tabla de 1000 µm

| Propiedad | Típico 1.0 mm | Típico 1.5 mm | Cociente (esperado ≈1.5) |
|---|---|---|---|
| Tracción en fluencia | 16 | 23.5 | 1.47 ✓ |
| Tracción en rotura | 28 | 43 | 1.54 ✓ |
| Desgarre | 130 | 195 | 1.50 ✓ |
| Punzonamiento | 320 | 480 | 1.50 ✓ |
| Densidad / OIT / SCR (no escalan) | iguales | iguales | ✓ |

## Advertencias de lectura

- **Sesgo a la baja de los "típicos":** Pavco y Maruplast declaran como típico cifras iguales
  al mínimo GM13. Los típicos de NAUE, Sotrafa y DM Geosintéticos están por encima. El extremo
  alto del rango es mejor estimador de una producción sana que el bajo.
- **Métodos EN no comparables:** Sotrafa, Atarfil y GSE (EMEA) publican además valores UNE-EN
  ISO 527 (rotura 33 MPa / 900 % típico Sotrafa), ISO 34-1 (desgarre 225 N típico) y EN ISO
  12236 (punzonamiento CBR 3.9–4.5 kN, otro ensayo). **No** van en las columnas ASTM; están en
  [datos-extraidos.csv](datos-extraidos.csv) con `comparable_astm=no`.
- Aún sin valores **medidos** de lote (certificados de calidad): los candidatos están en
  FUENTES.md §B, pendientes de descarga con cuenta Scribd/Studocu — para 1.5 mm hay 4
  certificados detectados, incluido un informe de laboratorio completo (SCH21089).
