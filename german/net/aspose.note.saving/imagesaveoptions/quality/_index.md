---
title: ImageSaveOptions.Quality
second_title: Aspose.Note für .NET-API-Referenz
description: ImageSaveOptions eigendom. Ruft einen Wert ab oder legt einen Wert fest der die Qualität des gespeicherten Bildes bestimmt. Dieser Wert wird als System.Drawing.Imaging.Encoder.QualityParameter an den Codec übergeben.
type: docs
weight: 40
url: /de/net/aspose.note.saving/imagesaveoptions/quality/
---
## ImageSaveOptions.Quality property

Ruft einen Wert ab oder legt einen Wert fest, der die Qualität des gespeicherten Bildes bestimmt. Dieser Wert wird als System.Drawing.Imaging.Encoder.Quality-Parameter an den Codec übergeben.

```csharp
public int Quality { get; set; }
```

### Bemerkungen

Der Wertebereich für die Qualitätskategorie reicht von 0 bis 100. Je niedriger die angegebene Zahl, desto höher die Komprimierung und desto geringer die Bildqualität. Null würde Ihnen die niedrigste Bildqualität und 100 die höchste geben . Der Standardwert ist 90.

### Beispiele

Zeigt, wie eine Bildqualität eingestellt wird, wenn ein Dokument als Bild im JPEG-Format gespeichert wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laden Sie das Dokument in Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// Speichern Sie das Dokument.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Quality = 100 });
```

Zeigt, wie ein Dokument als Bild im Tiff-Format mit JPEG-Komprimierung gespeichert wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laden Sie das Dokument in Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingJpegCompression.tiff");

// Speichern Sie das Dokument.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          TiffCompression = TiffCompression.Jpeg,
                          Quality = 93
                      });
```

### Siehe auch

* class [ImageSaveOptions](../)
* namensraum [Aspose.Note.Saving](../../imagesaveoptions/)
* Montage [Aspose.Note](../../../)


