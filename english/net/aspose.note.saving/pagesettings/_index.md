---
title: Class PageSettings
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.Saving.PageSettings class. Represents the layout settings for a page
type: docs
weight: 750
url: /net/aspose.note.saving/pagesettings/
---
## PageSettings class

Represents the layout settings for a page.

```csharp
public class PageSettings
```

## Properties

| Name | Description |
| --- | --- |
| static [A4](../../aspose.note.saving/pagesettings/a4/) { get; } | Gets settings for the A4-format page. |
| static [A4NoHeightLimit](../../aspose.note.saving/pagesettings/a4noheightlimit/) { get; } | Gets settings for the A4-format page with limitless height. |
| static [Letter](../../aspose.note.saving/pagesettings/letter/) { get; } | Gets settings for the Letter-format page. |
| static [LetterNoHeightLimit](../../aspose.note.saving/pagesettings/letternoheightlimit/) { get; } | Gets settings for the Letter-format page with limitless height. |

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

* namespace [Aspose.Note.Saving](../../aspose.note.saving/)
* assembly [Aspose.Note](../../)


