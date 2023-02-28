---
title: Enum BinarizationMethod
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.Saving.BinarizationMethod αρίθμηση. Καθορίζει τη μέθοδο δυαδοποίησης για μια εικόνα.
type: docs
weight: 560
url: /el/net/aspose.note.saving/binarizationmethod/
---
## BinarizationMethod enumeration

Καθορίζει τη μέθοδο δυαδοποίησης για μια εικόνα.

```csharp
public enum BinarizationMethod
```

### Αξίες

| Ονομα | αξία | Περιγραφή |
| --- | --- | --- |
| FixedThreshold | `0` | Η δυαδοποίηση της εικόνας πραγματοποιείται χρησιμοποιώντας καθορισμένο σταθερό όριο. |
| Otsu | `1` | Η δυαδοποίηση της εικόνας εκτελείται προσαρμοστικά χρησιμοποιώντας τη μέθοδο του Otsu για την αξιολόγηση του ορίου. |

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


