---
title: CompositeNode1.GetChildNodes
second_title: Aspose.Note for .NET API Reference
description: CompositeNode μέθοδος. Λήψη όλων των θυγατρικών κόμβων ανά τύπο κόμβου.
type: docs
weight: 70
url: /el/net/aspose.note/compositenode-1/getchildnodes/
---
## CompositeNode&lt;T&gt;.GetChildNodes&lt;T1&gt; method

Λήψη όλων των θυγατρικών κόμβων ανά τύπο κόμβου.

```csharp
public override List<T1> GetChildNodes<T1>()
    where T1 : class, INode
```

| Παράμετρος | Περιγραφή |
| --- | --- |
| T1 | Ο τύπος των στοιχείων στη λίστα που επιστρέφεται. |

### Επιστρεφόμενη Αξία

Μια λίστα με θυγατρικούς κόμβους.

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

* interface [INode](../../inode/)
* class [CompositeNode&lt;T&gt;](../)
* χώρος ονομάτων [Aspose.Note](../../compositenode-1/)
* συνέλευση [Aspose.Note](../../../)


