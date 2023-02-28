---
title: Class ImageSaveOptions
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.Saving.ImageSaveOptions τάξη. Επιτρέπει τον καθορισμό πρόσθετων επιλογών κατά την απόδοση σελίδων εγγράφου σε εικόνες.
type: docs
weight: 720
url: /el/net/aspose.note.saving/imagesaveoptions/
---
## ImageSaveOptions class

Επιτρέπει τον καθορισμό πρόσθετων επιλογών κατά την απόδοση σελίδων εγγράφου σε εικόνες.

```csharp
public class ImageSaveOptions : SaveOptions
```

## Κατασκευαστές

| Ονομα | Περιγραφή |
| --- | --- |
| [ImageSaveOptions](imagesaveoptions/)(SaveFormat) | Αρχικοποιεί μια νέα παρουσία του`ImageSaveOptions` τάξη. |

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| [BinarizationOptions](../../aspose.note.saving/imagesaveoptions/binarizationoptions/) { get; set; } | Λαμβάνει ή ορίζει επιλογές για τη δυαδοποίηση της εικόνας. |
| [ColorMode](../../aspose.note.saving/imagesaveoptions/colormode/) { get; set; } | Παίρνει ή θέτει[`ColorMode`](./colormode/) για την εικόνα εξόδου. |
| [FontsSubsystem](../../aspose.note.saving/saveoptions/fontssubsystem/) { get; set; } | Λαμβάνει ή ορίζει τις ρυθμίσεις της γραμματοσειράς που θα χρησιμοποιηθούν κατά την αποθήκευση |
| [PageCount](../../aspose.note.saving/saveoptions/pagecount/) { get; set; } | Λαμβάνει ή ορίζει τον αριθμό των σελίδων προς αποθήκευση. Από προεπιλογή είναιMaxValue που σημαίνει ότι όλες οι σελίδες του εγγράφου θα αποδοθούν. |
| [PageIndex](../../aspose.note.saving/saveoptions/pageindex/) { get; set; } | Λαμβάνει ή ορίζει το ευρετήριο της πρώτης σελίδας προς αποθήκευση. Από προεπιλογή είναι 0. |
| [Quality](../../aspose.note.saving/imagesaveoptions/quality/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που καθορίζει την ποιότητα της αποθηκευμένης εικόνας. Αυτή η τιμή μεταβιβάζεται στον κωδικοποιητή ως παράμετρος System.Drawing.Imaging.Encoder.Quality. |
| [Resolution](../../aspose.note.saving/imagesaveoptions/resolution/) { get; set; } | Λαμβάνει ή ορίζει την ανάλυση για τις εικόνες που δημιουργούνται, σε κουκκίδες ανά ίντσα. |
| [SaveFormat](../../aspose.note.saving/saveoptions/saveformat/) { get; } | Λαμβάνει τη μορφή στην οποία είναι αποθηκευμένο το έγγραφο. |
| [TiffCompression](../../aspose.note.saving/imagesaveoptions/tiffcompression/) { get; set; } | Λαμβάνει ή ορίζει τον τύπο συμπίεσης που θα χρησιμοποιηθεί κατά την αποθήκευση των δημιουργούμενων εικόνων στη μορφή TIFF. |

### Παραδείγματα

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

Δείχνει πώς να αποθηκεύσετε το σημειωματάριο ως εικόνα με καθορισμένες επιλογές.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Φόρτωση σημειωματάριου OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;

dataDir = dataDir + "ConvertToImageWithOptions_out.png";

// Αποθηκεύστε το Σημειωματάριο
notebook.Save(dataDir, notebookSaveOptions);
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

Δείχνει πώς να αποθηκεύσετε το πεπλατυσμένο σημειωματάριο ως εικόνα.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Φόρτωση σημειωματάριου OneNote
var notebook = new Notebook(dataDir + "Notizbuch öffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;
notebookSaveOptions.Flatten = true;

dataDir = dataDir + "ConvertToImageAsFlattenedNotebook_out.png";

// Αποθηκεύστε το Σημειωματάριο
notebook.Save(dataDir, notebookSaveOptions);
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

Δείχνει πώς να αποθηκεύσετε ένα έγγραφο σε μορφή png.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Εκκίνηση αντικειμένου ImageSaveOptions 
ImageSaveOptions opts = new ImageSaveOptions(SaveFormat.Png)
                            {
                                // Ορισμός ευρετηρίου σελίδας
                                PageIndex = 1
                            };

dataDir = dataDir + "ConvertSpecificPageToImage_out.png";

// Αποθηκεύστε το έγγραφο ως PNG.
oneFile.Save(dataDir, opts);
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

* class [SaveOptions](../saveoptions/)
* χώρος ονομάτων [Aspose.Note.Saving](../../aspose.note.saving/)
* συνέλευση [Aspose.Note](../../)


