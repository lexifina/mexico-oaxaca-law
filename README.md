# Oaxaca: law history in git

The law of the State of Oaxaca (Estado Libre y Soberano de Oaxaca, Mexico) as a git history: one file per article, one commit per publication that changed it, dated the day it took effect, with the decree as the commit's author. `git blame` names the decree behind every paragraph; `git log` lists every change to an article; checking out a date gives the text in force that day.

It follows the shared design of [lexifina/global-law](https://github.com/lexifina/global-law), which places it at `mx-oax/`. Mexico's federal law is in [lexifina/mexico-law](https://github.com/lexifina/mexico-law).

The text is in Spanish, exactly as the source prints it.

## What this repository holds

58 ordenamientos with 961 versions so far: the constitution first, then the codes and laws in force, added in parts. Regulations, decrees and repealed laws are not included yet.

| Folder | Ordenamiento | Versions | History |
| --- | --- | ---: | --- |
| `constitucion-politica/` | CONSTITUCION POLITICA DEL ESTADO LIBRE Y SOBERANO DE OAXACA | 292 | as first published, then each reform: 4 April 1922 to 2 August 2026 |
| `codigo-civil/` | CODIGO CIVIL PARA EL ESTADO DE OAXACA | 104 | as first published, then each reform: 30 November 1944 to 2 August 2026 |
| `codigo-de-procedimientos-civiles/` | CODIGO DE PROCEDIMIENTOS CIVILES PARA EL ESTADO DE OAXACA | 50 | as first published, then each reform: 30 November 1944 to 14 March 2021 |
| `codigo-familiar/` | CODIGO FAMILIAR PARA EL ESTADO DE OAXACA | 10 | as first published, then each reform: 5 December 2021 to 2 August 2026 |
| `codigo-fiscal-municipal/` | CODIGO FISCAL MUNICIPAL DEL ESTADO DE OAXACA | 4 | as first published, then each reform: 10 May 2015 to 17 October 2021 |
| `codigo-fiscal/` | CODIGO FISCAL PARA EL ESTADO DE OAXACA | 16 | as first published, then each reform: 22 December 2012 to 10 December 2025 |
| `codigo-penal/` | CODIGO PENAL PARA EL ESTADO LIBRE Y SOBERANO DE OAXACA | 172 | as first published, then each reform: 7 November 1980 to 26 July 2026 |
| `ley-contra-la-violencia-y-acoso-entre-iguales/` | LEY CONTRA LA VIOLENCIA Y ACOSO ENTRE IGUALES PARA EL ESTADO DE OAXACA | 1 | as first published: 11 March 2015 |
| `ley-de-adopciones/` | LEY DE ADOPCIONES DEL ESTADO DE OAXACA | 4 | as first published, then each reform: 13 May 2017 to 31 July 2022 |
| `ley-de-adquisiciones-enajenaciones-arrendamientos-prestacion/` | LEY DE ADQUISICIONES, ENAJENACIONES, ARRENDAMIENTOS, PRESTACION DE SERVICIOS Y ADMINISTRACION DE BIENES MUEBLES E INMUEBLES DEL ESTADO DE OAXACA | 8 | as first published, then each reform: 12 November 2016 to 1 February 2026 |
| `ley-de-agua-potable-y-alcantarillado/` | LEY DE AGUA POTABLE Y ALCANTARILLADO PARA EL ESTADO DE OAXACA | 17 | as first published, then each reform: 14 February 1993 to 7 July 2024 |
| `ley-de-amnistia/` | LEY DE AMNISTIA PARA EL ESTADO DE OAXACA | 2 | as first published, then each reform: 9 December 2000 to 1 April 2001 |
| `ley-de-archivos/` | LEY DE ARCHIVOS PARA EL ESTADO DE OAXACA | 5 | as first published, then each reform: 16 February 2020 to 11 February 2024 |
| `ley-de-asistencia-y-prevencion-de-la-violencia-familiar/` | LEY DE ASISTENCIA Y PREVENCION DE LA VIOLENCIA FAMILIAR DEL ESTADO DE OAXACA | 2 | as first published, then each reform: 9 December 2017 to 9 March 2024 |
| `ley-de-bienes-pertenecientes-al-estado-de-oaxaca/` | LEY DE BIENES PERTENECIENTES AL ESTADO DE OAXACA | 7 | as first published, then each reform: 15 December 1951 to 12 December 2017 |
| `ley-de-cambio-climatico/` | LEY DE CAMBIO CLIMATICO PARA EL ESTADO DE OAXACA | 11 | as first published, then each reform: 29 November 2013 to 4 January 2026 |
| `ley-de-caminos-y-aeropistas-de-oaxaca/` | LEY DE CAMINOS Y AEROPISTAS DE OAXACA | 6 | as first published, then each reform: 28 May 1989 to 4 July 2024 |
| `ley-de-caminos-carreteras-y-puentes/` | LEY DE CAMINOS, CARRETERAS Y PUENTES PARA EL ESTADO DE OAXACA | 3 | as first published, then each reform: 15 April 2007 to 13 July 2025 |
| `ley-de-catastro/` | LEY DE CATASTRO PARA EL ESTADO DE OAXACA | 17 | as first published, then each reform: 17 December 1996 to 30 July 2025 |
| `ley-de-ciencia-tecnologia-e-innovacion/` | LEY DE CIENCIA, TECNOLOGIA E INNOVACION PARA EL ESTADO DE OAXACA - (ANTES LEY DE CIENCIA Y TECNOLOGIA PARA EL ESTADO DE OAXACA) - | 10 | as first published, then each reform: 13 April 2008 to 21 August 2022 |
| `ley-de-consulta-previa-libre-e-informada-de-los-pueblos-y-co/` | LEY DE CONSULTA PREVIA, LIBRE E INFORMADA DE LOS PUEBLOS Y COMUNIDADES INDIGENAS Y AFROMEXICANAS PARA EL ESTADO DE OAXACA | 2 | as first published, then each reform: 23 February 2020 to 3 March 2020 |
| `ley-de-coordinacion-estatal-de-las-zonas-economicas-especial/` | LEY DE COORDINACION ESTATAL DE LAS ZONAS ECONOMICAS ESPECIALES | 2 | as first published, then each reform: 18 October 2016 to 8 October 2017 |
| `ley-de-coordinacion-fiscal/` | LEY DE COORDINACION FISCAL PARA EL ESTADO DE OAXACA | 28 | as first published, then each reform: 1 January 2001 to 10 December 2025 |
| `ley-de-coordinacion-para-el-desarrollo-metropolitano-sustent/` | LEY DE COORDINACION PARA EL DESARROLLO METROPOLITANO SUSTENTABLE DEL ESTADO DE OAXACA | 2 | as first published, then each reform: 18 December 2011 to 29 November 2013 |
| `ley-de-coordinacion-para-el-fomento-del-aprovechamiento-sust/` | LEY DE COORDINACION PARA EL FOMENTO DEL APROVECHAMIENTO SUSTENTABLE DE LAS FUENTES DE ENERGIA RENOVABLE EN EL ESTADO DE OAXACA | 3 | as first published, then each reform: 4 April 2010 to 11 November 2018 |
| `ley-de-cultura-fisica-y-deporte/` | LEY DE CULTURA FISICA Y DEPORTE PARA EL ESTADO DE OAXACA | 9 | as first published, then each reform: 23 October 2019 to 24 May 2026 |
| `ley-de-derechos-de-los-pueblos-y-comunidades-indigenas-y-afr/` | LEY DE DERECHOS DE LOS PUEBLOS Y COMUNIDADES INDIGENAS Y AFROMEXICANO -- ANTES LEY DE DERECHOS DE LOS PUEBLOS Y COMUNIDADES INDIGENAS-- DEL ESTADO DE OAXACA | 11 | as first published, then each reform: 20 June 1998 to 4 January 2026 |
| `ley-de-desarrollo-cultural/` | LEY DE DESARROLLO CULTURAL PARA EL ESTADO DE OAXACA | 13 | as first published, then each reform: 29 August 2010 to 21 September 2025 |
| `ley-de-desarrollo-forestal-sustentable/` | LEY DE DESARROLLO FORESTAL SUSTENTABLE DEL ESTADO DE OAXACA | 8 | as first published, then each reform: 12 June 2013 to 7 September 2025 |
| `ley-de-desarrollo-rural-sustentable/` | LEY DE DESARROLLO RURAL SUSTENTABLE DEL ESTADO DE OAXACA | 16 | as first published, then each reform: 10 April 2012 to 23 February 2025 |
| `ley-de-deuda-publica/` | LEY DE DEUDA PUBLICA PARA EL ESTADO DE OAXACA | 11 | as first published, then each reform: 1 December 2017 to 16 December 2023 |
| `ley-de-educacion/` | LEY DE EDUCACION PARA EL ESTADO LIBRE Y SOBERANO DE OAXACA | 3 | as first published, then each reform: 12 April 2016 to 3 April 2022 |
| `ley-de-encierros-y-depositos-de-vehiculos/` | LEY DE ENCIERROS Y DEPOSITOS DE VEHICULOS PARA EL ESTADO DE OAXACA | 5 | as first published, then each reform: 9 December 2017 to 21 September 2025 |
| `ley-de-entidades-paraestatales/` | LEY DE ENTIDADES PARAESTATALES DEL ESTADO DE OAXACA | 12 | as first published, then each reform: 1 March 1998 to 18 August 2023 |
| `ley-de-entrega-recepcion-de-los-recursos-y-bienes/` | LEY DE ENTREGA-RECEPCION DE LOS RECURSOS Y BIENES DEL ESTADO DE OAXACA | 5 | as first published, then each reform: 21 October 2017 to 30 July 2023 |
| `ley-de-estimulos-y-recompensas-a-los-funcionarios-y-empleado/` | LEY DE ESTIMULOS Y RECOMPENSAS A LOS FUNCIONARIOS Y EMPLEADOS DEL GOBIERNO DEL ESTADO Y MAESTROS FEDERALIZADOS | 2 | as first published, then each reform: 21 July 1962 to 24 November 1984 |
| `ley-de-expropiacion/` | LEY DE EXPROPIACION DEL ESTADO DE OAXACA | 2 | as first published, then each reform: 30 December 1950 to 5 April 2026 |
| `ley-de-firma-electronica-avanzada/` | LEY DE FIRMA ELECTRONICA AVANZADA DEL ESTADO DE OAXACA | 2 | as first published, then each reform: 15 October 2016 to 16 November 2024 |
| `ley-de-fiscalizacion-superior-y-rendicion-de-cuentas/` | LEY DE FISCALIZACION SUPERIOR Y RENDICION DE CUENTAS DEL ESTADO DE OAXACA | 4 | as first published, then each reform: 1 October 2023 to 10 July 2025 |
| `ley-de-fomento-a-la-lactancia-materna-en-el-estado-de-oaxaca/` | LEY DE FOMENTO A LA LACTANCIA MATERNA EN EL ESTADO DE OAXACA | 3 | as first published, then each reform: 13 May 2017 to 10 August 2025 |
| `ley-de-fomento-a-las-actividades-artesanales/` | LEY DE FOMENTO A LAS ACTIVIDADES ARTESANALES DEL ESTADO DE OAXACA | 16 | as first published, then each reform: 27 April 2014 to 30 July 2023 |
| `ley-de-fomento-al-primer-empleo/` | LEY DE FOMENTO AL PRIMER EMPLEO PARA EL ESTADO DE OAXACA | 4 | as first published, then each reform: 9 December 2017 to 15 October 2023 |
| `ley-de-fomento-para-la-lectura-la-escritura-el-acceso-al-lib/` | LEY DE FOMENTO PARA LA LECTURA, LA ESCRITURA, EL ACCESO AL LIBRO Y LAS BIBLIOTECAS EN EL ESTADO Y MUNICIPIOS DE OAXACA | 4 | as first published, then each reform: 5 December 2021 to 22 March 2026 |
| `ley-de-hacienda-municipal/` | LEY DE HACIENDA MUNICIPAL DEL ESTADO DE OAXACA | 22 | as first published, then each reform: 2 September 1990 to 16 July 2023 |
| `ley-de-igualdad-entre-mujeres-y-hombres/` | LEY DE IGUALDAD ENTRE MUJERES Y HOMBRES PARA EL ESTADO DE OAXACA | 17 | as first published, then each reform: 26 April 2009 to 13 October 2024 |
| `ley-de-ingresos/` | LEY DE INGRESOS DEL ESTADO DE OAXACA PARA EL EJERCICIO FISCAL 2026 | 1 | as first published: 10 December 2025 |
| `ley-de-ingresos-del-municipio-de-concepcion-buenavista-distr/` | LEY DE INGRESOS DEL MUNICIPIO DE CONCEPCION BUENAVISTA, DISTRITO DE COIXTLAHUACA, OAXACA, PARA EL EJERCICIO FISCAL 2025 | 1 | oldest version available: 23 February 2025 |
| `ley-de-ingresos-del-municipio-de-heroica-ciudad-de-juchitan/` | LEY DE INGRESOS DEL MUNICIPIO DE HEROICA CIUDAD DE JUCHITAN DE ZARAGOZA, DISTRITO DE JUCHITAN, OAXACA, PARA EL EJERCICIO FISCAL 2024 | 1 | as first published: 17 February 2024 |
| `ley-de-ingresos-del-municipio-de-magdalena-zahuatlan-distrit/` | LEY DE INGRESOS DEL MUNICIPIO DE MAGDALENA ZAHUATLAN, DISTRITO DE NOCHIXTLAN, OAXACA, PARA EL EJERCICIO FISCAL 2025 | 1 | as first published: 16 March 2025 |
| `ley-de-ingresos-del-municipio-de-miahuatlan-de-porfirio-diaz/` | LEY DE INGRESOS DEL MUNICIPIO DE MIAHUATLAN DE PORFIRIO DIAZ, DISTRITO DE MIAHUATLAN, OAXACA, PARA EL EJERCICIO FISCAL 2025 | 1 | as first published: 9 March 2025 |
| `ley-de-ingresos-del-municipio-de-oaxaca-de-juarez-distrito-d/` | LEY DE INGRESOS DEL MUNICIPIO DE OAXACA DE JUAREZ, DISTRITO DEL CENTRO, OAXACA, PARA EL EJERCICIO FISCAL 2026 | 2 | as first published, then each reform: 17 January 2026 to 29 March 2026 |
| `ley-de-ingresos-del-municipio-de-salina-cruz-distrito-de-teh/` | LEY DE INGRESOS DEL MUNICIPIO DE SALINA CRUZ, DISTRITO DE TEHUANTEPEC, OAXACA, PARA EL EJERCICIO FISCAL 2025 | 1 | as first published: 20 April 2025 |
| `ley-de-ingresos-del-municipio-de-san-antonino-el-alto-distri/` | LEY DE INGRESOS DEL MUNICIPIO DE SAN ANTONINO EL ALTO, DISTRITO DE ZIMATLAN, OAXACA, PARA EL EJERCICIO FISCAL 2026 | 1 | as first published: 18 January 2026 |
| `ley-de-ingresos-del-municipio-de-san-antonino-monte-verde-di/` | LEY DE INGRESOS DEL MUNICIPIO DE SAN ANTONINO MONTE VERDE, DISTRITO DE TEPOSCOLULA, OAXACA, PARA EL EJERCICIO FISCAL 2025 | 1 | as first published: 23 March 2025 |
| `ley-de-ingresos-del-municipio-de-san-bartolome-loxicha-distr/` | LEY DE INGRESOS DEL MUNICIPIO DE SAN BARTOLOME LOXICHA, DISTRITO DE POCHUTLA, OAXACA, PARA EL EJERCICIO FISCAL 2026 | 1 | as first published: 1 February 2026 |
| `ley-de-ingresos-del-municipio-de-san-bartolome-quialana-dist/` | LEY DE INGRESOS DEL MUNICIPIO DE SAN BARTOLOME QUIALANA, DISTRITO DE TLACOLULA, OAXACA, PARA EL EJERCICIO FISCAL 2025 | 1 | as first published: 29 March 2025 |
| `ley-de-ingresos-del-municipio-de-san-dionisio-del-mar-distri/` | LEY DE INGRESOS DEL MUNICIPIO DE SAN DIONISIO DEL MAR, DISTRITO DE JUCHITAN, OAXACA, PARA EL EJERCICIO FISCAL 2025 | 1 | as first published: 16 March 2025 |
| `ley-de-ingresos-del-municipio-de-san-dionisio-ocotlan-distri/` | LEY DE INGRESOS DEL MUNICIPIO DE SAN DIONISIO OCOTLAN, DISTRITO DE OCOTLAN, OAXACA, PARA EL EJERCICIO FISCAL 2026 | 1 | as first published: 18 January 2026 |

## Source

The legislation compilation of Mexico's Supreme Court, the Suprema Corte de Justicia de la Nación (SCJN), at <https://legislacion.scjn.gob.mx/>. For each ordenamiento it lists every publication in the state's official gazette (Periódico Oficial) that changed it (decree, erratum, ruling), with the date of publication, the decree's extract and the whole consolidated text as it stood after that publication. Each version here is one of those texts.

## Dates

- Each commit is dated at **noon, America/Mexico_City, on the day the publication took effect**: the day its own transitorios name, as SCJN's extract quotes them (most often the day after publication). When a decree names none, 0 days after publication, the state rule SCJN cites.
- A consolidated text holds every change published before it, so it is never dated before the latest of their in-force days. Different in-force days for parts of one decree are not split.
- An act's first commit is its first publication when SCJN holds the original text; otherwise it is the oldest version SCJN holds.
- Versions that take effect after the retrieval day are on the `futuro` branch, never merged into `main`.

## Files

`<act>/art-005.md` is Artículo 5, `art-005-bis.md` Artículo 5 Bis; `encabezado.md` holds the title, the promulgation and preamble; `transitorios-original.md` the original transitory articles and `transitorios-<date>.md` those of the reform published that day. Section headings and editor's notes such as "(REFORMADO, P.O. ...)" stay in the file of the article they stand before. One paragraph per line.

## How it is checked

- Every version of every act is read back from git on the day it took effect and on the day before (`tools/check_repo.py`); both must match `corpus.json`.
- The letters and digits of every version equal those of SCJN's own text of that version (read independently of the parser), and every unit's text appears in it in order.
- Health checks: no merge commits, commit dates never go backwards, nothing dated in the future, and every commit's trailers parse.

## What "author" means

The author of a commit is the publication that changed the text (a decree, an erratum or a ruling), named by its category, gazette date and issue, with an e-mail address that cannot exist (`<key>@legislacion.scjn.gob.mx.invalid`). The committer is always Lexifina.

## Limits

This is not an official publication. The binding text is the one published in the state's official gazette (Periódico Oficial). The history starts with the oldest text SCJN holds for each ordenamiento, which for many is later than its enactment. Only the ordenamientos listed above are included.
