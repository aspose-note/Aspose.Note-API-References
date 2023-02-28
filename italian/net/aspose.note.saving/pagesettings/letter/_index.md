---
title: PageSettings.Letter
second_title: Aspose.Note per .NET API Reference
description: PageSettings proprietà. Ottiene le impostazioni per la pagina in formato Lettera.
type: docs
weight: 30
url: /it/net/aspose.note.saving/pagesettings/letter/
---
## PageSettings.Letter property

Ottiene le impostazioni per la pagina in formato Lettera.

```csharp
public static PageSettings Letter { get; }
```

### Esempi

Mostra come salvare un documento in formato Pdf con layout di pagina Lettera.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Carica il documento in Aspose.Note.
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingLetterPageSettings.pdf");

// Salva il documento.
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.Letter });
```

### Guarda anche

* class [PageSettings](../)
* spazio dei nomi [Aspose.Note.Saving](../../pagesettings/)
* assemblea [Aspose.Note](../../../)


