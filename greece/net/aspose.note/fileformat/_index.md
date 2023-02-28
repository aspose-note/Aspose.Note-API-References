---
title: Enum FileFormat
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.FileFormat αρίθμηση. Αντιπροσωπεύει τη μορφή αρχείου OneNote.
type: docs
weight: 90
url: /el/net/aspose.note/fileformat/
---
## FileFormat enumeration

Αντιπροσωπεύει τη μορφή αρχείου OneNote.

```csharp
public enum FileFormat
```

### Αξίες

| Ονομα | αξία | Περιγραφή |
| --- | --- | --- |
| Unknown | `0` | Άγνωστη μορφή αρχείου. |
| OneNote2007 | `1` | OneNote 2010. |
| OneNote2010 | `2` | OneNote 2010. |
| OneNoteOnline | `3` | OneNote Online. |

### Παραδείγματα

Δείχνει πώς μπορείτε να ελέγξετε εάν η φόρτωση ενός εγγράφου απέτυχε επειδή δεν υποστηρίζεται η μορφή OneNote 2007.

```csharp
// Η διαδρομή προς τον κατάλογο εγγράφων.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "OneNote2007.one");

try
{
    new Document(fileName);
}
catch (UnsupportedFileFormatException e)
{
    if (e.FileFormat == FileFormat.OneNote2007)
    {
        Console.WriteLine("It looks like the provided file is in OneNote 2007 format that is not supported.");
    }
    else
        throw;
}
```

### Δείτε επίσης

* χώρος ονομάτων [Aspose.Note](../../aspose.note/)
* συνέλευση [Aspose.Note](../../)


