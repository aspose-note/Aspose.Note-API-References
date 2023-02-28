---
title: ImageSaveOptions.Quality
second_title: Aspose.Note voor .NET API-referentie
description: ImageSaveOptions eigendom. Hiermee wordt een waarde opgehaald of ingesteld die de kwaliteit van de opgeslagen afbeelding bepaalt. Deze waarde wordt doorgegeven aan de codec als System.Drawing.Imaging.Encoder.Qualityparameter.
type: docs
weight: 40
url: /nl/net/aspose.note.saving/imagesaveoptions/quality/
---
## ImageSaveOptions.Quality property

Hiermee wordt een waarde opgehaald of ingesteld die de kwaliteit van de opgeslagen afbeelding bepaalt. Deze waarde wordt doorgegeven aan de codec als System.Drawing.Imaging.Encoder.Quality-parameter.

```csharp
public int Quality { get; set; }
```

### Opmerkingen

Het bereik van bruikbare waarden voor de kwaliteitscategorie is van 0 tot 100. Hoe lager het opgegeven getal, hoe hoger de compressie en dus hoe lager de kwaliteit van de afbeelding. Nul geeft u de afbeelding met de laagste kwaliteit en 100 de hoogste . De standaardwaarde is 90.

### Voorbeelden

Laat zien hoe u een afbeeldingskwaliteit instelt wanneer u een document opslaat als afbeelding in JPEG-indeling.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laad het document in Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// Sla het document op.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Quality = 100 });
```

Laat zien hoe u een document kunt opslaan als afbeelding in Tiff-indeling met behulp van JPEG-compressie.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laad het document in Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingJpegCompression.tiff");

// Sla het document op.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          TiffCompression = TiffCompression.Jpeg,
                          Quality = 93
                      });
```

### Zie ook

* class [ImageSaveOptions](../)
* naamruimte [Aspose.Note.Saving](../../imagesaveoptions/)
* montage [Aspose.Note](../../../)


