---
title: PageSettings.Letter
second_title: Aspose.Note for .NET API Reference
description: PageSettings property. Gets settings for the Letterformat page
type: docs
weight: 30
url: /net/aspose.note.saving/pagesettings/letter/
---
## PageSettings.Letter property

Gets settings for the Letter-format page.

```csharp
public static PageSettings Letter { get; }
```

## Examples

Shows how to save a document in Pdf format with Letter page layout.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Load the document into Aspose.Note.
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingLetterPageSettings.pdf");

// Save the document.
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.Letter });
```

### See Also

* class [PageSettings](../)
* namespace [Aspose.Note.Saving](../../pagesettings/)
* assembly [Aspose.Note](../../../)


