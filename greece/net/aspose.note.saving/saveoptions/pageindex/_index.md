---
title: SaveOptions.PageIndex
second_title: Aspose.Note for .NET API Reference
description: SaveOptions ιδιοκτησία. Λαμβάνει ή ορίζει το ευρετήριο της πρώτης σελίδας προς αποθήκευση. Από προεπιλογή είναι 0.
type: docs
weight: 30
url: /el/net/aspose.note.saving/saveoptions/pageindex/
---
## SaveOptions.PageIndex property

Λαμβάνει ή ορίζει το ευρετήριο της πρώτης σελίδας προς αποθήκευση. Από προεπιλογή είναι 0.

```csharp
public int PageIndex { get; set; }
```

### Παραδείγματα

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

Δείχνει πώς να δημιουργήσετε ένα έγγραφο και να αποθηκεύσετε σε μορφή html το καθορισμένο εύρος σελίδων.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Εκκίνηση εγγράφου OneNote
Document doc = new Document();

Page page = doc.AppendChildLast(new Page());

// Προεπιλεγμένο στυλ για όλο το κείμενο του εγγράφου.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title()
             {
                 TitleText = new RichText() { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText() { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText() { Text = "12:34", ParagraphStyle = textStyle }
             };

// Αποθήκευση σε μορφή HTML
dataDir = dataDir + "CreateAndSavePageRange_out.html";
doc.Save(dataDir, new HtmlSaveOptions
                  {
                      PageCount = 1,
                      PageIndex = 0
                  });
```

Δείχνει πώς να δημιουργήσετε ένα έγγραφο με μορφοποιημένο εμπλουτισμένο κείμενο.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Δημιουργήστε ένα αντικείμενο της κλάσης Document
Document doc = new Document();

// Αρχικοποίηση αντικειμένου κλάσης σελίδας
Page page = new Page();

// Αρχικοποίηση αντικειμένου κλάσης τίτλου
Title title = new Title();

// Εκκίνηση αντικειμένου κλάσης TextStyle και ορισμός ιδιοτήτων μορφοποίησης
ParagraphStyle defaultTextStyle = new ParagraphStyle
                                      {
                                          FontColor = Color.Black,
                                          FontName = "Arial",
                                          FontSize = 10
                                      };

RichText titleText = new RichText() { ParagraphStyle = defaultTextStyle }.Append("Title!");
Outline outline = new Outline()
                      {
                          VerticalOffset = 100,
                          HorizontalOffset = 100
                      };
OutlineElement outlineElem = new OutlineElement();

TextStyle textStyleForHelloWord = new TextStyle
                                      {
                                          FontColor = Color.Red,
                                          FontName = "Arial",
                                          FontSize = 10,
                                      };

TextStyle textStyleForOneNoteWord = new TextStyle
                                        {
                                            FontColor = Color.Green,
                                            FontName = "Calibri",
                                            FontSize = 10,
                                            IsItalic = true,
                                        };

TextStyle textStyleForTextWord = new TextStyle
                                     {
                                         FontColor = Color.Blue,
                                         FontName = "Arial",
                                         FontSize = 15,
                                         IsBold = true,
                                         IsItalic = true,
                                     };

RichText text = new RichText() { ParagraphStyle = defaultTextStyle }
                    .Append("Hello", textStyleForHelloWord)
                    .Append(" OneNote", textStyleForOneNoteWord)
                    .Append(" text", textStyleForTextWord)
                    .Append("!", TextStyle.Default);

title.TitleText = titleText;

// Ορισμός τίτλου σελίδας
page.Title = title;

// Προσθήκη κόμβου εμπλουτισμένου κειμένου
outlineElem.AppendChildLast(text);

// Προσθήκη κόμβου OutlineElement
outline.AppendChildLast(outlineElem);

// Προσθήκη κόμβου Outline
page.AppendChildLast(outline);

// Προσθήκη κόμβου σελίδας
doc.AppendChildLast(page);

// Αποθήκευση εγγράφου OneNote
dataDir = dataDir + "CreateDocWithFormattedRichText_out.one";
doc.Save(dataDir);
```

### Δείτε επίσης

* class [SaveOptions](../)
* χώρος ονομάτων [Aspose.Note.Saving](../../saveoptions/)
* συνέλευση [Aspose.Note](../../../)


