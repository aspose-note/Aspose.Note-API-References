---
title: PdfSaveOptions.PageSettings
second_title: Aspose.Note voor .NET API-referentie
description: PdfSaveOptions eigendom. Hiermee worden de paginainstellingen voor elke pagina in het document opgehaald of ingesteld. Standaard afhankelijk van CurrentUICulture Amerikaanse culturen hebben letterinstellingen andere hebben A4instellingen.
type: docs
weight: 40
url: /nl/net/aspose.note.saving/pdfsaveoptions/pagesettings/
---
## PdfSaveOptions.PageSettings property

Hiermee worden de pagina-instellingen voor elke pagina in het document opgehaald of ingesteld. Standaard afhankelijk van CurrentUICulture, *Amerikaanse culturen hebben letterinstellingen, andere hebben A4-instellingen.

```csharp
public PageSettings PageSettings { get; set; }
```

### Voorbeelden

Laat zien hoe u een document in pdf-indeling kunt opslaan met de pagina-indeling Letter.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laad het document in Aspose.Note.
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingLetterPageSettings.pdf");

// Sla het document op.
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.Letter });
```

Laat zien hoe u een document opslaat in Pdf-formaat met A4-paginalay-out zonder hoogtebeperking.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laad het document in Aspose.Note.
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingA4PageSettingsWithoutHeightLimit.pdf");

// Sla het document op.
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.A4NoHeightLimit });
```

### Zie ook

* class [PageSettings](../../pagesettings/)
* class [PdfSaveOptions](../)
* naamruimte [Aspose.Note.Saving](../../pdfsaveoptions/)
* montage [Aspose.Note](../../../)


