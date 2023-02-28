---
title: PageSettings.Letter
second_title: Aspose.Note voor .NET API-referentie
description: PageSettings eigendom. Krijgt instellingen voor de Letterformaat pagina.
type: docs
weight: 30
url: /nl/net/aspose.note.saving/pagesettings/letter/
---
## PageSettings.Letter property

Krijgt instellingen voor de Letter-formaat pagina.

```csharp
public static PageSettings Letter { get; }
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

### Zie ook

* class [PageSettings](../)
* naamruimte [Aspose.Note.Saving](../../pagesettings/)
* montage [Aspose.Note](../../../)


