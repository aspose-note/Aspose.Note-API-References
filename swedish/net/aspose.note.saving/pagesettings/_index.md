---
title: Class PageSettings
second_title: Aspose.Note för .NET API-referens
description: Aspose.Note.Saving.PageSettings klass. Representerar layoutinställningarna för en sida.
type: docs
weight: 820
url: /sv/net/aspose.note.saving/pagesettings/
---
## PageSettings class

Representerar layoutinställningarna för en sida.

```csharp
public class PageSettings
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| static [A4](../../aspose.note.saving/pagesettings/a4/) { get; } | Hämtar inställningar för sidan i A4-format. |
| static [A4NoHeightLimit](../../aspose.note.saving/pagesettings/a4noheightlimit/) { get; } | Får inställningar för sidan i A4-format med obegränsad höjd. |
| static [Letter](../../aspose.note.saving/pagesettings/letter/) { get; } | Hämtar inställningar för sidan med bokstavsformat. |
| static [LetterNoHeightLimit](../../aspose.note.saving/pagesettings/letternoheightlimit/) { get; } | Hämtar inställningar för sidan med bokstavsformat med obegränsad höjd. |

### Exempel

Visar hur man sparar ett dokument i pdf-format med Letter-sidlayout.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Ladda dokumentet i Aspose.Note.
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingLetterPageSettings.pdf");

// Spara dokumentet.
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.Letter });
```

Visar hur man sparar ett dokument i pdf-format med A4 sidlayout utan höjdbegränsning.

```csharp
// Sökvägen till dokumentkatalogen.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Ladda dokumentet i Aspose.Note.
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingA4PageSettingsWithoutHeightLimit.pdf");

// Spara dokumentet.
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.A4NoHeightLimit });
```

### Se även

* namnutrymme [Aspose.Note.Saving](../../aspose.note.saving/)
* hopsättning [Aspose.Note](../../)


