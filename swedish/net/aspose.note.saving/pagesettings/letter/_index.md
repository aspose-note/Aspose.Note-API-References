---
title: PageSettings.Letter
second_title: Aspose.Note för .NET API-referens
description: PageSettings fast egendom. Hämtar inställningar för sidan med bokstavsformat.
type: docs
weight: 30
url: /sv/net/aspose.note.saving/pagesettings/letter/
---
## PageSettings.Letter property

Hämtar inställningar för sidan med bokstavsformat.

```csharp
public static PageSettings Letter { get; }
```

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

### Se även

* class [PageSettings](../)
* namnutrymme [Aspose.Note.Saving](../../pagesettings/)
* hopsättning [Aspose.Note](../../../)


