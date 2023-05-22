---
title: AttachedFile.Bytes
second_title: Aspose.Note for .NET API Reference
description: AttachedFile property. Gets the binary data for an embedded file
type: docs
weight: 50
url: /net/aspose.note/attachedfile/bytes/
---
## AttachedFile.Bytes property

Gets the binary data for an embedded file.

```csharp
public byte[] Bytes { get; }
```

## Examples

Shows how to get content of an attached file.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_Attachments();

// Load the document into Aspose.Note.
Document oneFile = new Document(dataDir + "Sample1.one");

// Get a list of attached file nodes
IList<AttachedFile> nodes = oneFile.GetChildNodes<AttachedFile>();

// Iterate through all nodes
foreach (AttachedFile file in nodes)
{
    // Load attached file to a stream object
    using (Stream outputStream = new MemoryStream(file.Bytes))
    {
        // Create a local file
        using (Stream fileStream = System.IO.File.OpenWrite(String.Format(dataDir + file.FileName)))
        {
            // Copy file stream
            CopyStream(outputStream, fileStream);
        }
    }
}
```

### See Also

* class [AttachedFile](../)
* namespace [Aspose.Note](../../attachedfile/)
* assembly [Aspose.Note](../../../)


