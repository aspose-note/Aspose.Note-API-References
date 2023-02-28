---
title: Enum ColorMode
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.Saving.ColorMode αρίθμηση. Η λειτουργία χρώματος της εικόνας.
type: docs
weight: 570
url: /el/net/aspose.note.saving/colormode/
---
## ColorMode enumeration

Η λειτουργία χρώματος της εικόνας.

```csharp
public enum ColorMode
```

### Αξίες

| Ονομα | αξία | Περιγραφή |
| --- | --- | --- |
| Normal | `0` | Πλήρης έγχρωμη εικόνα |
| GrayScale | `1` | Εικόνα σε κλίμακα του γκρι |
| BlackAndWhite | `2` | Δυαδική εικόνα: χρησιμοποιούνται μόνο ασπρόμαυρα χρώματα |

### Παραδείγματα

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

* χώρος ονομάτων [Aspose.Note.Saving](../../aspose.note.saving/)
* συνέλευση [Aspose.Note](../../)


