---
title: Class UnsupportedFileFormatException
second_title: Aspose.Note för .NET API-referens
description: Aspose.Note.UnsupportedFileFormatException klass. Kastas under dokumentladdning när filformatet inte känns igen eller inte stöds av Aspose.Note.
type: docs
weight: 990
url: /sv/net/aspose.note/unsupportedfileformatexception/
---
## UnsupportedFileFormatException class

Kastas under dokumentladdning, när filformatet inte känns igen eller inte stöds av Aspose.Note.

```csharp
public class UnsupportedFileFormatException : Exception
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [FileFormat](../../aspose.note/unsupportedfileformatexception/fileformat/) { get; } | Hämtar filformatet för skickade data om det upptäcks. |

### Exempel

Visar hur du kontrollerar om en dokumentladdning misslyckades eftersom OneNote 2007-formatet inte stöds.

```csharp
// Sökvägen till dokumentkatalogen.
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

### Se även

* namnutrymme [Aspose.Note](../../aspose.note/)
* hopsättning [Aspose.Note](../../)


