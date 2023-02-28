---
title: PageSettings.A4NoHeightLimit
second_title: Aspose.Note voor .NET API-referentie
description: PageSettings eigendom. Krijgt instellingen voor de A4formaat pagina met onbeperkte hoogte.
type: docs
weight: 20
url: /nl/net/aspose.note.saving/pagesettings/a4noheightlimit/
---
## PageSettings.A4NoHeightLimit property

Krijgt instellingen voor de A4-formaat pagina met onbeperkte hoogte.

```csharp
public static PageSettings A4NoHeightLimit { get; }
```

### Voorbeelden

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

* class [PageSettings](../)
* naamruimte [Aspose.Note.Saving](../../pagesettings/)
* montage [Aspose.Note](../../../)


