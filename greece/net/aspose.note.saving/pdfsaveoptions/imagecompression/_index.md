---
title: PdfSaveOptions.ImageCompression
second_title: Aspose.Note for .NET API Reference
description: PdfSaveOptions ιδιοκτησία. Λαμβάνει ή ορίζει τον τύπο συμπίεσης που εφαρμόζεται σε εικόνες στο αρχείο PDF.
type: docs
weight: 20
url: /el/net/aspose.note.saving/pdfsaveoptions/imagecompression/
---
## PdfSaveOptions.ImageCompression property

Λαμβάνει ή ορίζει τον τύπο συμπίεσης που εφαρμόζεται σε εικόνες στο αρχείο PDF.

```csharp
public PdfImageCompression ImageCompression { get; set; }
```

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

* enum [PdfImageCompression](../../../aspose.note.saving.pdf/pdfimagecompression/)
* class [PdfSaveOptions](../)
* χώρος ονομάτων [Aspose.Note.Saving](../../pdfsaveoptions/)
* συνέλευση [Aspose.Note](../../../)


