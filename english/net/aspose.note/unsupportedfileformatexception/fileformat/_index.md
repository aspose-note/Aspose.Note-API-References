---
title: UnsupportedFileFormatException.FileFormat
second_title: Aspose.Note for .NET API Reference
description: UnsupportedFileFormatException property. Gets the file format of passed data if detected
type: docs
weight: 10
url: /net/aspose.note/unsupportedfileformatexception/fileformat/
---
## UnsupportedFileFormatException.FileFormat property

Gets the file format of passed data if detected.

```csharp
public FileFormat FileFormat { get; }
```

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

* enum [FileFormat](../../fileformat/)
* class [UnsupportedFileFormatException](../)
* namespace [Aspose.Note](../../unsupportedfileformatexception/)
* assembly [Aspose.Note](../../../)


