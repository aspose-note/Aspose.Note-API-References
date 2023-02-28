---
title: Document.Save
second_title: Aspose.Note for .NET API Reference
description: Document μέθοδος. Αποθηκεύει το έγγραφο του OneNote σε ένα αρχείο.
type: docs
weight: 140
url: /el/net/aspose.note/document/save/
---
## Save(string) {#save_3}

Αποθηκεύει το έγγραφο του OneNote σε ένα αρχείο.

```csharp
public void Save(string fileName)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fileName | String | Το πλήρες όνομα του αρχείου. Εάν υπάρχει ήδη ένα αρχείο με το καθορισμένο πλήρες όνομα, το υπάρχον αρχείο αντικαθίσταται. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | Η δομή του εγγράφου παραβιάζει τις προδιαγραφές. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | Η αιτούμενη μορφή αποθήκευσης δεν υποστηρίζεται. |

### Παραδείγματα

Δείχνει πώς να αποθηκεύσετε ένα έγγραφο.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormat_out.one";

Document doc = new Document(dataDir + inputFile);
doc.Save(dataDir + outputFile);
```

### Δείτε επίσης

* class [Document](../)
* χώρος ονομάτων [Aspose.Note](../../document/)
* συνέλευση [Aspose.Note](../../../)

---

## Save(Stream) {#save}

Αποθηκεύει το έγγραφο του OneNote σε μια ροή.

```csharp
public void Save(Stream stream)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| stream | Stream | Το System.IO.Ροή όπου θα αποθηκευτεί το έγγραφο. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | Η δομή του εγγράφου παραβιάζει τις προδιαγραφές. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | Η αιτούμενη μορφή αποθήκευσης δεν υποστηρίζεται. |

### Δείτε επίσης

* class [Document](../)
* χώρος ονομάτων [Aspose.Note](../../document/)
* συνέλευση [Aspose.Note](../../../)

---

## Save(string, SaveFormat) {#save_4}

Αποθηκεύει το έγγραφο του OneNote σε ένα αρχείο στην καθορισμένη μορφή.

```csharp
public void Save(string fileName, SaveFormat format)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fileName | String | Το πλήρες όνομα του αρχείου. Εάν υπάρχει ήδη ένα αρχείο με το καθορισμένο πλήρες όνομα, το υπάρχον αρχείο αντικαθίσταται. |
| format | SaveFormat | Η μορφή με την οποία αποθηκεύεται το έγγραφο. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | Η δομή του εγγράφου παραβιάζει τις προδιαγραφές. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | Η αιτούμενη μορφή αποθήκευσης δεν υποστηρίζεται. |

### Παραδείγματα

Δείχνει πώς να αποθηκεύσετε ένα έγγραφο χρησιμοποιώντας την απαρίθμηση SaveFormat.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingSaveFormat_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, SaveFormat.One);
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

### Δείτε επίσης

* enum [SaveFormat](../../saveformat/)
* class [Document](../)
* χώρος ονομάτων [Aspose.Note](../../document/)
* συνέλευση [Aspose.Note](../../../)

---

## Save(Stream, SaveFormat) {#save_1}

Αποθηκεύει το έγγραφο του OneNote σε μια ροή με την καθορισμένη μορφή.

```csharp
public void Save(Stream stream, SaveFormat format)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| stream | Stream | Το System.IO.Ροή όπου θα αποθηκευτεί το έγγραφο. |
| format | SaveFormat | Η μορφή με την οποία αποθηκεύεται το έγγραφο. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | Η δομή του εγγράφου παραβιάζει τις προδιαγραφές. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | Η αιτούμενη μορφή αποθήκευσης δεν υποστηρίζεται. |

### Παραδείγματα

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

Δείχνει πώς να αποθηκεύσετε ένα έγγραφο σε μια ροή.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

MemoryStream dstStream = new MemoryStream();
doc.Save(dstStream, SaveFormat.Pdf);

// Επανατύλιξη της θέσης ροής πίσω στο μηδέν, ώστε να είναι έτοιμη για την επόμενη ανάγνωση.
dstStream.Seek(0, SeekOrigin.Begin);
```

Δείχνει πώς να εφαρμόσετε το στυλ σκούρου θέματος σε ένα έγγραφο.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Text();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document doc = new Document(Path.Combine(dataDir, "Aspose.one"));

foreach (var page in doc)
{
    page.BackgroundColor = Color.Black;
}

foreach (var node in doc.GetChildNodes<RichText>())
{
    var c = node.ParagraphStyle.FontColor;
    if (c.IsEmpty || Math.Abs(c.R - Color.Black.R) + Math.Abs(c.G - Color.Black.G) + Math.Abs(c.B - Color.Black.B) <= 30)
    {
        node.ParagraphStyle.FontColor = Color.White;
    }
}

doc.Save(Path.Combine(dataDir, "AsposeDarkTheme.pdf"));
```

### Δείτε επίσης

* enum [SaveFormat](../../saveformat/)
* class [Document](../)
* χώρος ονομάτων [Aspose.Note](../../document/)
* συνέλευση [Aspose.Note](../../../)

---

## Save(string, SaveOptions) {#save_5}

Αποθηκεύει το έγγραφο του OneNote σε ένα αρχείο χρησιμοποιώντας τις καθορισμένες επιλογές αποθήκευσης.

```csharp
public void Save(string fileName, SaveOptions options)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fileName | String | Το πλήρες όνομα του αρχείου. Εάν υπάρχει ήδη ένα αρχείο με το καθορισμένο πλήρες όνομα, το υπάρχον αρχείο αντικαθίσταται. |
| options | SaveOptions | Καθορίζει τις επιλογές για τον τρόπο αποθήκευσης του εγγράφου στο αρχείο. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | Η δομή του εγγράφου παραβιάζει τις προδιαγραφές. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | Η αιτούμενη μορφή αποθήκευσης δεν υποστηρίζεται. |

### Παραδείγματα

Δείχνει πώς να αποθηκεύσετε ένα έγγραφο χρησιμοποιώντας το OneSaveOptions.

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingOneSaveOptions_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, new OneSaveOptions());
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

Δείχνει πώς να αποθηκεύσετε ένα έγγραφο σε μορφή Pdf με διάταξη σελίδας Letter.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingLetterPageSettings.pdf");

// Αποθηκεύστε το έγγραφο.
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.Letter });
```

Δείχνει πώς να αποθηκεύσετε ένα έγγραφο σε μορφή Pdf με διάταξη σελίδας Α4 χωρίς όριο ύψους.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingA4PageSettingsWithoutHeightLimit.pdf");

// Αποθηκεύστε το έγγραφο.
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.A4NoHeightLimit });
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

Δείχνει πώς να αποθηκεύσετε ένα έγγραφο σε μορφή pdf.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Αρχικοποίηση αντικειμένου PdfSaveOptions
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Ορισμός ευρετηρίου σελίδας της πρώτης σελίδας που θα αποθηκευτεί
                              PageIndex = 0,

                              // Ορισμός αριθμού σελίδων
                              PageCount = 1,
                          };

// Αποθηκεύστε το έγγραφο ως PDF
dataDir = dataDir + "SaveRangeOfPagesAsPDF_out.pdf";
oneFile.Save(dataDir, opts);
```

Δείχνει πώς να αποθηκεύσετε ένα έγγραφο σε μορφή pdf χρησιμοποιώντας συγκεκριμένες ρυθμίσεις.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

// Αρχικοποίηση αντικειμένου PdfSaveOptions
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // Χρησιμοποιήστε συμπίεση Jpeg
                              ImageCompression = Saving.Pdf.PdfImageCompression.Jpeg,

                              // Ποιότητα για συμπίεση JPEG
                              JpegQuality = 90
                          };

dataDir = dataDir + "Document.SaveWithOptions_out.pdf";
doc.Save(dataDir, opts);
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

* class [SaveOptions](../../../aspose.note.saving/saveoptions/)
* class [Document](../)
* χώρος ονομάτων [Aspose.Note](../../document/)
* συνέλευση [Aspose.Note](../../../)

---

## Save(Stream, SaveOptions) {#save_2}

Αποθηκεύει το έγγραφο του OneNote σε μια ροή χρησιμοποιώντας τις καθορισμένες επιλογές αποθήκευσης.

```csharp
public void Save(Stream stream, SaveOptions options)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| stream | Stream | Το System.IO.Ροή όπου θα αποθηκευτεί το έγγραφο. |
| options | SaveOptions | Καθορίζει τις επιλογές για τον τρόπο αποθήκευσης του εγγράφου σε ροή. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | Η δομή του εγγράφου παραβιάζει τις προδιαγραφές. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | Η αιτούμενη μορφή αποθήκευσης δεν υποστηρίζεται. |

### Παραδείγματα

Δείχνει πώς να αποθηκεύσετε ένα έγγραφο σε μορφή pdf χρησιμοποιώντας καθορισμένη προεπιλεγμένη γραμματοσειρά.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Αποθηκεύστε το έγγραφο ως PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontName_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions() 
                      {
                          FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFont("Times New Roman")
                      });
```

Δείχνει πώς να αποθηκεύσετε ένα έγγραφο σε μορφή pdf χρησιμοποιώντας την προεπιλεγμένη γραμματοσειρά από ένα αρχείο.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// Φόρτωση του εγγράφου στο Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Αποθηκεύστε το έγγραφο ως PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromFile_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions()
                          {
                              FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromFile(fontFile)
                          });
```

Δείχνει πώς να αποθηκεύσετε ένα έγγραφο σε μορφή pdf χρησιμοποιώντας προεπιλεγμένη γραμματοσειρά από μια ροή.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// Φόρτωση του εγγράφου στο Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Αποθηκεύστε το έγγραφο ως PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromStream_out.pdf";

using (var stream = File.Open(fontFile, FileMode.Open, FileAccess.Read, FileShare.Read))
{
    oneFile.Save(dataDir, new PdfSaveOptions()
                              {
                                  FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromStream(stream)
                              });
}
```

### Δείτε επίσης

* class [SaveOptions](../../../aspose.note.saving/saveoptions/)
* class [Document](../)
* χώρος ονομάτων [Aspose.Note](../../document/)
* συνέλευση [Aspose.Note](../../../)


