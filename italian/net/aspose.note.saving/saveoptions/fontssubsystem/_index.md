---
title: SaveOptions.FontsSubsystem
second_title: Aspose.Note per .NET API Reference
description: SaveOptions proprietà. Ottiene o imposta le impostazioni del carattere da utilizzare durante il salvataggio
type: docs
weight: 10
url: /it/net/aspose.note.saving/saveoptions/fontssubsystem/
---
## SaveOptions.FontsSubsystem property

Ottiene o imposta le impostazioni del carattere da utilizzare durante il salvataggio

```csharp
public FontsSubsystem FontsSubsystem { get; set; }
```

### Esempi

Mostra come salvare un documento in formato pdf utilizzando il carattere predefinito specificato.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Carica il documento in Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Salva il documento come PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontName_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions() 
                      {
                          FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFont("Times New Roman")
                      });
```

Mostra come salvare un documento in formato pdf utilizzando il carattere predefinito da un file.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// Carica il documento in Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Salva il documento come PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromFile_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions()
                          {
                              FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromFile(fontFile)
                          });
```

Mostra come salvare un documento in formato pdf utilizzando il carattere predefinito da un flusso.

```csharp
// Il percorso della directory dei documenti.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// Carica il documento in Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Salva il documento come PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromStream_out.pdf";

using (var stream = File.Open(fontFile, FileMode.Open, FileAccess.Read, FileShare.Read))
{
    oneFile.Save(dataDir, new PdfSaveOptions()
                              {
                                  FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromStream(stream)
                              });
}
```

### Guarda anche

* class [FontsSubsystem](../../../aspose.note.fonts/fontssubsystem/)
* class [SaveOptions](../)
* spazio dei nomi [Aspose.Note.Saving](../../saveoptions/)
* assemblea [Aspose.Note](../../../)


