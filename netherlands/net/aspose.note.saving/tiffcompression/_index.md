---
title: Enum TiffCompression
second_title: Aspose.Note voor .NET API-referentie
description: Aspose.Note.Saving.TiffCompression opsomming. Geeft aan welk type compressie moet worden gebruikt bij het opslaan van een document in de TIFFindeling.
type: docs
weight: 880
url: /nl/net/aspose.note.saving/tiffcompression/
---
## TiffCompression enumeration

Geeft aan welk type compressie moet worden gebruikt bij het opslaan van een document in de TIFF-indeling.

```csharp
public enum TiffCompression
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| None | `1` | Specificeert geen compressie. |
| Rle | `2` | Specificeert RLE-compressie. |
| Ccitt3 | `3` | Specificeert CCITT Groep 3 faxcodering. |
| Ccitt4 | `4` | Specificeert CCITT Groep 4 faxcodering. |
| Lzw | `5` | Specificeert LZW-compressie. |
| PackBits | `32773` | Specificeert Macintosh RLE-compressie. |
| Jpeg | `7` | Specificeert JPEG DCT-compressiecompressie. |

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

* naamruimte [Aspose.Note.Saving](../../aspose.note.saving/)
* montage [Aspose.Note](../../)


