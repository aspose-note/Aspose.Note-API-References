---
title: ImageSaveOptions.Quality
second_title: Aspose.Note for .NET API Reference
description: ImageSaveOptions ιδιοκτησία. Λαμβάνει ή ορίζει μια τιμή που καθορίζει την ποιότητα της αποθηκευμένης εικόνας. Αυτή η τιμή μεταβιβάζεται στον κωδικοποιητή ως παράμετρος System.Drawing.Imaging.Encoder.Quality.
type: docs
weight: 40
url: /el/net/aspose.note.saving/imagesaveoptions/quality/
---
## ImageSaveOptions.Quality property

Λαμβάνει ή ορίζει μια τιμή που καθορίζει την ποιότητα της αποθηκευμένης εικόνας. Αυτή η τιμή μεταβιβάζεται στον κωδικοποιητή ως παράμετρος System.Drawing.Imaging.Encoder.Quality.

```csharp
public int Quality { get; set; }
```

### Παρατηρήσεις

Το εύρος των χρήσιμων τιμών για την κατηγορία ποιότητας είναι από 0 έως 100. Όσο μικρότερος είναι ο καθορισμένος αριθμός, τόσο μεγαλύτερη είναι η συμπίεση και επομένως χαμηλότερη η ποιότητα της εικόνας. Το μηδέν θα σας έδινε τη χαμηλότερη ποιότητα εικόνας και το 100 την υψηλότερη . Η προεπιλεγμένη τιμή είναι 90.

### Παραδείγματα

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

### Δείτε επίσης

* class [ImageSaveOptions](../)
* χώρος ονομάτων [Aspose.Note.Saving](../../imagesaveoptions/)
* συνέλευση [Aspose.Note](../../../)


