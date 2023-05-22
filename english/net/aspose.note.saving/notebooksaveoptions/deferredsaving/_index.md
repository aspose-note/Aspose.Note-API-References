---
title: NotebookSaveOptions.DeferredSaving
second_title: Aspose.Note for .NET API Reference
description: NotebookSaveOptions property. Gets or sets a value indicating whether children documents should be saved explicitly
type: docs
weight: 10
url: /net/aspose.note.saving/notebooksaveoptions/deferredsaving/
---
## NotebookSaveOptions.DeferredSaving property

Gets or sets a value indicating whether children documents should be saved explicitly.

```csharp
public bool DeferredSaving { get; set; }
```

## Remarks

Default value is `false`, so child documents will be saved implicitly. Value `true` is indicating that user should save each notebook's child node explicitly. If notebook is saving to stream, the value is always `true` despite was explicitly set by user to `false`.

### See Also

* class [NotebookSaveOptions](../)
* namespace [Aspose.Note.Saving](../../notebooksaveoptions/)
* assembly [Aspose.Note](../../../)


