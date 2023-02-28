---
title: Document.AutomaticLayoutChangesDetectionEnabled
second_title: Aspose.Note for .NET API Reference
description: Document ιδιοκτησία. Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν το Aspose.Note εκτελεί αυτόματα τον εντοπισμό αλλαγών διάταξης. Η προεπιλεγμένη τιμή είναιαληθής .
type: docs
weight: 20
url: /el/net/aspose.note/document/automaticlayoutchangesdetectionenabled/
---
## Document.AutomaticLayoutChangesDetectionEnabled property

Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν το Aspose.Note εκτελεί αυτόματα τον εντοπισμό αλλαγών διάταξης. Η προεπιλεγμένη τιμή είναι`αληθής` .

```csharp
public bool AutomaticLayoutChangesDetectionEnabled { get; set; }
```

### Παραδείγματα

Δείχνει πώς να αποθηκεύσετε ένα έγγραφο σε διαφορετικές μορφές.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Εκκίνηση του νέου εγγράφου
Document doc = new Document() { AutomaticLayoutChangesDetectionEnabled = false };

// Εκκίνηση της νέας σελίδας
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Προεπιλεγμένο στυλ για όλο το κείμενο του εγγράφου.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// Προσθήκη κόμβου σελίδας
doc.AppendChildLast(page);

// Αποθηκεύστε το έγγραφο του OneNote σε διαφορετικές μορφές, ορίστε το μέγεθος γραμματοσειράς κειμένου και εντοπίστε τις αλλαγές διάταξης με μη αυτόματο τρόπο.
doc.Save(dataDir + "ConsequentExportOperations_out.html");            
doc.Save(dataDir + "ConsequentExportOperations_out.pdf");            
doc.Save(dataDir + "ConsequentExportOperations_out.jpg");            
textStyle.FontSize = 11;           
doc.DetectLayoutChanges();            
doc.Save(dataDir + "ConsequentExportOperations_out.bmp");
```

### Δείτε επίσης

* class [Document](../)
* χώρος ονομάτων [Aspose.Note](../../document/)
* συνέλευση [Aspose.Note](../../../)


