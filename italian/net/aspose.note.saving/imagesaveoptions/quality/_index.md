---
title: ImageSaveOptions.Quality
second_title: Aspose.Note per .NET API Reference
description: ImageSaveOptions proprietà. Ottiene o imposta un valore che determina la qualità dellimmagine salvata. Questo valore viene passato al codec come parametro System.Drawing.Imaging.Encoder.Quality.
type: docs
weight: 40
url: /it/net/aspose.note.saving/imagesaveoptions/quality/
---
## ImageSaveOptions.Quality property

Ottiene o imposta un valore che determina la qualità dell'immagine salvata. Questo valore viene passato al codec come parametro System.Drawing.Imaging.Encoder.Quality.

```csharp
public int Quality { get; set; }
```

### Osservazioni

L'intervallo di valori utili per la categoria di qualità va da 0 a 100. Più basso è il numero specificato, maggiore è la compressione e quindi minore è la qualità dell'immagine. Zero darebbe la qualità dell'immagine più bassa e 100 la più alta . Il valore predefinito è 90.

### Esempi

Mostra come impostare una qualità dell'immagine quando si salva un documento come immagine in formato JPEG.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Carica il documento in Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// Salva il documento.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Quality = 100 });
```

Mostra come salvare un documento come immagine in formato Tiff utilizzando la compressione Jpeg.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Carica il documento in Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingJpegCompression.tiff");

// Salva il documento.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          TiffCompression = TiffCompression.Jpeg,
                          Quality = 93
                      });
```

### Guarda anche

* class [ImageSaveOptions](../)
* spazio dei nomi [Aspose.Note.Saving](../../imagesaveoptions/)
* assemblea [Aspose.Note](../../../)


