---
title: Document.FileFormat
second_title: Aspose.Note for .NET API Reference
description: Document ιδιοκτησία. Λαμβάνει μορφή αρχείου OneNote 2010 OneNote Online.
type: docs
weight: 60
url: /el/net/aspose.note/document/fileformat/
---
## Document.FileFormat property

Λαμβάνει μορφή αρχείου (OneNote 2010, OneNote Online).

```csharp
public FileFormat FileFormat { get; }
```

### Παραδείγματα

Δείχνει πώς να αποκτήσετε τη μορφή αρχείου ενός εγγράφου.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");
switch (document.FileFormat)
{
    case FileFormat.OneNote2010:
        // Process OneNote 2010
        break;
    case FileFormat.OneNoteOnline:
        // Επεξεργαστείτε το OneNote Online
        break;
}
```

### Δείτε επίσης

* enum [FileFormat](../../fileformat/)
* class [Document](../)
* χώρος ονομάτων [Aspose.Note](../../document/)
* συνέλευση [Aspose.Note](../../../)


