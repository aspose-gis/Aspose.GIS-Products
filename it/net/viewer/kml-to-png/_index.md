---
title: Converti KML in PNG
url: /it/net/viewer/kml-to-png/
linkTitle: Converti KML in PNG
weight: 10
---

## Convertitore da KML a PNG .NET

Questo esempio mostra come convertire un file KML in un'immagine PNG utilizzando la libreria NetViewer.

### Prerequisiti

*   Visual Studio
*   .NET Framework 4.7.2 o versione successiva
*   NetViewer NuGet package

### Passaggi

1.  Crea un nuovo progetto applicazione console .NET.
2.  Installa il pacchetto NuGet NetViewer.
3.  Aggiungi le seguenti istruzioni `using`:

```csharp
using NetViewer;
using System.Drawing;
using System.Drawing.Imaging;
```

4.  Utilizza la seguente funzione per convertire un file KML in un'immagine PNG:

```csharp
public static void ConvertKmlToPng(string kmlFilePath, string pngFilePath)
{
    // Crea un oggetto KmlViewer.
    var viewer = new KmlViewer();

    // Carica il file KML.
    viewer.LoadKml(kmlFilePath);

    // Rendi l'immagine.
    Bitmap bitmap = viewer.Render(1024, 768);

    // Salva l'immagine come PNG.
    bitmap.Save(pngFilePath, ImageFormat.Png);

    // Libera le risorse.
    bitmap.Dispose();
}
```

### Esempio di utilizzo

```csharp
string kmlFilePath = "path/to/your/file.kml";
string pngFilePath = "path/to/your/output.png";

ConvertKmlToPng(kmlFilePath, pngFilePath);
```

Questo codice convertirà il file KML specificato nel percorso `kmlFilePath` in un'immagine PNG e la salverà nel percorso `pngFilePath`. La dimensione dell'immagine renderizzata è di 1024x768 pixel.

### Note

*   Assicurati che il file KML sia valido.
*   La libreria NetViewer richiede una connessione Internet per scaricare le risorse necessarie.
*   Puoi personalizzare la dimensione dell'immagine renderizzata modificando i parametri nella funzione `Render()`.
*   Se riscontri problemi, consulta la documentazione della libreria NetViewer o contatta il supporto tecnico.

