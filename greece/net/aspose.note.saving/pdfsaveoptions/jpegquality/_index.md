---
title: PdfSaveOptions.JpegQuality
second_title: Aspose.Note for .NET API Reference
description: PdfSaveOptions ιδιοκτησία. Λαμβάνει ή ορίζει μια τιμή που καθορίζει την ποιότητα των εικόνων JPEG μέσα στο έγγραφο PDF. Η τιμή μπορεί να ποικίλλει από 0 έως 100 όπου 0 σημαίνει χειρότερη ποιότητα αλλά μέγιστη συμπίεση και 100 σημαίνει καλύτερη ποιότητα αλλά ελάχιστη συμπίεση.
type: docs
weight: 30
url: /el/net/aspose.note.saving/pdfsaveoptions/jpegquality/
---
## PdfSaveOptions.JpegQuality property

Λαμβάνει ή ορίζει μια τιμή που καθορίζει την ποιότητα των εικόνων JPEG μέσα στο έγγραφο PDF. Η τιμή μπορεί να ποικίλλει από 0 έως 100 όπου 0 σημαίνει χειρότερη ποιότητα αλλά μέγιστη συμπίεση και 100 σημαίνει καλύτερη ποιότητα αλλά ελάχιστη συμπίεση.

```csharp
public int JpegQuality { get; set; }
```

### Παρατηρήσεις

Η προεπιλεγμένη τιμή είναι 90.

### Παραδείγματα

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

### Δείτε επίσης

* class [PdfSaveOptions](../)
* χώρος ονομάτων [Aspose.Note.Saving](../../pdfsaveoptions/)
* συνέλευση [Aspose.Note](../../../)


