---
title: PdfSaveOptions.PageSettings
second_title: Aspose.Note per .NET API Reference
description: PdfSaveOptions proprietà. Ottiene o imposta le impostazioni di pagina per ogni pagina nel documento. Per impostazione predefinita dipende da CurrentUICulture le culture statunitensi hanno limpostazione lettera altre hanno impostazioni A4.
type: docs
weight: 40
url: /it/net/aspose.note.saving/pdfsaveoptions/pagesettings/
---
## PdfSaveOptions.PageSettings property

Ottiene o imposta le impostazioni di pagina per ogni pagina nel documento. Per impostazione predefinita dipende da CurrentUICulture, *le culture statunitensi hanno l'impostazione lettera, altre hanno impostazioni A4.

```csharp
public PageSettings PageSettings { get; set; }
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

* class [PageSettings](../../pagesettings/)
* class [PdfSaveOptions](../)
* spazio dei nomi [Aspose.Note.Saving](../../pdfsaveoptions/)
* assemblea [Aspose.Note](../../../)


