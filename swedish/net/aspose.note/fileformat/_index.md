---
title: Enum FileFormat
second_title: Aspose.Note för .NET API-referens
description: Aspose.Note.FileFormat uppräkning. Representerar OneNotefilformat.
type: docs
weight: 90
url: /sv/net/aspose.note/fileformat/
---
## FileFormat enumeration

Representerar OneNote-filformat.

```csharp
public enum FileFormat
```

### Värderingar

| namn | Värde | Beskrivning |
| --- | --- | --- |
| Unknown | `0` | Okänt filformat. |
| OneNote2007 | `1` | OneNote 2010. |
| OneNote2010 | `2` | OneNote 2010. |
| OneNoteOnline | `3` | OneNote Online. |

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


