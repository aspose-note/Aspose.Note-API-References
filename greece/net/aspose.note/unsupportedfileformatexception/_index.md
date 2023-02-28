---
title: Class UnsupportedFileFormatException
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.UnsupportedFileFormatException τάξη. Ρίχτηκε κατά τη φόρτωση του εγγράφου όταν η μορφή αρχείου δεν αναγνωρίζεται ή δεν υποστηρίζεται από το Aspose.Σημείωση.
type: docs
weight: 990
url: /el/net/aspose.note/unsupportedfileformatexception/
---
## UnsupportedFileFormatException class

Ρίχτηκε κατά τη φόρτωση του εγγράφου, όταν η μορφή αρχείου δεν αναγνωρίζεται ή δεν υποστηρίζεται από το Aspose.Σημείωση.

```csharp
public class UnsupportedFileFormatException : Exception
```

## Ιδιότητες

| Ονομα | Περιγραφή |
| --- | --- |
| [FileFormat](../../aspose.note/unsupportedfileformatexception/fileformat/) { get; } | Λαμβάνει τη μορφή αρχείου των δεδομένων που έχουν περάσει εάν εντοπιστεί. |

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


