---
title: PdfSaveOptions.PageSettings
second_title: Aspose.Note for .NET API Reference
description: PdfSaveOptions property. Gets or sets the page settings for each page in document. By default depends on CurrentUICulture US cultures have letter setting other have A4 settings
type: docs
weight: 40
url: /net/aspose.note.saving/pdfsaveoptions/pagesettings/
---
## PdfSaveOptions.PageSettings property

Gets or sets the page settings for each page in document. By default depends on CurrentUICulture, *US cultures have letter setting, other have A4 settings.

```csharp
public PageSettings PageSettings { get; set; }
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

* class [PageSettings](../../pagesettings/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Note.Saving](../../pdfsaveoptions/)
* assembly [Aspose.Note](../../../)


