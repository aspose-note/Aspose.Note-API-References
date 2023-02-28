---
title: UnsupportedFileFormatException.FileFormat
second_title: Aspose.Note for .NET API Reference
description: UnsupportedFileFormatException ιδιοκτησία. Λαμβάνει τη μορφή αρχείου των δεδομένων που έχουν περάσει εάν εντοπιστεί.
type: docs
weight: 10
url: /el/net/aspose.note/unsupportedfileformatexception/fileformat/
---
## UnsupportedFileFormatException.FileFormat property

Λαμβάνει τη μορφή αρχείου των δεδομένων που έχουν περάσει εάν εντοπιστεί.

```csharp
public FileFormat FileFormat { get; }
```

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

* enum [FileFormat](../../fileformat/)
* class [UnsupportedFileFormatException](../)
* χώρος ονομάτων [Aspose.Note](../../unsupportedfileformatexception/)
* συνέλευση [Aspose.Note](../../../)


