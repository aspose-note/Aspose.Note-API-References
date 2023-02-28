---
title: PageSettings.A4NoHeightLimit
second_title: Aspose.Note per .NET API Reference
description: PageSettings proprietà. Ottiene le impostazioni per la pagina in formato A4 con altezza illimitata.
type: docs
weight: 20
url: /it/net/aspose.note.saving/pagesettings/a4noheightlimit/
---
## PageSettings.A4NoHeightLimit property

Ottiene le impostazioni per la pagina in formato A4 con altezza illimitata.

```csharp
public static PageSettings A4NoHeightLimit { get; }
```

### Esempi

Mostra come salvare un documento in formato Pdf con layout di pagina A4 senza limiti di altezza.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Carica il documento in Aspose.Note.
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingA4PageSettingsWithoutHeightLimit.pdf");

// Salva il documento.
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.A4NoHeightLimit });
```

### Guarda anche

* class [PageSettings](../)
* spazio dei nomi [Aspose.Note.Saving](../../pagesettings/)
* assemblea [Aspose.Note](../../../)


