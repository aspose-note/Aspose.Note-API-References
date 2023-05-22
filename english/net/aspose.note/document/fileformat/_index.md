---
title: Document.FileFormat
second_title: Aspose.Note for .NET API Reference
description: Document property. Gets file format OneNote 2010 OneNote Online
type: docs
weight: 60
url: /net/aspose.note/document/fileformat/
---
## Document.FileFormat property

Gets file format (OneNote 2010, OneNote Online).

```csharp
public FileFormat FileFormat { get; }
```

## Examples

Shows how to get file format of a document.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");
switch (document.FileFormat)
{
    case FileFormat.OneNote2010:
        // Process OneNote 2010
        break;
    case FileFormat.OneNoteOnline:
        // Process OneNote Online
        break;
}
```

### See Also

* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)


