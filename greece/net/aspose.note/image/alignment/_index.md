---
title: Image.Alignment
second_title: Aspose.Note for .NET API Reference
description: Image ιδιοκτησία. Λαμβάνει ή ορίζει τη στοίχιση.
type: docs
weight: 20
url: /el/net/aspose.note/image/alignment/
---
## Image.Alignment property

Λαμβάνει ή ορίζει τη στοίχιση.

```csharp
public HorizontalAlignment Alignment { get; set; }
```

### Παραδείγματα

Δείχνει πώς να προσθέσετε μια εικόνα από αρχείο σε έγγραφο με ιδιότητες καθορισμένες από το χρήστη.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Images();

// Φόρτωση εγγράφου από τη ροή.
Document doc = new Document(dataDir + "Aspose.one");

// Λάβετε την πρώτη σελίδα του εγγράφου.
Aspose.Note.Page page = doc.FirstChild;

// Φόρτωση εικόνας από το αρχείο.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // Αλλάξτε το μέγεθος της εικόνας σύμφωνα με τις ανάγκες σας (προαιρετικό).
                              Width = 100,
                              Height = 100,

                              // Ορίστε τη θέση της εικόνας στη σελίδα (προαιρετικό).
                              HorizontalOffset = 100,
                              VerticalOffset = 400,

                              // Ορισμός στοίχισης εικόνας
                              Alignment = HorizontalAlignment.Right
                          };

// Προσθέστε την εικόνα στη σελίδα.
page.AppendChildLast(image);
```

Δείχνει πώς να προσθέσετε μια εικόνα από τη ροή σε ένα έγγραφο.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Images();

// Δημιουργήστε ένα αντικείμενο της κλάσης Document
Document doc = new Document();

// Αρχικοποίηση αντικειμένου κλάσης σελίδας
Aspose.Note.Page page = new Aspose.Note.Page(doc);

Outline outline1 = new Outline(doc);
OutlineElement outlineElem1 = new OutlineElement(doc);

using (FileStream fs = File.OpenRead(dataDir + "image.jpg"))
{

    // Φορτώστε τη δεύτερη εικόνα χρησιμοποιώντας το όνομα, την επέκταση και τη ροή της εικόνας.
    Aspose.Note.Image image1 = new Aspose.Note.Image(doc, "Penguins.jpg", fs)
                                   {
                                       // Ορισμός στοίχισης εικόνας
                                       Alignment = HorizontalAlignment.Right
                                   };

    outlineElem1.AppendChildLast(image1);
}

outline1.AppendChildLast(outlineElem1);
page.AppendChildLast(outline1);

doc.AppendChildLast(page);

// Αποθήκευση εγγράφου OneNote
dataDir = dataDir + "BuildDocAndInsertImageUsingImageStream_out.one";
doc.Save(dataDir);
```

Δείχνει πώς να προσθέσετε μια εικόνα από αρχείο σε έγγραφο.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Images();

// Δημιουργήστε ένα αντικείμενο της κλάσης Document
Document doc = new Document();

// Αρχικοποίηση αντικειμένου κλάσης σελίδας
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Εκκίνηση αντικειμένου κλάσης Outline και ορισμός ιδιοτήτων μετατόπισης
Outline outline = new Outline(doc);

// Αρχικοποίηση αντικειμένου κλάσης OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

// Φόρτωση εικόνας από τη διαδρομή του αρχείου.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // Ορισμός στοίχισης εικόνας
                              Alignment = HorizontalAlignment.Right
                          };

// Προσθέστε εικόνα
outlineElem.AppendChildLast(image);

// Προσθήκη στοιχείων περιγράμματος
outline.AppendChildLast(outlineElem);

// Προσθήκη κόμβου Outline
page.AppendChildLast(outline);

// Προσθήκη κόμβου σελίδας
doc.AppendChildLast(page);

// Αποθήκευση εγγράφου OneNote
dataDir = dataDir + "BuildDocAndInsertImage_out.one";
doc.Save(dataDir);
```

### Δείτε επίσης

* enum [HorizontalAlignment](../../horizontalalignment/)
* class [Image](../)
* χώρος ονομάτων [Aspose.Note](../../image/)
* συνέλευση [Aspose.Note](../../../)


