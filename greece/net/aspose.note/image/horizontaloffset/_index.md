---
title: Image.HorizontalOffset
second_title: Aspose.Note for .NET API Reference
description: Image ιδιοκτησία. Λαμβάνει ή ορίζει την οριζόντια μετατόπιση.
type: docs
weight: 100
url: /el/net/aspose.note/image/horizontaloffset/
---
## Image.HorizontalOffset property

Λαμβάνει ή ορίζει την οριζόντια μετατόπιση.

```csharp
public float HorizontalOffset { get; set; }
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

### Δείτε επίσης

* class [Image](../)
* χώρος ονομάτων [Aspose.Note](../../image/)
* συνέλευση [Aspose.Note](../../../)


