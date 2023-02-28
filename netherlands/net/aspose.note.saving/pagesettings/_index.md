---
title: Class PageSettings
second_title: Aspose.Note voor .NET API-referentie
description: Aspose.Note.Saving.PageSettings klas. Vertegenwoordigt de layoutinstellingen voor een pagina.
type: docs
weight: 820
url: /nl/net/aspose.note.saving/pagesettings/
---
## PageSettings class

Vertegenwoordigt de lay-outinstellingen voor een pagina.

```csharp
public class PageSettings
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| static [A4](../../aspose.note.saving/pagesettings/a4/) { get; } | Krijgt instellingen voor de A4-formaat pagina. |
| static [A4NoHeightLimit](../../aspose.note.saving/pagesettings/a4noheightlimit/) { get; } | Krijgt instellingen voor de A4-formaat pagina met onbeperkte hoogte. |
| static [Letter](../../aspose.note.saving/pagesettings/letter/) { get; } | Krijgt instellingen voor de Letter-formaat pagina. |
| static [LetterNoHeightLimit](../../aspose.note.saving/pagesettings/letternoheightlimit/) { get; } | Krijgt instellingen voor de pagina in Letter-formaat met onbeperkte hoogte. |

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

* naamruimte [Aspose.Note.Saving](../../aspose.note.saving/)
* montage [Aspose.Note](../../)


