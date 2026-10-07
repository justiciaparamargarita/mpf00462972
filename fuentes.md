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
  - Fiscalía PCyF Nro. 20 - Notifica resolución s_ caso _Hospital Piñero_.pdf
  - mail harari.pdf
  - mail harari pide copias.pdf
  - mail harari solicita nuevo enlace de descarga y respuesta dada.pdf
  - mail kosciuk a perito del cij diletto.pdf
- Dentro de cada zip hay archivos repetidos con distinto nombre (94 contenidos distintos en 100 archivos del zip de wetransfer; 108 en los 114 de Filemail).

## Historia clínica

Los 7 PDF `historia clinica parte 1..7 (1).pdf` (284, 32, 58, 36, 2, 1 y 12 páginas; 425 en total) no figuran como archivos propios en el repo. Están unidos, en ese orden y página por página, en `historia_clinica/historia_clinica.pdf` (425 páginas, verificado por render). Las 252 páginas útiles están en `historia_clinica/paginas/` y `transcripciones/`; las demás se detallan en `historia_clinica/eliminadas.md`.

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
