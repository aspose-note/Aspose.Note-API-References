---
title: AttachedFile.Bytes
second_title: Aspose.Note for .NET API Reference
description: AttachedFile ιδιοκτησία. Λαμβάνει τα δυαδικά δεδομένα για ένα ενσωματωμένο αρχείο.
type: docs
weight: 50
url: /el/net/aspose.note/attachedfile/bytes/
---
## AttachedFile.Bytes property

Λαμβάνει τα δυαδικά δεδομένα για ένα ενσωματωμένο αρχείο.

```csharp
public byte[] Bytes { get; }
```

### Παραδείγματα

Δείχνει τον τρόπο λήψης περιεχομένου ενός συνημμένου αρχείου.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_Attachments();

// Φόρτωση του εγγράφου στο Aspose.Note.
Document oneFile = new Document(dataDir + "Sample1.one");

// Λάβετε μια λίστα με συνημμένους κόμβους αρχείων
IList<AttachedFile> nodes = oneFile.GetChildNodes<AttachedFile>();

// Επανάληψη σε όλους τους κόμβους
foreach (AttachedFile file in nodes)
{
    // Φόρτωση συνημμένου αρχείου σε αντικείμενο ροής
    using (Stream outputStream = new MemoryStream(file.Bytes))
    {
        // Δημιουργία τοπικού αρχείου
        using (Stream fileStream = System.IO.File.OpenWrite(String.Format(dataDir + file.FileName)))
        {
            // Αντιγραφή ροής αρχείου
            CopyStream(outputStream, fileStream);
        }
    }
}
```

### Δείτε επίσης

* class [AttachedFile](../)
* χώρος ονομάτων [Aspose.Note](../../attachedfile/)
* συνέλευση [Aspose.Note](../../../)


