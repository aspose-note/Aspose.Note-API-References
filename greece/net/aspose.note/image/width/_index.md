---
title: Image.Width
second_title: Aspose.Note for .NET API Reference
description: Image ιδιοκτησία. Λαμβάνει ή ορίζει το πλάτος. Αυτό είναι το πραγματικό πλάτος της εικόνας στο έγγραφο MS OneNote.
type: docs
weight: 180
url: /el/net/aspose.note/image/width/
---
## Image.Width property

Λαμβάνει ή ορίζει το πλάτος. Αυτό είναι το πραγματικό πλάτος της εικόνας στο έγγραφο MS OneNote.

```csharp
public float Width { get; set; }
```

### Παραδείγματα

Δείχνει πώς να λαμβάνετε μετα-πληροφορίες εικόνας.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Images();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Λήψη όλων των κόμβων εικόνας
IList<Aspose.Note.Image> images = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in images)
{
    Console.WriteLine("Width: {0}", image.Width);
    Console.WriteLine("Height: {0}", image.Height);
    Console.WriteLine("OriginalWidth: {0}", image.OriginalWidth);
    Console.WriteLine("OriginalHeight: {0}", image.OriginalHeight);
    Console.WriteLine("FileName: {0}", image.FileName);
    Console.WriteLine("LastModifiedTime: {0}", image.LastModifiedTime);
    Console.WriteLine();
}
```

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


