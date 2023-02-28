---
title: Class PageSettings
second_title: Aspose.Note per .NET API Reference
description: Aspose.Note.Saving.PageSettings classe. Rappresenta le impostazioni di layout per una pagina.
type: docs
weight: 820
url: /it/net/aspose.note.saving/pagesettings/
---
## PageSettings class

Rappresenta le impostazioni di layout per una pagina.

```csharp
public class PageSettings
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| static [A4](../../aspose.note.saving/pagesettings/a4/) { get; } | Ottiene le impostazioni per la pagina in formato A4. |
| static [A4NoHeightLimit](../../aspose.note.saving/pagesettings/a4noheightlimit/) { get; } | Ottiene le impostazioni per la pagina in formato A4 con altezza illimitata. |
| static [Letter](../../aspose.note.saving/pagesettings/letter/) { get; } | Ottiene le impostazioni per la pagina in formato Lettera. |
| static [LetterNoHeightLimit](../../aspose.note.saving/pagesettings/letternoheightlimit/) { get; } | Ottiene le impostazioni per la pagina in formato Lettera con altezza illimitata. |

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

* spazio dei nomi [Aspose.Note.Saving](../../aspose.note.saving/)
* assemblea [Aspose.Note](../../)


