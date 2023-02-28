---
title: PageSettings.A4NoHeightLimit
second_title: Aspose.Note för .NET API-referens
description: PageSettings fast egendom. Får inställningar för sidan i A4format med obegränsad höjd.
type: docs
weight: 20
url: /sv/net/aspose.note.saving/pagesettings/a4noheightlimit/
---
## PageSettings.A4NoHeightLimit property

Får inställningar för sidan i A4-format med obegränsad höjd.

```csharp
public static PageSettings A4NoHeightLimit { get; }
```

### Exempel

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

* class [PageSettings](../)
* namnutrymme [Aspose.Note.Saving](../../pagesettings/)
* hopsättning [Aspose.Note](../../../)


