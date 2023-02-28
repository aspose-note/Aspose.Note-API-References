---
title: Enum TiffCompression
second_title: Aspose.Note för .NET API-referens
description: Aspose.Note.Saving.TiffCompression uppräkning. Anger vilken typ av komprimering som ska användas när ett dokument sparas i TIFFformat.
type: docs
weight: 880
url: /sv/net/aspose.note.saving/tiffcompression/
---
## TiffCompression enumeration

Anger vilken typ av komprimering som ska användas när ett dokument sparas i TIFF-format.

```csharp
public enum TiffCompression
```

### Värderingar

| namn | Värde | Beskrivning |
| --- | --- | --- |
| None | `1` | Anger ingen komprimering. |
| Rle | `2` | Anger RLE-komprimering. |
| Ccitt3 | `3` | Anger CCITT Group 3-faxkodning. |
| Ccitt4 | `4` | Anger CCITT Group 4-faxkodning. |
| Lzw | `5` | Anger LZW-komprimering. |
| PackBits | `32773` | Anger Macintosh RLE-komprimering. |
| Jpeg | `7` | Anger JPEG DCT-komprimering. |

### Exempel

Visar hur man sparar ett dokument som bild i Tiff-format med PackBits-komprimering.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Ladda dokumentet i Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingPackBitsCompression.tiff");

// Spara dokumentet.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          TiffCompression = TiffCompression.PackBits
                      });
```

Visar hur man sparar ett dokument som bild i Tiff-format med Jpeg-komprimering.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Ladda dokumentet i Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingJpegCompression.tiff");

// Spara dokumentet.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          TiffCompression = TiffCompression.Jpeg,
                          Quality = 93
                      });
```

Visar hur man sparar ett dokument som bild i Tiff-format med hjälp av CCITT Group 3-faxkomprimering.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Ladda dokumentet i Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingCcitt3Compression.tiff");

// Spara dokumentet.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          ColorMode = ColorMode.BlackAndWhite,
                          TiffCompression = TiffCompression.Ccitt3
                      });
```

### Se även

* namnutrymme [Aspose.Note.Saving](../../aspose.note.saving/)
* hopsättning [Aspose.Note](../../)


