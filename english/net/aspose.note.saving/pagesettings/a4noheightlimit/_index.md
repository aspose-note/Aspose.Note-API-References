---
title: PageSettings.A4NoHeightLimit
second_title: Aspose.Note for .NET API Reference
description: PageSettings property. Gets settings for the A4format page with limitless height
type: docs
weight: 20
url: /net/aspose.note.saving/pagesettings/a4noheightlimit/
---
## PageSettings.A4NoHeightLimit property

Gets settings for the A4-format page with limitless height.

```csharp
public static PageSettings A4NoHeightLimit { get; }
```

## Examples

Shows how to save a document in Pdf format with A4 page layout without height limit.

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Load the document into Aspose.Note.
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingA4PageSettingsWithoutHeightLimit.pdf");

// Save the document.
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.A4NoHeightLimit });
```

### See Also

* class [PageSettings](../)
* namespace [Aspose.Note.Saving](../../pagesettings/)
* assembly [Aspose.Note](../../../)


