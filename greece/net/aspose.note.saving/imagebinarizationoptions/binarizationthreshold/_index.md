---
title: ImageBinarizationOptions.BinarizationThreshold
second_title: Aspose.Note for .NET API Reference
description: ImageBinarizationOptions ιδιοκτησία. Λαμβάνει ή ορίζει την τιμή κατωφλίου για τη μέθοδο δυαδοποίησης σταθερού ορίου. Η προεπιλεγμένη τιμή είναι 128.
type: docs
weight: 30
url: /el/net/aspose.note.saving/imagebinarizationoptions/binarizationthreshold/
---
## ImageBinarizationOptions.BinarizationThreshold property

Λαμβάνει ή ορίζει την τιμή κατωφλίου για τη μέθοδο δυαδοποίησης σταθερού ορίου. Η προεπιλεγμένη τιμή είναι 128.

```csharp
public byte BinarizationThreshold { get; set; }
```

### Παραδείγματα

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

* class [ImageBinarizationOptions](../)
* χώρος ονομάτων [Aspose.Note.Saving](../../imagebinarizationoptions/)
* συνέλευση [Aspose.Note](../../../)


