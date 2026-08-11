# Fuentes de los valores de referencia

Cada número de las tablas debe poder rastrearse a una entrada de esta lista. Tipos de dato:

- **medido** — resultado de ensayo real (certificado de calidad / MQC por lote / informe de laboratorio). La mejor fuente.
- **típico** — columna de valores típicos o declarados de una ficha técnica (distinta de la de mínimos).
- **mínimo** — ficha que solo declara mínimos/MARV estilo GM13. Sirve como piso, no como valor real.

Búsqueda web realizada el 2026-08-11 (78 fuentes candidatas únicas detectadas).

## A. Descargadas e incorporadas al repo (carpeta [`fuentes/`](fuentes/))

Descarga automática verificada el 2026-08-11. **Valores extraídos y volcados** a las tablas y a
[datos-extraidos.csv](datos-extraidos.csv) (563 puntos de dato con fabricante, valor original
impreso, valor convertido, naturaleza, método y si es comparable con la fila ASTM de la tabla).

Hallazgos del procesamiento:
- `naue-carbofol406-1500um-gm13.pdf` resultó ser **texturada** (BF/TF) — excluida de las tablas.
- `cedex-blanco-2013.pdf` es una lámina de **2.0 mm** con 16 años de envejecimiento y valores
  leídos de figuras — sirve de contexto, no para las tablas de 1.0/1.5.
- `geosynthetics-mag-2018.pdf` aportó 6 fabricantes adicionales con HDPE liso (AGRU, Atarfil,
  GSE, Huitex, Layfield, Solmax) + Raven (excluido, no es HDPE liso estándar).
- Las fichas europeas (Sotrafa, Atarfil, GSE EMEA, NAUE) traen además columnas de **valores
  típicos/declarados** según normas EN — de lo mejor que se consiguió sin certificados.

| Archivo | Fabricante | Espesor | Tipo esperado | Origen |
|---|---|---|---|---|
| `solmax-1000um-lisa-ldm.pdf` | Solmax | 1.0 mm | mínimo | [hubspot LDM](https://7800567.fs1.hubspotusercontent-na1.net/hubfs/7800567/LDM/HELP%20-%20LDM/Fichas%20t%C3%A9cnicas/Geomembranas/FT_SOLMAX%20HDPE%20Black%20Smooth%201.0MM.pdf) |
| `solmax-premium-hdpe.pdf` | Solmax | multiespesor | mínimo | [fergusonwaterworks.com](https://www.fergusonwaterworks.com/wp-content/uploads/2022/11/Solmax-Premium-HDPE.pdf) |
| `gse-hd-smooth-metric-emea.pdf` | GSE (Solmax) | multiespesor | mínimo | [media.assetfront.com](https://media.assetfront.com/20538/assets/86928/GzjCuDDqxcc0d4T1.pdf) |
| `gse-hd-smooth-product.pdf` | GSE (Solmax) | multiespesor | mínimo | [hdpe.ca](https://hdpe.ca/wp-content/uploads/2026/05/GSE-HD-Smooth-Product-Description-Sheet.pdf) |
| `agru-hd-smooth-2013.pdf` | AGRU America | 0.75/1.0/1.5 mm | mínimo | [fieldliningservices.com](https://fieldliningservices.com/wp-content/uploads/2015/10/2013-HD-smooth-data-sheet-AGRU.pdf) |
| `naue-carbofol406-1000um.pdf` | NAUE (Carbofol 406) | 1.0 mm | típico (EN/DIN) | [hubspot](https://f.hubspotusercontent10.net/hubfs/7800567/FT_CARBOFOL%20HDPE%20406%201,0%20ss.pdf) |
| `naue-carbofol406-1500um-gm13.pdf` | NAUE (Carbofol 406, BF/TF: ¿texturada?) | 1.5 mm | mínimo | [hubspot](https://f.hubspotusercontent10.net/hubfs/7800567/FT_CARBOFOL%20HDPE%20406%201,5%20BFTF%20GM13.pdf) |
| `naue-carbofol406-ss-gm13-rev11.pdf` | NAUE (Carbofol 406 lisa) | ? | mínimo | [altocy.com](https://altocy.com/wp-content/uploads/2019/08/2179-406-s-s-GM-13-Rev.11-eng.pdf) |
| `atarfil-hd.pdf` | Atarfil | multiespesor | típico (EN) | [geomembranasmexicanas.com](https://geomembranasmexicanas.com/wp-content/uploads/2015/09/Atarfil-HD.pdf) |
| `sotrafa-alvatech5002.pdf` | Sotrafa (Alvatech 5002) | multiespesor | típico (EN) | [sotrafa.com](https://sotrafa.com/documentos/Alvatech-5002.pdf) |
| `sotrafa-alvatech5002-ficha.pdf` | Sotrafa (Alvatech 5002) | multiespesor | típico (EN) | [sotrafageo.com](https://sotrafageo.com/wp-content/uploads/2021/10/Ficha-Te%CC%81cnica-ALVATECH-5002.pdf) |
| `sotrafa-catalogo-alvatech.pdf` | Sotrafa (catálogo Alvatech) | multiespesor | típico (EN) | [sotrafageo.com](https://sotrafageo.com/wp-content/uploads/2020/03/Cata%CC%81logo-GEOMEMBRANAS-ALVATECH-ESP.pdf) |
| `maruplast-ft-2024.pdf` | Maruplast (Perú) | multiespesor | mínimo | [maruplast.com](https://maruplast.com/wp-content/uploads/2024/10/Geomembrana-HDPE-FT-2024_2.pdf) |
| `maruplast-ft-2022.pdf` | Maruplast (Perú, rev. anterior) | multiespesor | mínimo | [maruplast.com](https://maruplast.com/wp-content/uploads/2024/01/Geomembrana-FT-2022.pdf) |
| `geosai-1000um.pdf` | GEOSAI (México) | 1.0 mm | mínimo | [geosai.com](https://www.geosai.com/fichas-tecnicas-SAI/GEOMEMBRANA-HDPE-SAI/Geomembrana%20HDPE%201mm%20SAI.pdf) |
| `dmgeo-1500um.pdf` | DM Geosintéticos (México) | 1.5 mm | mínimo | [dmgeosinteticos.mx](https://www.dmgeosinteticos.mx/wp-content/uploads/2025/05/FICHA-TECNICA-GEOMEMBRANA-HDPE-1.5-MM.pdf) |
| `pavco-geomembranas-2021.pdf` | Pavco Wavin (Colombia) | multiespesor | mínimo (MARV) | [geosoftpavco.com](https://www.geosoftpavco.com/pdf/fichas/2021-DIC/Pavco/Geomembranas_FT2021.pdf) |
| `gobpe-homologacion-1mm.pdf` | Perú Compras (homologación estatal) | 1.0 mm | mínimo | [gob.pe](https://cdn.www.gob.pe/uploads/document/file/5973908/5293373-ficha-geomembrana-de-hdpe-de-1mm.pdf) |
| `geosynthetics-mag-2018.pdf` | Varios (guía comparativa 2018) | multiespesor | mínimo | [geosyntheticsmagazine.com](https://geosyntheticsmagazine.com/wp-content/uploads/sites/26/2018/02/Geomembranes_2018.pdf) |
| `cedex-blanco-2013.pdf` | CEDEX / Zornberg (ensayos en embalses) | ? | **medido** | [sites.utexas.edu](https://sites.utexas.edu/zornberg/wp-content/uploads/sites/5286/2022/03/Blanco_Noval_Garcia_Martin_Aguiar_Vara_Zornberg_2013.pdf) |

## B. Requieren cuenta Scribd/Studocu — descarga manual del usuario

Los documentos más valiosos: **certificados de calidad con valores medidos por lote**.
Descargar con cuenta propia y subir a [`fuentes/`](fuentes/).

### Prioridad alta — certificados con valores medidos

| Documento | Espesor | Link |
|---|---|---|
| Certificado de calidad HDPE liso nominal 1.00 mm, OF 150920, 20 rollos (TDM) | **1.0 mm** | [scribd 394031756](https://www.scribd.com/document/394031756/Certificado-de-Calidad-HDPE-Liso-Nominal-1-00-Mm-of-150920-01-Al-20-20-Rollos) |
| Certificado de calidad geomembrana HDPE 1 mm — NUVACORP / Lares | **1.0 mm** | [studocu 127973711](https://www.studocu.com/pe/document/universidad-tecnologica-del-peru/resistencia-de-materiales/certificado-de-calidad-geomembrana-hdpe-1mm-lares-grupo-inmobiliario/127973711) |
| Certificado de calidad geomembrana HDPE liso GM13 1.50 mm (rollo 210×7.01 m) | **1.5 mm** | [scribd 536962713](https://www.scribd.com/document/536962713/01-Certificado-de-calidad-Geomembrana-HDPE-Liso-GM13-1-50-mm) |
| CC geomembrana HDPE 1.5 mm lisa 7×140 m, 16 rollos (Delta) | **1.5 mm** | [scribd 554251868](https://www.scribd.com/document/554251868/09-21-CC-Geomembrana-HDPE-1-5mm-Lisa-de-7x140m-Nominal-16R-163376) |
| CC geomembrana HDPE 1.5 mm lisa 7×140 m, 16 rollos (Nortene/Cidelsa) | **1.5 mm** | [scribd 554251708](https://www.scribd.com/document/554251708/09-21-CC-Geomembrana-HDPE-1-5mm-Lisa-de-7x140m-Nominal-16R-163376-1) |
| Informe de laboratorio HDPE 1.5 mm SCH21089 (espesor, densidad, tracción, desgarre, punzonamiento, negro de humo, SCR) | **1.5 mm** | [scribd 728499721](https://www.scribd.com/document/728499721/1-5mm-SCH21089-final) |
| Certificado PQA geomembrana (fabricada 04-05-2019) | ¿? | [scribd 559329763](https://www.scribd.com/document/559329763/certificado-PQA-GEOMEMBRANA) |
| Certificado de calidad HDP (espesor medido 1.35/1.32 mm → ¿nominal 1.5?) | ¿1.5 mm? | [scribd 545684537](https://www.scribd.com/document/545684537/CERTIFICADO-DE-CALIDAD-HDP) |

### Prioridad media — más certificados y fichas por verificar

| Documento | Espesor | Link |
|---|---|---|
| Nortene HDPE lisa 1500 Cidelsa nominal | 1.5 mm | [scribd 554251873](https://es.scribd.com/document/554251873/Nortene-Hdpe-Lisa-1500-Cidelsa-Nominal-1) |
| Certificado de calidad de geomembrana (GHDPE075LN, ¿0.75 mm?) | ¿0.75 mm? | [scribd 510281669](https://www.scribd.com/document/510281669/CERTIFICADO-DE-CALIDAD-DE-GEOMEMBRANA) |
| Certificado de conformidad HDPE lisa Cal 40 | 1.0 mm | [scribd 808728072](https://www.scribd.com/document/808728072/CERTIFICADO-DE-CONFORMIDAD-GEOMEMBRANA-HDPE-LISA-CAL-40) |
| Certificado de calidad LLDPE 1.00 mm serie 2486-12 (comparativo, no HDPE) | 1.0 mm | [scribd 346752924](https://www.scribd.com/document/346752924/Certificado-de-Calidad-fact-0001-000184-Liso-LLPE-Serie-2486-12-1-00mm-01-rollos-1-pdf) |
| Certificado 1521 — Grupo Verqro (verificar contenido) | ¿? | [scribd 573800467](https://www.scribd.com/document/573800467/Certificado-1521-Grupo-Verqro-s-de-Rl-de-Cv) |
| Certificado de calidad geomembrana y accesorios — SKINLAND | 1.0 mm | [studocu 115206883](https://www.studocu.com/pe/document/universidad-nacional-del-centro-del-peru/tecnologia-de-los-materiales/certificado-de-calidad-de-geomenbrana-y-otros-accesorios/115206883) |
| Ficha técnica GSE en español (mín. promedio por rollo) | multiespesor | [scribd 462458517](https://www.scribd.com/document/462458517/Ficha-Tecnica-Geomembrana-HDPE-GSE-espanol) |
| FT HDPE 1.5 mm lisa (con rangos admisibles) | 1.5 mm | [scribd 531861960](https://www.scribd.com/document/531861960/FT-GEOMEMBRANA-HDPE-1-5MM-LISA) |
| FT HDPE lisa 1.50 mm (propiedades completas) | 1.5 mm | [scribd 469142748](https://www.scribd.com/document/469142748/GEOMEMBRANA-HDPE-LISA-1-50mm) |
| FT HDPE 1.5 mm | 1.5 mm | [scribd 776126151](https://www.scribd.com/document/776126151/FICHA-TECNICA-GEOMEMBRANA-HDPE-DE-1-50MM) |
| FT HDPE 1.0 mm | 1.0 mm | [scribd 719114629](https://www.scribd.com/document/719114629/FICHA-TECNICA-GEOMEMBRANA-HDPE-DE-1-0MM) |
| FT HDPE 1.5 mm lisa nominal | 1.5 mm | [scribd 736306260](https://www.scribd.com/document/736306260/FICHA-TECNICA-HDPE-DE-1-5MM-LISA-NOMINAL) |
| FT HDPE lisa 1.00 mm GMA | 1.0 mm | [scribd 241267757](https://www.scribd.com/doc/241267757/Geomembrana-Hdpe-Lisa-1-00mm-Gma) |
| FT HDPE todos los espesores, 7 m de ancho | multiespesor | [scribd 502610805](https://www.scribd.com/document/502610805/Ficha-Tecnica-GEOMEMBRANA-HDPE-todos-los-espesores-7-ancho) |
| EETT HDPE lisa 1.00 mm — Geoace Perú | 1.0 mm | [studocu 21149693](https://www.studocu.com/pe/document/universidad-continental/materiales-de-construccion/eett-geomembrana-nominal-hdpe-lisa-100-mm-geoace-peru-sac/21149693) |
| Manual de control de calidad para geomembranas HDPE (contexto MQC) | multiespesor | [studocu 103083992](https://www.studocu.com/cl/document/pontificia-universidad-catolica-de-chile/construccion-civil/720582635-manual-de-control-de-calidad-geomembrana/103083992) |

## C. Páginas de fabricantes (portal de descarga, sin PDF directo en la búsqueda)

| Fabricante | Link |
|---|---|
| Atarfil HD (oficial) | https://www.atarfil.com/producto/atarfil-hd/ |
| TDM Perú | https://www.tdm.com.pe/products-geosinteticos-geomembranas-polietileno/ |
| Cidelsa Perú | https://www.cidelsa.com/en/productos/geomembrana-de-polietietileno-pe/ |
| Coripa Argentina | https://coripa.com.ar/geomembranas/ |
| Polytex Chile | https://www.polytex.cl/en/categorias/geomembranas-y-geotextiles/geomembrana-de-polietileno-de-alta-densidad-hpde |
| BPM (China) — HDPE 1.5 mm | https://www.bpmgeo.com/hdpe-geomembrane/hdpe-geomembrane-1.5mm |
| BPM (China) — línea HDPE | https://www.bpmgeomembrane.com/geomembranes/high-density-polyethylene-geomembrane/ |
| Tinhy (China) — HDPE lisa | https://tinhygeosynthetics.com/geosynthetics-products/geomembranes/smooth-hdpe-geomembranes/ |
| Tinhy (China) — guía de especificaciones | https://tinhygeosynthetics.com/resources/geosynthetic-knowledge-base/hdpe-geomembrane-specifications/ |
| Geosino (China) — comparativa 1.5 mm | https://www.geosyntheticscn.com/the-8-best-hdpe-geomembrane-1-5-mm-list |
| hyhdpemembrane (China) — certificados y test reports | https://www.hyhdpemembrane.com/certificates-polyethylene-geomembrane/ |
| hyhdpemembrane (China) — HDPE 1.0–2.0 mm | https://www.hyhdpemembrane.com/product/hdpe-geomembrane-liner/ |
| Sotrafageo — cómo leer la ficha Alvatech | https://sotrafageo.com/en/interpretation-of-the-alvatech-geomembrane-technical-data-sheet/ |

## D. Académicas con valores medidos (papers y tesis)

| Documento | Acceso | Link |
|---|---|---|
| CEDEX, Ing. Civil 120: características iniciales medidas de geomembranas de embalses | libre | https://hispagua.cedex.es/sites/default/files/hispagua_articulo/Ingcivil/2000/120/articulo2/articulo.htm |
| MDPI Polymers: fluencia y tracción medidas en HDPE (probetas 0.5/1.5 mm) | libre | https://doi.org/10.3390/polym16142019 |
| PMC: efecto UV sobre HDPE — tracción y OIT medidos | libre | https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8226566/ |
| PMC: tracción y punzonamiento de HDPE bajo lixiviado | libre | https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5452658/ |
| ScienceDirect: vida útil de geomembranas HDPE 1.5 mm (OIT medido) | resumen libre | https://www.sciencedirect.com/science/article/pii/S2214509523003923 |
| ASCE: conformidad de HDPE contra GRI-GM13 (¡valores de producción vs norma!) | de pago | https://ascelibrary.org/doi/10.1061/40782(161)58 |
| ScienceDirect: punzonamiento HDPE 1.5 mm sobre arcilla con piedras | de pago | https://www.sciencedirect.com/science/article/abs/pii/S0266114410000075 |
| Academia.edu: tracción de HDPE vs temperatura y químicos | requiere cuenta | https://www.academia.edu/26049074/Evaluation_of_Tensile_Properties_of_HDPE_Geomembranes_with_Temperature_under_Exposure_to_Chemical_Solutions |
| Tesis UPN: corte y desgarro en soldaduras HDPE | libre (página) | https://repositorio.upn.edu.pe/handle/11537/21770 |
| Tesis UNAM Moquegua: QA/QC de instalación de HDPE | libre (página) | https://repositorio.unam.edu.pe/items/f21dd692-72d5-4a9c-8a56-93e9bd2c67dd |

## E. No accesibles desde esta sesión

| Documento | Motivo |
|---|---|
| Solmax HDPE métrica y GSE HD High Performance en geosindex.com | dominio bloqueado por el proxy |
| TCS Geotechnics 1.0 mm (UK) | captcha del sitio |
| Tesis UPN PDF directo (bitstream) | el repositorio devuelve página HTML, no el PDF |
| Solmax GSE HD (solmax.com), AGRU.com, NAUE.com oficiales | dominios bloqueados por el proxy (la vía WebFetch); reintentarlos vía curl en próxima pasada |

## Referencia normativa

- GRI-GM13, *Test Methods, Test Properties and Testing Frequency for High Density
  Polyethylene (HDPE) Smooth and Textured Geomembranes*, Geosynthetic Institute.
  Origen de la columna "Mín. GRI-GM13" de ambas tablas.
