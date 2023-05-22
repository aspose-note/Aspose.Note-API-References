---
title: Enum FileFormat
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.FileFormat enum. Represents OneNote file format
type: docs
weight: 90
url: /net/aspose.note/fileformat/
---
## FileFormat enumeration

Represents OneNote file format.

```csharp
public enum FileFormat
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Unknown | `0` | Unknown file format. |
| OneNote2007 | `1` | OneNote 2010. |
| OneNote2010 | `2` | OneNote 2010. |
| OneNoteOnline | `3` | OneNote Online. |

## Examples

Shows how to check if a document load is failed because OneNote 2007 format is not supported.

```csharp
// The path to the documents directory.
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

### See Also

* namespace [Aspose.Note](../../aspose.note/)
* assembly [Aspose.Note](../../)


