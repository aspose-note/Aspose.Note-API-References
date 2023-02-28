---
title: PdfSaveOptions.PageSettings
second_title: Aspose.Note för .NET API-referens
description: PdfSaveOptions fast egendom. Hämtar eller ställer in sidinställningarna för varje sida i dokumentet. Som standard beror på CurrentUICulture USAkulturer har bokstavsinställning andra har A4inställningar.
type: docs
weight: 40
url: /sv/net/aspose.note.saving/pdfsaveoptions/pagesettings/
---
## PdfSaveOptions.PageSettings property

Hämtar eller ställer in sidinställningarna för varje sida i dokumentet. Som standard beror på CurrentUICulture, *USA-kulturer har bokstavsinställning, andra har A4-inställningar.

```csharp
public PageSettings PageSettings { get; set; }
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

* class [PageSettings](../../pagesettings/)
* class [PdfSaveOptions](../)
* namnutrymme [Aspose.Note.Saving](../../pdfsaveoptions/)
* hopsättning [Aspose.Note](../../../)


