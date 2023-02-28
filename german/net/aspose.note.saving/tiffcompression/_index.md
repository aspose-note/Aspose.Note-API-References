---
title: Enum TiffCompression
second_title: Aspose.Note für .NET-API-Referenz
description: Aspose.Note.Saving.TiffCompression opsomming. Gibt an welcher Komprimierungstyp verwendet werden soll wenn ein Dokument im TIFFFormat gespeichert wird.
type: docs
weight: 880
url: /de/net/aspose.note.saving/tiffcompression/
---
## TiffCompression enumeration

Gibt an, welcher Komprimierungstyp verwendet werden soll, wenn ein Dokument im TIFF-Format gespeichert wird.

```csharp
public enum TiffCompression
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| None | `1` | Gibt keine Komprimierung an. |
| Rle | `2` | Gibt die RLE-Komprimierung an. |
| Ccitt3 | `3` | Gibt die CCITT-Faxcodierung der Gruppe 3 an. |
| Ccitt4 | `4` | Gibt die CCITT-Faxcodierung der Gruppe 4 an. |
| Lzw | `5` | Gibt die LZW-Komprimierung an. |
| PackBits | `32773` | Gibt die Macintosh-RLE-Komprimierung an. |
| Jpeg | `7` | Gibt die JPEG-DCT-Komprimierung an. |

### Beispiele

Zeigt, wie ein Dokument als Bild im Tiff-Format mit PackBits-Komprimierung gespeichert wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laden Sie das Dokument in Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingPackBitsCompression.tiff");

// Speichern Sie das Dokument.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          TiffCompression = TiffCompression.PackBits
                      });
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

Zeigt, wie ein Dokument als Bild im Tiff-Format mit CCITT Group 3-Faxkomprimierung gespeichert wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laden Sie das Dokument in Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingCcitt3Compression.tiff");

// Speichern Sie das Dokument.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          ColorMode = ColorMode.BlackAndWhite,
                          TiffCompression = TiffCompression.Ccitt3
                      });
```

### Siehe auch

* namensraum [Aspose.Note.Saving](../../aspose.note.saving/)
* Montage [Aspose.Note](../../)


