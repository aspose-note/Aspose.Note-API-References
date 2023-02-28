---
title: Class ImageBinarizationOptions
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.Saving.ImageBinarizationOptions τάξη. Επιλογές για δυαδοποίηση εικόνας.
type: docs
weight: 710
url: /el/net/aspose.note.saving/imagebinarizationoptions/
---
## ImageBinarizationOptions class

Επιλογές για δυαδοποίηση εικόνας.

```csharp
public class ImageBinarizationOptions
```

## Κατασκευαστές

| Ονομα | Περιγραφή |
| --- | --- |
| [ImageBinarizationOptions](imagebinarizationoptions/)() | Ο προεπιλεγμένος κατασκευαστής. |

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| [BinarizationMethod](../../aspose.note.saving/imagebinarizationoptions/binarizationmethod/) { get; set; } | Λαμβάνει ή ορίζει τη μέθοδο δυαδοποίησης. Η προεπιλεγμένη τιμή είναιFixedThreshold . |
| [BinarizationThreshold](../../aspose.note.saving/imagebinarizationoptions/binarizationthreshold/) { get; set; } | Λαμβάνει ή ορίζει την τιμή κατωφλίου για τη μέθοδο δυαδοποίησης σταθερού ορίου. Η προεπιλεγμένη τιμή είναι 128. |

### Παραδείγματα

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


