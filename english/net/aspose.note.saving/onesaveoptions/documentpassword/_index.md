---
title: OneSaveOptions.DocumentPassword
second_title: Aspose.Note for .NET API Reference
description: OneSaveOptions property. Gets or sets a password to encrypt the document content
type: docs
weight: 20
url: /net/aspose.note.saving/onesaveoptions/documentpassword/
---
## OneSaveOptions.DocumentPassword property

Gets or sets a password to encrypt the document content.

```csharp
public string DocumentPassword { get; set; }
```

## Examples

Shows how to save document with encryption.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_NoteBook();

Document document = new Document();
document.Save(dataDir + "CreatingPasswordProtectedDoc_out.one", new OneSaveOptions() { DocumentPassword = "pass" });
```

### See Also

* class [OneSaveOptions](../)
* namespace [Aspose.Note.Saving](../../onesaveoptions/)
* assembly [Aspose.Note](../../../)


