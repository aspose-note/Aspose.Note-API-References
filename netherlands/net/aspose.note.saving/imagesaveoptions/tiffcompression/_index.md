---
title: ImageSaveOptions.TiffCompression
second_title: Aspose.Note voor .NET API-referentie
description: ImageSaveOptions eigendom. Hiermee wordt het type compressie opgehaald of ingesteld dat moet worden gebruikt bij het opslaan van gegenereerde afbeeldingen in het TIFFformaat.
type: docs
weight: 60
url: /nl/net/aspose.note.saving/imagesaveoptions/tiffcompression/
---
## ImageSaveOptions.TiffCompression property

Hiermee wordt het type compressie opgehaald of ingesteld dat moet worden gebruikt bij het opslaan van gegenereerde afbeeldingen in het TIFF-formaat.

```csharp
public TiffCompression TiffCompression { get; set; }
```

### Voorbeelden

Laat zien hoe u een document opslaat als afbeelding in Tiff-indeling met behulp van PackBits-compressie.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laad het document in Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingPackBitsCompression.tiff");

// Sla het document op.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          TiffCompression = TiffCompression.PackBits
                      });
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

Laat zien hoe u een document kunt opslaan als afbeelding in Tiff-indeling met behulp van CCITT Groep 3-faxcompressie.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laad het document in Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingCcitt3Compression.tiff");

// Sla het document op.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          ColorMode = ColorMode.BlackAndWhite,
                          TiffCompression = TiffCompression.Ccitt3
                      });
```

### Zie ook

* enum [TiffCompression](../../tiffcompression/)
* class [ImageSaveOptions](../)
* naamruimte [Aspose.Note.Saving](../../imagesaveoptions/)
* montage [Aspose.Note](../../../)


