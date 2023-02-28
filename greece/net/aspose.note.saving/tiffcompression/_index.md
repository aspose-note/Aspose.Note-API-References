---
title: Enum TiffCompression
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.Saving.TiffCompression αρίθμηση. Καθορίζει τον τύπο συμπίεσης που θα χρησιμοποιείται κατά την αποθήκευση ενός εγγράφου σε μορφή TIFF.
type: docs
weight: 880
url: /el/net/aspose.note.saving/tiffcompression/
---
## TiffCompression enumeration

Καθορίζει τον τύπο συμπίεσης που θα χρησιμοποιείται κατά την αποθήκευση ενός εγγράφου σε μορφή TIFF.

```csharp
public enum TiffCompression
```

### Αξίες

| Ονομα | αξία | Περιγραφή |
| --- | --- | --- |
| None | `1` | Καθορίζει καμία συμπίεση. |
| Rle | `2` | Καθορίζει συμπίεση RLE. |
| Ccitt3 | `3` | Καθορίζει την κωδικοποίηση φαξ CCITT Group 3. |
| Ccitt4 | `4` | Καθορίζει την κωδικοποίηση φαξ της ομάδας 4 CCITT. |
| Lzw | `5` | Καθορίζει συμπίεση LZW. |
| PackBits | `32773` | Καθορίζει τη συμπίεση RLE Macintosh. |
| Jpeg | `7` | Καθορίζει συμπίεση συμπίεσης JPEG DCT. |

### Παραδείγματα

Δείχνει πώς να αποθηκεύσετε ένα έγγραφο ως εικόνα σε μορφή Tiff χρησιμοποιώντας συμπίεση PackBits.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingPackBitsCompression.tiff");

// Αποθηκεύστε το έγγραφο.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          TiffCompression = TiffCompression.PackBits
                      });
```

Δείχνει πώς να αποθηκεύσετε ένα έγγραφο ως εικόνα σε μορφή Tiff χρησιμοποιώντας συμπίεση Jpeg.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingJpegCompression.tiff");

// Αποθηκεύστε το έγγραφο.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          TiffCompression = TiffCompression.Jpeg,
                          Quality = 93
                      });
```

Δείχνει πώς να αποθηκεύσετε ένα έγγραφο ως εικόνα σε μορφή Tiff χρησιμοποιώντας συμπίεση φαξ CCITT Group 3.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingCcitt3Compression.tiff");

// Αποθηκεύστε το έγγραφο.
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          ColorMode = ColorMode.BlackAndWhite,
                          TiffCompression = TiffCompression.Ccitt3
                      });
```

### Δείτε επίσης

* χώρος ονομάτων [Aspose.Note.Saving](../../aspose.note.saving/)
* συνέλευση [Aspose.Note](../../)


