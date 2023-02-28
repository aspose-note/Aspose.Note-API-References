---
title: Image.Bytes
second_title: Aspose.Note for .NET API Reference
description: Image ιδιοκτησία. Λαμβάνει το χώρο αποθήκευσης δεδομένων εικόνας.
type: docs
weight: 50
url: /el/net/aspose.note/image/bytes/
---
## Image.Bytes property

Λαμβάνει το χώρο αποθήκευσης δεδομένων εικόνας.

```csharp
public byte[] Bytes { get; }
```

### Παραδείγματα

Δείχνει πώς να λάβετε μια εικόνα από ένα έγγραφο.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Images();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Λήψη όλων των κόμβων εικόνας
IList<Aspose.Note.Image> nodes = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in nodes)
{
    using (MemoryStream stream = new MemoryStream(image.Bytes))
    {
        using (Bitmap bitMap = new Bitmap(stream))
        {
            // Αποθήκευση byte εικόνας σε ένα αρχείο
            bitMap.Save(String.Format(dataDir + "{0}", Path.GetFileName(image.FileName)));
        }
    }
}
```

### Δείτε επίσης

* class [Image](../)
* χώρος ονομάτων [Aspose.Note](../../image/)
* συνέλευση [Aspose.Note](../../../)


