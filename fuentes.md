---
expediente: "MPF00462972"
---

# Fuentes: archivos enviados por la Fiscalía

Dos zips con la documentación de la causa. Ambos descomprimen en la carpeta `Piñero/`.

| | wetransfer-535d56.zip | Filemail.com files 2020-8-3 zatwleekkuykixs.zip |
|---|---|---|
| Servicio | WeTransfer | Filemail (fecha en el nombre: 2020-08-03) |
| Tamaño | 63 941 135 bytes | 71 913 483 bytes |
| Archivos | 100 | 114 |
| Compresión | ninguna (stored) | ninguna (stored) |
| Generador | ZipTricks 4.8.2 (comentario del zip) | sin comentario; sistema FAT (Windows) |
| Fecha interna de los archivos | 2020-07-13 21:23:04 UTC (igual para todos; es la fecha de armado del zip, no la de cada documento) | 2020-08-02 22:20:34 a 22:23:34, hora local -03 (56 marcas distintas; fecha de copia al zip) |
| Fecha del archivo en disco | 2020-07-30 | 2020-08-02 |

## Contenido

- Tipos: wetransfer 91 pdf, 4 jpg, 3 wav, 1 mp3, 1 docx. Filemail 105 pdf, 4 jpg, 3 wav, 1 mp3, 1 docx.
- Los 100 archivos de wetransfer están todos en Filemail con contenido idéntico (comparado por MD5).
- Filemail tiene 14 pdf que no están en wetransfer:
  - 986585 CEDS.pdf
  - 986585 R informe Nicolas Kosciuk.pdf
  - 986585 Rta. UFO (Notificación N° 1930).pdf
  - boletin oficial kuchasky.pdf
  - boletin oficial kuchasky 18-5-20.pdf
  - boletin oficial kuchasky 19-5-20.pdf
  - correo kosciuk.pdf
  - correo kosciuk 31 7 20.pdf
  - correo y respuesta denunciante kosciuk.pdf
  - Fiscalía PCyF Nro. 20 - Notifica resolución s_ caso _HOSPITAL PIÑERO_.pdf
  - mail harari.pdf
  - mail harari pide copias.pdf
  - mail harari solicita nuevo enlace de descarga y respuesta dada.pdf
  - mail kosciuk a perito del cij diletto.pdf
- Dentro de cada zip hay archivos repetidos con distinto nombre (94 contenidos distintos en 100 archivos del zip de wetransfer; 108 en los 114 de Filemail).

## Historia clínica

Los 7 PDF `historia clinica parte 1..7 (1).pdf` (284, 32, 58, 36, 2, 1 y 12 páginas; 425 en total) están en `historia_clinica/historia_clinica_1..7.pdf` (`_1a` y `_2a`: versiones redacted de `_1` y `_2`, misma paginación). Las 252 páginas útiles están en `historia_clinica/fojas/` y `transcripciones/`; las demás se detallan en `historia_clinica/eliminadas.md`.

SHA-256 de `historia_clinica_N.pdf`:

1. 83bc1fcf8ee189f2ddfcd7b0563d9e47249215b7ee2ad82c45297ca56da85e8e
2. fb88783634608b3d97b5f90fbcec7ccb781316a4121a243aeef9e12597cf92ff
3. 0700e7339be2b46d2b1d5625cb40412326cfc24b7027c80a3f293a70b274d80f
4. d927fce0da8fb469c4ae8b81cd5df319c9da07decdf410c73a2bd3b061d5fe19
5. e6197c7e4163c9cc8715c4b5c88d26330e90b93aff34f79f11e2b50b035487fb
6. e6ff2e4716a4c31331891f85f97bb2688e6d5d8b1a4d456e7f033d5ffa27a061
7. 38a424bfc02547e6279074d72dc59d81f0c9b1bb0da52435a6f53ad5a095d8f4

## Archivos excluidos del repo

- `DNI KOSCIUK (1) (1).pdf` y `DNI KOSCIUK (2) (2).pdf`: documento de identidad del denunciante; dato personal que no aporta a la investigación.
- `IMG-20200612-WA0006.jpg`: partida de nacimiento del denunciante; dato personal que no aporta a la investigación.
- `Documento 45 (1) (3).pdf` y `Documento 49 (17) (1).pdf`: documentos de identidad del denunciante y de su abogado; datos personales que no aportan a la investigación.
- `boletin oficial kuchasky.pdf`, `boletin oficial kuchasky 18-5-20.pdf` y `boletin oficial kuchasky 19-5-20.pdf`: publicaciones del Boletín Oficial; son de dominio público, ocupan espacio y no hacen a la investigación.
- `MPF-_20200214_02102604 (1).pdf`: 134 páginas sobre la detención de otra persona, con intervención del mismo fiscal, todo del 12 de febrero de 2020; corresponde a otro expediente, enviado por error.

## Metadatos de los PDF

La fecha interna del zip no sirve para fechar los documentos. Para fecharlos se usa el texto del PDF o su `CreationDate` (`pdfinfo`). Programa generador (`Creator`/`Producer`) de los 99 PDF distintos y qué indica:

| Generador | PDF | Indicio |
|---|---|---|
| wkhtmltopdf 0.12.4 (con o sin iText 5.4.5) | 28 | Sistema de la Fiscalía (proveídos, decretos, informes `MPF00462972_*`); CreationDate entre 2020-05-12 y 2020-06-12 |
| Chrome 83/84 (Skia/PDF) | 32 | Páginas web o mails impresos desde Chrome en Windows 10; entre 2020-06-10 y 2020-08-02 |
| RICOH MP 501 | 7 | Escaneos de documentos en papel; 2020-05-26 |
| PDFium | 4 | Impresión desde visor PDF de Chrome/Edge; 2020-05-04 a 2020-06-10 |
| Microsoft Word 2010/2013/2016 | 6 | Documentos redactados en Word; 2020-06-06 a 2020-07-28 |
| Microsoft Print To PDF | 3 | Impresión desde Windows; 2020-06-29 |
| iText 4.2.0 / 5.5.6 / LiveCycle ES2-ES3 | 7 | Documentos oficiales (notificaciones, boletín oficial); 2020-04-30 a 2020-06-24 |
| RxRelease / Haru 2.4.0 | 4 | Sin Creator ni fecha |
| Otros (PScript5/Acrobat Distiller, Writer, TCPDF, PaperPort 14, Kodak) | 8 | Un documento cada uno, sin patrón común |

## Archivos originales

MD5 de cada archivo de `Piñero/` y su ubicación en el repo.

| MD5 | Nombre original | Ubicación |
|---|---|---|
| 839acf4b2cd32057a5590b97f2e13e51 | 986585 CEDS.pdf | `2020/07/28/memo_respuesta_notificacion_1930.pdf` |
| 80245161de138ae19e3e5e6577b4df7a | 986585 R informe Nicolas Kosciuk.pdf | `2020/04/30/informe_coord_salud_sobre_denunciante.pdf` |
| be9aa86072e02199eddbe1a366a5346e | 986585 Rta. UFO (Notificación N° 1930).pdf | `2020/07/15/defensor_pueblo_respuesta_a_ufo.pdf` |
| 1c94b2aab147c21f38ea1c32010a5461 | CREDENCIAL DR HARARI CAUSA MPF 462972 (1).pdf | `2020/06/08/correo_harari_credencial.pdf` |
| ccf562c24e3c0922ff179fcf1d645dc6 | Consulta sobre cuerpo.pdf | `2020/06/22/correo_consulta_sobre_cuerpo.pdf` |
| 0d719f614cccccf1ac930927b0831abd | Correo - RBranca@fiscalias.gob.ar 2 (1).pdf | `2020/06/07/correo_denunciante_responde_a_sosa.pdf` |
| 1ecd6abdcdc416fdd1829c5e71965743 | Correo - RBranca@fiscalias.gob.ar 3 (1).pdf | `2020/06/08/correo_branca_informa_imputacion_y_allanamiento.pdf` |
| 002b80de592eea4ef325161021433e9f | Correo - RBranca@fiscalias.gob.ar 4 (1).pdf | `2020/06/08/correo_denunciante_pesar_cadaver.pdf` |
| d45042fa41f89fbf02f1f99ff5f48c90 | Correo - RBranca@fiscalias.gob.ar 5 (1).pdf | `2020/06/08/correo_denunciante_pide_acceso_documentos.pdf` |
| abb5e2c2b119271cbe7f97b2b0928d1c | Correo - RBranca@fiscalias.gob.ar 6 (1).pdf | `2020/06/09/correo_denunciante_sugiere_contactar_a_miguel.pdf` |
| b1098e66eaf142f2860c01222282b4d3 | Correo - RBranca@fiscalias.gob.ar 7 (1).pdf | `2020/06/09/correo_denunciante.pdf` |
| 526433a72ed161633f8de9acd678de3b | Correo - RBranca@fiscalias.gob.ar informe Omar (1).pdf | `2020/06/10/correo_more_envia_informe_cij.pdf` |
| 2039444df00a0dda181853f7ad449a4e | Correo - RBranca@fiscalias.gob.ar nuevo correo 18-6 (1).pdf | `2020/06/18/correo_denunciante_ofrece_ayuda_investigar.pdf` |
| 622d7d06dbbcbca6175698adbe132c4a | DNI KOSCIUK (1) (1).pdf | excluido |
| 622d7d06dbbcbca6175698adbe132c4a | DNI KOSCIUK (2) (2).pdf | excluido |
| 93d85d8b8fd0c93f93199e63e605945b | DNI QUERELLANTE CUSA MPF 462972 (1).pdf | `2020/06/08/correo_harari_dni_querellante.pdf` |
| 84a3aef759735acf60ea09e407890b32 | Documento 45 (1) (3).pdf | excluido |
| 509d682fec28b462033a3f9b28c1d0af | Documento 46 (1) (5).pdf | `2020/05/05/denuncia_penal_escaneo.pdf` |
| c291d7904ad0039ce104502248ae9810 | Documento 49 (1) (1).pdf | `2020/06/08/querella_constitucion_escaneo.pdf` |
| 5ec5542efe121fa5a4d49b5b53434863 | Documento 49 (17) (1).pdf | excluido |
| 69495d318832e42a67f55085a30d1943 | FW_ Causa Kuchasky (1).pdf | `2020/06/16/correo_rozas_reenvia_informe_diletto.pdf` |
| 2df09e36bb140e62fab6bc62d8fffaa0 | Fiscalía PCyF Nro. 20 - Notifica resolución de Juzgado relativa a petición de querella.pdf | `2020/06/22/correo_pide_expediente_digital_para_abogado.pdf` |
| cd96faf446fb9e8982b7835ca111f2d7 | Fiscalía PCyF Nro. 20 - Notifica resolución s_ caso _HOSPITAL PIÑERO_.pdf | `2020/07/30/correo_fiscalia_notifica_resolucion_caso.pdf` |
| 9253670f98e87762a8cf9c6c9468b779 | GAP_375825.pdf | `den00641871/2020/06/29/oficio_policia_consulta_llamados_911.pdf` |
| 94717ef210eb5a9db0a5e70385768cb0 | GRABADO 25-3-2020 HORA 13.16.30 ABONADO N° 1124020854 SUCESO N° 30489464.wav | `den00641871/2020/03/25/llamada_911_131630_suceso_30489464.wav` |
| 9c6a7a246b32d187ec224af97543dd5d | GRABADO 25-3-2020 HORA 20.09.02 ABONADO N° 1124020854 SUCESO N° 30493529.mp3 | `den00641871/2020/03/25/llamada_911_200902_suceso_30493529.mp3` |
| 4a21da57b7ef55fde0a1a2fe3dfd6ca4 | GRABADO 25-3-2020 HORA 20.21.58 ABONADO N° 1124020854 SUCESO N° 30493637.wav | `den00641871/2020/03/25/llamada_911_202158_suceso_30493637.wav` |
| ee5faeacc099dcc0c9559ccb847b6c1b | GRABADO 25-3-2020 HORA 20.45.54 ABONADO N° 1124020854 SUCESO N° 30493810.wav | `den00641871/2020/03/25/llamada_911_204554_suceso_30493810.wav` |
| 7cdf63408bdb75712dfeccf4c1b8a980 | IF-2020-15059541-GCABA-DGEVYC (1).pdf | `2020/06/09/informe_gedo_espacios_verdes.pdf` |
| dcd5476ae2c512fd4d6a4421122d9795 | IF-2020-15091431-GCABA-DGEVYC (1).pdf | `2020/06/10/informe_espacios_verdes_ubicacion_cuerpo.pdf` |
| b20fdb40d0c882fe5e068d0ad724bcf2 | IMG-20200612-WA0006.jpg | excluido |
| c96608bc21e9ad6ea8932fbac83fe9cc | Informe auxiiar Cij 63177 (1).pdf | `2020/07/03/informe_auxiliar_cij_gabinete_medico.pdf` |
| c96608bc21e9ad6ea8932fbac83fe9cc | Informe auxiiar Cij 63177.pdf | `2020/07/03/informe_auxiliar_cij_gabinete_medico.pdf` |
| eb01c1e33a45b3410a58edb9749af69d | Intervencion CIJ 63358 (kosciuk).pdf | `2020/07/03/informe_auxiliar_cij_gabinete_psicologico.pdf` |
| 9b198c7c747cf1b138e4fdfbb0fbd8f3 | Kuchasky (2).pdf | `2020/06/10/informe_medicolegal_cij.pdf` |
| 3ea3da09e555ef72a20a2b100e1985eb | Kuchasky Margarita (1).pdf | `2020/04/30/acta_defuncion.pdf` |
| 3ea3da09e555ef72a20a2b100e1985eb | Kuchasky Margarita (2) (1).pdf | `2020/04/30/acta_defuncion.pdf` |
| c568a76e86037a7c2637a2321f18a098 | MPF 462972 (2).pdf | `2020/06/10/correo_peretti_adjunta_informe_medicolegal.pdf` |
| 011808054d95ea3e523034f1285e3e81 | MPF-_20200214_02102604 (1).pdf | excluido |
| d01963e86e69c7c7c2fb093c823d46e9 | MPF00462972_Art._108.-_L_2303._Causales_para_el_allanamiento__Solicitud_1589315463 (1).pdf | `2020/05/12/fiscalia_solicitud_allanamiento_hospital.pdf` |
| 0ec8649341dbc7fc698fee63c55145a7 | MPF00462972_Art._11.-_L_2303_Legitimación._Oportunidad__Constitución_Querella_-_Interesado_sin_legitimación_1592938029.pdf | `2020/06/23/fiscalia_resolucion_peticion_querella.pdf` |
| b89a395a755ee3cafa5dab1720e873a0 | MPF00462972_Art._92.-_L_2303._Decreto_de_determ._de_hechos__Fijación_objeto_Procesal_(Múltiples_Personas)_1589303349 (2).pdf | `2020/05/12/fiscalia_decreto_objeto_procesal_inicial.pdf` |
| e75f17bd139d02f3ea18c44daf9fc62b | MPF00462972_Art._92.-_L_2303._Decreto_de_determ._de_hechos__Fijación_objeto_Procesal_(Múltiples_Personas)_1592505215 (1).pdf | `2020/06/18/fiscalia_decreto_objeto_procesal_modificado.pdf` |
| e75f17bd139d02f3ea18c44daf9fc62b | MPF00462972_Art._92.-_L_2303._Decreto_de_determ._de_hechos__Fijación_objeto_Procesal_(Múltiples_Personas)_1592505215.pdf | `2020/06/18/fiscalia_decreto_objeto_procesal_modificado.pdf` |
| 33243b5811946d2fbc0f53e72fb3466f | MPF00462972_Certificado_de_causa___otros_1592319150.pdf | `2020/06/16/fiscalia_certificado_correo_diletto.pdf` |
| b0c1fbec47e7df5f9982c5fefe6ffb3c | MPF00462972_Informe_del_investigador_1591708584.pdf | `2020/06/09/informe_investigador_correos_querella.pdf` |
| a69f687ff3f206e3e214137f20a9cdf3 | MPF00462972_Informe_del_investigador_1591808563.pdf | `2020/06/10/informe_investigador_correos_peretti_maffuchi.pdf` |
| 696c768a5999591ef9def84ce41c28d4 | MPF00462972_Informe_del_investigador_1591877299.pdf | `2020/06/11/informe_investigador_correos_denunciante.pdf` |
| 6db562a1f94bc142848724321cf5f869 | MPF00462972_Informe_del_investigador_1591877598.pdf | `2020/06/11/informe_investigador_correo_more.pdf` |
| f67ba2fe97a680ee4ebd2afbf3c4172b | MPF00462972_Informe_del_investigador_1591969796 (1).pdf | `2020/06/12/informe_investigador_notificacion_a_harari.pdf` |
| 7b24b6371014998e5692097ba2439156 | MPF00462972_Informe_del_investigador_1592484529.pdf | `2020/06/18/informe_investigador_correo_denunciante.pdf` |
| da04278f069bf4cdea2f43b48d402ef7 | MPF00462972_Informe_del_investigador_1592925210.pdf | `2020/06/23/informe_investigador_correos_pretende_querella.pdf` |
| 3dd708f6e6a8a7878d4442ca7187b0de | MPF00462972_Informe_del_investigador_1592925336.pdf | `2020/06/23/informe_investigador_dos_correos_denunciante.pdf` |
| 0bb33e482f5c853dc4b6743d3cd6d4b1 | MPF00462972_Informe_del_investigador_1593468528.pdf | `2020/06/29/informe_investigador_declina_competencia_pami.pdf` |
| f800a64df1b92e800b9a39011b511f4f | MPF00462972_Informe_del_investigador_1593545096.pdf | `2020/06/30/informe_investigador_contactos_kiwi.pdf` |
| 7fe0a497fc83c2d4d9b9577308ba42a3 | MPF00462972_Intervención_de_Juzgado_Diligencia_con_firma_de_Juez_1592516010 (1).pdf | `2020/06/18/fiscalia_remite_a_juzgado_21_rechazo_querella.pdf` |
| 408ed0d3517a3d1a903230cff7b134a2 | MPF00462972_Intervención_de_Juzgado_Diligencia_con_firma_de_Juez_1593195266.pdf | `2020/06/26/fiscalia_discrepa_con_jueza_sobre_querella.pdf` |
| 8bff47fb0dbb6748c1203a0f4509710d | MPF00462972_Proveido_simple_1589303914 (1).pdf | `2020/05/12/proveido_requiere_intervencion_cij.pdf` |
| 6e534b459c1adde3ef388810b6b38bea | MPF00462972_Proveido_simple_1589314749.pdf | `2020/05/12/proveido_deja_sin_efecto_orden_presentacion.pdf` |
| 991ab4df69737f4a6e5ef9869ff0bc7c | MPF00462972_Proveido_simple_1589556888 (1).pdf | `2020/05/15/proveido_requiere_cij_tras_juzgado_21.pdf` |
| 678cd6e9cb25044b5f05577029dc4d83 | MPF00462972_Proveido_simple_1589557046 (2).pdf | `2020/05/15/orden_presentacion_cij_historia_clinica.pdf` |
| 5fc56b07f613b31054bc0dc9d88a76b0 | MPF00462972_Proveido_simple_1591632035 (1).pdf | `2020/06/08/proveido_intervencion_gabinete_medico_cij.pdf` |
| df0c29485d74d4fd8f826f259a7591d7 | MPF00462972_Proveido_simple_1591968761 (1).pdf | `2020/06/11/proveido_querella_ilegible_y_partida.pdf` |
| 9c611a731c4b9df2de80e10ad4d37e4d | MPF00462972_Proveido_simple_1592501531.pdf | `2020/06/18/proveido_evaluacion_psiquiatrica_denunciante.pdf` |
| 8567ee185030e3160d0a3eafbb9fcee6 | MPF00462972_Proveido_simple_1592938095 (1).pdf | `2020/06/23/proveido_informa_ubicacion_del_cuerpo.pdf` |
| 125516e198c588a0679e9fc8f8ee4c70 | MPF00462972_Proveido_simple_1593440156.pdf | `den00641871/2020/06/29/proveido_requiere_911.pdf` |
| 0bc9845842b3a57a3991f7e1c940d686 | MPF00462972_Proveido_simple_1594643667.pdf | `2020/07/13/proveido_tiene_por_querellante.pdf` |
| 9f3f5e1d4cc549ac6638a8b57b773a20 | MPF00462972__Art._279.-_L_2303._Recurso_de_Apelación_-_Interposición_-_Juicio_1593463974 (1).pdf | `2020/06/29/fiscalia_reposicion_con_apelacion_subsidio.pdf` |
| 459e91a05fd8e7fb55b4b5aef9ff082a | MPF462697 HOSP DEAGUDO PIÑEIRO.pdf | `den00641871/2020/07/02/policia_diligencia_judicial_217_20.pdf` |
| 6f0b3af0e8c0ad89ab510e7d7ebd5778 | NO-2020-13866937-GCABA-HGAPP (1).pdf | `2020/05/19/nota_hospital_seguimiento_cadaveres.pdf` |
| 36b6219f709ef88c361f0de300a9ad8f | Nota GAP-375825.pdf | `den00641871/2020/06/29/respuesta_911_registros_llamados.pdf` |
| 9e55d59485650c6f12b19d2dade6e319 | Re_ Denuncia MPF 462972 1 (1).pdf | `2020/06/07/correo_sosa_reenvia_a_fiscalia_20.pdf` |
| e08d1222b853f93f6f7043148b008fba | Re_ SE CONSTITUYE EN QUERELLANTE CAUSA MPF 462972 (1).pdf | `2020/06/12/correo_fiscalia_notifica_proveido.pdf` |
| c3ebedefbdfe855e4f97226b5acb3523 | Reenv_ informe CIJ Entrevista Kosciuk.pdf | `2020/07/03/correo_escrich_reenvia_informe_auxiliar.pdf` |
| 585cf44fbb999dc668c2002bec0da3b7 | SE CONSTITUYE EN QUERELLANTE CAUSA MPF 462972 (1).pdf | `2020/06/08/correo_harari_se_constituye_querellante.pdf` |
| 983a07b04fc81103155bfc19968de820 | SE CONSTITUYEN EN QUERELLANTE  DEF (1).docx | `2020/06/07/querella_constitucion_formato_word.docx` |
| 61b34317765eca518b331b1418e3b3c0 | SUCESO N° 30489464.pdf | `den00641871/2020/03/25/informe_suceso_30489464.pdf` |
| 352e070d3a3db65026726ff469dff174 | SUCESO N° 30493529 - 30493637.pdf | `den00641871/2020/03/25/informe_suceso_30493529_30493637.pdf` |
| d2f6d84f32e5096d73728de34b2df695 | SUCESO N° 30493810.pdf | `den00641871/2020/03/25/informe_suceso_30493810.pdf` |
| 328f6d41655fb24450f9567ea503d642 | S_ Oficio Judicial.- KUCHASKY MARGARITA LEONOR - Caso MPF Nº 462972 e Intervención CIJ Nº 615445__ (3).pdf | `2020/06/10/correo_cementerios_responde_oficio.pdf` |
| a6712038eca8ff9632fd16429bb6e674 | TRANSCRPCION.pdf | `den00641871/2020/06/29/transcripcion_llamadas_911.pdf` |
| 36744ad11ec4f4562f077cc24698b672 | acta orden de presentación.jpg | `2020/05/18/acta_orden_presentacion_hospital.jpg` |
| a161def928a961d31fecfad7b00f543a | boletin oficial kuchasky 18-5-20.pdf | excluido |
| 8517e3e350e7a5f4422ca8969f55b1ff | boletin oficial kuchasky 19-5-20.pdf | excluido |
| c08f5bb9f9b3b26ceebf059ebb1e3ec5 | boletin oficial kuchasky.pdf | excluido |
| b6f684b8e4671735c5e41d90ecfc475b | cedula (16) (1).pdf | `2020/06/24/cedula_juzgado_26_competencia_pami.pdf` |
| cb2776a1086129d6a22264c0aed2feae | correo kosciuk 31 7 20.pdf | `2020/07/31/correo_denunciante_responde_a_branca.pdf` |
| f9c7d061fc53d429915832eefe451e85 | correo kosciuk.pdf | `2020/07/31/correo_denunciante_consulta_falso_testimonio.pdf` |
| 1337412e7b094f7b4c3bca9052e171e3 | correo y respuesta denunciante kosciuk.pdf | `2020/07/31/correo_branca_responde_sobre_entrevista.pdf` |
| e60897d4728895e59540cd2e82c6e8ff | descarga (1).pdf | `2020/06/22/juzgado_21_providencia_sobre_querella_1.pdf` |
| 65cb6c369dfbeb3c90d05619242b64d5 | descarga.pdf | `2020/06/24/juzgado_21_providencia_sobre_querella_2.pdf` |
| b6be16a49bda8c3314664ddca17d7bef | historia clinica parte 1 (1).pdf | `historia_clinica/historia_clinica_1.pdf` |
| 5301fc0c9246297a7d77eeb9079d0ab4 | historia clinica parte 2 (1).pdf | `historia_clinica/historia_clinica_2.pdf` |
| 80f703f39dc8f455d53a98d011718dbd | historia clinica parte 3 (1).pdf | `historia_clinica/historia_clinica_3.pdf` |
| 79e229444b46c3cf10e03aa8b02a1084 | historia clinica parte 4 (1).pdf | `historia_clinica/historia_clinica_4.pdf` |
| 63a302f8be67356e7f4079617298f7c1 | historia clinica parte 5 (1).pdf | `historia_clinica/historia_clinica_5.pdf` |
| 0a6638f3b4639d9b17d1503b2cc0362a | historia clinica parte 6 (1).pdf | `historia_clinica/historia_clinica_6.pdf` |
| 84c274c1a97bc471f59f922e7396d703 | historia clinica parte 7 (1).pdf | `historia_clinica/historia_clinica_7.pdf` |
| e8ee0bbdfb0eb82fe1c91e4c6a2501f6 | informe (1) (1).pdf | `2020/06/10/informe_cij_tareas_investigacion.pdf` |
| a61061f8a197072097f61d18e6b1c2ad | informe (2).pdf | `2020/06/03/informe_cij_orden_presentacion_hospital.pdf` |
| 5f15267098c6580c2f85d3ac4ee94fb7 | insert_notificacion18791589411838.pdf | `2020/05/13/cedula_juzgado_21_resolucion_allanamiento.pdf` |
| 65cb6c369dfbeb3c90d05619242b64d5 | juzgado piñero querella.pdf | `2020/06/24/juzgado_21_providencia_sobre_querella_2.pdf` |
| b8d78aad27b0545b2d56afcedbc10fc1 | kosciuk correo consulta UBA.pdf | `2020/06/22/correo_branca_responde_consulta_denuncia.pdf` |
| 1efda4850ca9209be67e3838daf859ee | mail harari pide copias.pdf | `2020/07/27/correo_harari_solicita_copia_expediente.pdf` |
| 55e9d887f186223165350d707c075f7b | mail harari solicita nuevo enlace de descarga y respuesta dada.pdf | `2020/07/30/correo_branca_responde_enlace_descarga.pdf` |
| db2c02cf4f14688041d7a822c13d0c88 | mail harari.pdf | `2020/07/15/correo_branca_responde_a_harari.pdf` |
| f504d56b10c60f6d06642ad0c932d91b | mail kosciuk a perito del cij diletto.pdf | `2020/08/01/correo_rozas_reenvia_mail_de_diletto.pdf` |
| 00377aa337266b50442b3a2be9b641a3 | orden de presentación1.jpg | `2020/05/15/orden_presentacion_hospital_1.jpg` |
| 3db8cb122396c5083530992cc31f0e45 | orden de presentación2.jpg | `2020/05/15/orden_presentacion_hospital_2.jpg` |
| 469db3b75d82504e56892e624391fab3 | querella piñero 2.pdf | `2020/06/22/correo_harari_adjunta_partida_nacimiento.pdf` |
| 08b19b59832611cf3e56db11d3de9543 | querella piñero.pdf | `2020/06/22/correo_harari_querella_formato_word.pdf` |
| 65cb6c369dfbeb3c90d05619242b64d5 | rechaza intervención juzgado kosciuk.pdf | `2020/06/24/juzgado_21_providencia_sobre_querella_2.pdf` |
| af04ed970080e193dd7472c3e9b0bf06 | resolucion querella hosp piñero.pdf | `2020/06/29/juzgado_21_resolucion_sobre_querella.pdf` |
| 39548cb259d225b2ddb22a81da2fcf1c | respuesta desempeño policia HOSPITAL PIÑERO.pdf | `2020/07/02/correo_policia_envia_diligencia_judicial.pdf` |
