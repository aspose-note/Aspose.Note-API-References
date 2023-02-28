---
title: Image.OriginalHeight
second_title: Aspose.Note for .NET API Reference
description: Image ιδιοκτησία. Λαμβάνει το αρχικό ύψος. Αυτό είναι το αρχικό πλάτος της εικόνας πριν από την αλλαγή μεγέθους.
type: docs
weight: 140
url: /el/net/aspose.note/image/originalheight/
---
## Image.OriginalHeight property

Λαμβάνει το αρχικό ύψος. Αυτό είναι το αρχικό πλάτος της εικόνας, πριν από την αλλαγή μεγέθους.

```csharp
public float OriginalHeight { get; }
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

### Δείτε επίσης

* class [Image](../)
* χώρος ονομάτων [Aspose.Note](../../image/)
* συνέλευση [Aspose.Note](../../../)


