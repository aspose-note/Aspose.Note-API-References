---
title: Enum SaveFormat
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.SaveFormat αρίθμηση. Υποδεικνύει τη μορφή στην οποία είναι αποθηκευμένο το έγγραφο.
type: docs
weight: 540
url: /el/net/aspose.note/saveformat/
---
## SaveFormat enumeration

Υποδεικνύει τη μορφή στην οποία είναι αποθηκευμένο το έγγραφο.

```csharp
public enum SaveFormat
```

### Αξίες

| Ονομα | αξία | Περιγραφή |
| --- | --- | --- |
| Png | `1` | Καθορίζει ότι η έξοδος είναι αρχείο PNG. |
| Bmp | `2` | Καθορίζει ότι η έξοδος είναι αρχείο BMP. |
| Jpeg | `3` | Καθορίζει ότι η έξοδος είναι αρχείο JPEG. |
| Gif | `4` | Καθορίζει ότι η έξοδος είναι ένα αρχείο GIF. |
| Tiff | `5` | Καθορίζει ότι η έξοδος είναι ένα αρχείο TIFF. |
| Pdf | `6` | Καθορίζει ότι η έξοδος είναι αρχείο PDF. |
| One | `7` | Καθορίζει ότι η έξοδος είναι ένα αρχείο OneNote. |
| Html | `8` | Καθορίζει ότι η έξοδος είναι ένα αρχείο HTML. |

### Παραδείγματα

Δείχνει πώς να αποθηκεύσετε ένα έγγραφο χρησιμοποιώντας την απαρίθμηση SaveFormat.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingSaveFormat_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, SaveFormat.One);
```

Δείχνει πώς να αποθηκεύσετε ένα έγγραφο σε μορφή pdf χρησιμοποιώντας τις προεπιλεγμένες ρυθμίσεις.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Αποθηκεύστε το έγγραφο ως PDF
dataDir = dataDir + "SaveWithDefaultSettings_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

Δείχνει πώς να αποθηκεύσετε ένα έγγραφο ως εικόνα σε μορφή Jpeg χρησιμοποιώντας το SaveFormat.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToJpegImageUsingSaveFormat_out.jpg";

// Αποθηκεύστε το έγγραφο.
oneFile.Save(dataDir, SaveFormat.Jpeg);
```

Δείχνει πώς να αποθηκεύσετε ένα έγγραφο σε μορφή gif.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToImageDefaultOptions_out.gif";

// Αποθηκεύστε το έγγραφο ως gif.
oneFile.Save(dataDir, SaveFormat.Gif);
```

Δείχνει πώς να ορίσετε μια ποιότητα εικόνας κατά την αποθήκευση εγγράφου ως εικόνα σε μορφή JPEG.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// Αποθηκεύστε το έγγραφο.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Quality = 100 });
```

Δείχνει πώς να αποθηκεύσετε ένα έγγραφο ως εικόνα σε μορφή Bmp χρησιμοποιώντας το ImageSaveOptions.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBmpImageUsingImageSaveOptions_out.bmp";

// Αποθηκεύστε το έγγραφο.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Bmp));
```

Δείχνει πώς να ορίσετε μια ανάλυση εικόνας κατά την αποθήκευση εγγράφου ως εικόνα.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SetOutputImageResolution_out.jpg";

// Αποθηκεύστε το έγγραφο.
doc.Save(dataDir, new ImageSaveOptions(SaveFormat.Jpeg) { Resolution = 220 });
```

Δείχνει πώς να αποθηκεύσετε ένα έγγραφο ως εικόνα σε κλίμακα του γκρι.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveAsGrayscaleImage_out.png";

// Αποθηκεύστε το έγγραφο ως gif.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                          {
                              ColorMode = ColorMode.GrayScale
                          });
```

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

Δείχνει πώς να αποθηκεύσετε ένα έγγραφο ως δυαδική εικόνα χρησιμοποιώντας τη μέθοδο του Otsu.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBinaryImageUsingOtsuMethod_out.png";

// Αποθηκεύστε το έγγραφο ως gif.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                        {
                            ColorMode = ColorMode.BlackAndWhite,
                            BinarizationOptions = new ImageBinarizationOptions()
                                                  {
                                                      BinarizationMethod = BinarizationMethod.Otsu,
                                                  }
                        });
```

Δείχνει πώς να αποθηκεύσετε ένα έγγραφο ως δυαδική εικόνα χρησιμοποιώντας σταθερό όριο.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBinaryImageUsingFixedThreshold_out.png";

// Αποθηκεύστε το έγγραφο ως gif.
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                          {
                              ColorMode = ColorMode.BlackAndWhite,
                              BinarizationOptions = new ImageBinarizationOptions()
                                                        {
                                                            BinarizationMethod = BinarizationMethod.FixedThreshold,
                                                            BinarizationThreshold = 123
                                                        }
                          });
```

### Δείτε επίσης

* χώρος ονομάτων [Aspose.Note](../../aspose.note/)
* συνέλευση [Aspose.Note](../../)


