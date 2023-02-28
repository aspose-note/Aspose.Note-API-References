---
title: Image.Tags
second_title: Aspose.Note for .NET API Reference
description: Image ιδιοκτησία. Λαμβάνει τη λίστα με όλες τις ετικέτες μιας παραγράφου.
type: docs
weight: 160
url: /el/net/aspose.note/image/tags/
---
## Image.Tags property

Λαμβάνει τη λίστα με όλες τις ετικέτες μιας παραγράφου.

```csharp
public List<ITag> Tags { get; }
```

### Παραδείγματα

Δείχνει πώς να προσθέσετε νέα εικόνα με ετικέτα.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Tags();

// Δημιουργήστε ένα αντικείμενο της κλάσης Document
Document doc = new Document();

// Αρχικοποίηση αντικειμένου κλάσης σελίδας
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Αρχικοποίηση αντικειμένου κλάσης Outline
Outline outline = new Outline(doc);

// Αρχικοποίηση αντικειμένου κλάσης OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

// Φόρτωση εικόνας
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "icon.jpg");

// Εισαγωγή εικόνας στον κόμβο του εγγράφου
outlineElem.AppendChildLast(image);
image.Tags.Add(NoteTag.CreateYellowStar());

// Προσθήκη κόμβου στοιχείου περιγράμματος
outline.AppendChildLast(outlineElem);

// Προσθήκη κόμβου περιγράμματος
page.AppendChildLast(outline);

// Προσθήκη κόμβου σελίδας
doc.AppendChildLast(page);

// Αποθήκευση εγγράφου OneNote
dataDir = dataDir + "AddImageNodeWithTag_out.one";
doc.Save(dataDir);
```

### Δείτε επίσης

* interface [ITag](../../itag/)
* class [Image](../)
* χώρος ονομάτων [Aspose.Note](../../image/)
* συνέλευση [Aspose.Note](../../../)


