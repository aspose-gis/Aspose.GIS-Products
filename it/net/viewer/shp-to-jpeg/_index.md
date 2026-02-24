---
title: Conversione SHP in JPEG
url: /it/viewer/shp-to-jpeg/
weight: 10
layout: single
start: true
toc: true
draft: false
description: Converti file shapefile (.shp) in immagini JPEG.
---

## Conversione SHP in JPEG

Questo strumento permette di convertire file shapefile (.shp) in immagini JPEG.  È possibile specificare l'area geografica da visualizzare, la risoluzione dell'immagine e altri parametri per ottenere il risultato desiderato.

### Requisiti

*   .NET Framework 4.7.2 o superiore
*   GDAL (Geospatial Data Abstraction Library)

### Installazione

1.  Scarica l'eseguibile SHPtoJPEG.exe.
2.  Assicurati di avere GDAL installato e configurato correttamente nel tuo sistema.  Se non hai GDAL, puoi scaricarlo da [https://gdal.org/](https://gdal.org/).
3.  Posiziona l'eseguibile SHPtoJPEG.exe in una cartella a tua scelta.

### Utilizzo

Per eseguire la conversione, apri il prompt dei comandi o il terminale e naviga nella cartella dove hai salvato SHPtoJPEG.exe.  Utilizza il seguente comando:

```
SHPtoJPEG.exe -i <file_shp> -o <file_jpeg> -r <risoluzione> -b <bbox> -p
```

Dove:

*   `-i`: Percorso del file shapefile di input (.shp).
*   `-o`: Percorso del file JPEG di output.
*   `-r`: Risoluzione dell'immagine in DPI (dots per inch).  Valore predefinito: 300.
*   `-b`: Bounding box da visualizzare nel formato `xmin,ymin,xmax,ymax`. Se omesso, viene utilizzato l'intero shapefile.
*   `-p`:  Utilizza la proiezione del file shapefile.

### Esempi

*   Per convertire il file "mappa.shp" in un'immagine JPEG chiamata "mappa.jpeg" con risoluzione 300 DPI:

```
SHPtoJPEG.exe -i mappa.shp -o mappa.jpeg -r 300
```

*   Per convertire il file "mappa.shp" in un'immagine JPEG chiamata "mappa_cropped.jpeg" con risoluzione 150 DPI e bounding box da 10 a 20:

```
SHPtoJPEG.exe -i mappa.shp -o mappa_cropped.jpeg -r 150 -b 10,10,20,20
```

*   Per convertire il file "mappa.shp" in un'immagine JPEG chiamata "mappa_projected.jpeg" utilizzando la proiezione del file shapefile:

```
SHPtoJPEG.exe -i mappa.shp -o mappa_projected.jpeg -p
```

### Parametri Aggiuntivi

| Parametro | Descrizione                                  | Valore Predefinito |
| --------- | -------------------------------------------- | ------------------ |
| `-l`      | Livello di dettaglio (compressione JPEG).     | 7                  |
| `-t`      | Formato del file di output (jpeg o png).    | jpeg               |

### Note

*   Assicurati che GDAL sia correttamente installato e configurato.  In caso contrario, lo strumento non funzionerà.
*   La risoluzione dell'immagine influisce sulla dimensione del file JPEG di output.  Valori più alti producono immagini di qualità superiore ma anche file più grandi.
*   Il bounding box definisce l'area geografica da visualizzare nell'immagine JPEG.  Assicurati che il bounding box sia valido e contenga i dati desiderati.
---
