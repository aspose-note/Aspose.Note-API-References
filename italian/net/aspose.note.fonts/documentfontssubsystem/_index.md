---
title: Class DocumentFontsSubsystem
second_title: Aspose.Note per .NET API Reference
description: Aspose.Note.Fonts.DocumentFontsSubsystem classe. Semplice implementazione di Aspose.Note.Fonts.FontsSubsystem. RecuperaFontFamily oggetto da OS.
type: docs
weight: 100
url: /it/net/aspose.note.fonts/documentfontssubsystem/
---
## DocumentFontsSubsystem class

Semplice implementazione di Aspose.Note.Fonts.FontsSubsystem. RecuperaFontFamily oggetto da OS.

```csharp
public class DocumentFontsSubsystem : FontsSubsystem
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [DocumentFontsSubsystem](documentfontssubsystem/#constructor)(Dictionary&lt;string, string&gt;) | Inizializza una nuova istanza di`DocumentFontsSubsystem` classe. |
| [DocumentFontsSubsystem](documentfontssubsystem/#constructor_1)(Stream, Dictionary&lt;string, string&gt;) | Inizializza una nuova istanza di`DocumentFontsSubsystem` classe. |
| [DocumentFontsSubsystem](documentfontssubsystem/#constructor_2)(string, Dictionary&lt;string, string&gt;) | Inizializza una nuova istanza di`DocumentFontsSubsystem` classe. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| static [Default](../../aspose.note.fonts/documentfontssubsystem/default/) { get; set; } | Ottiene o imposta l'istanza statica predefinita. |
| [DefaultFont](../../aspose.note.fonts/fontssubsystem/defaultfont/) { get; } | Ottiene o imposta il carattere predefinito. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| static [UsingDefaultFont](../../aspose.note.fonts/documentfontssubsystem/usingdefaultfont/)(string, Dictionary&lt;string, string&gt;) | Crea una nuova istanza DocumentFontsSubsystem utilizzando il nome del carattere predefinito specificato. |
| static [UsingDefaultFontFromFile](../../aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromfile/)(string, Dictionary&lt;string, string&gt;) | Crea una nuova istanza DocumentFontsSubsystem utilizzando un font dal file specificato come predefinito. |
| static [UsingDefaultFontFromStream](../../aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromstream/)(Stream, Dictionary&lt;string, string&gt;) | Crea una nuova istanza DocumentFontsSubsystem utilizzando un font dallo stream specificato come predefinito. |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont/)(Stream) | Aggiungi il carattere. |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont/)(string) | Aggiungi il carattere. |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont/)(Stream, string) | Aggiungi il carattere. |
| [AddFontSubstitution](../../aspose.note.fonts/fontssubsystem/addfontsubstitution/)(string, string) | Aggiunge la sostituzione dei caratteri. |
| virtual [GetFontFamily](../../aspose.note.fonts/fontssubsystem/getfontfamily/)(string) | Ottiene la famiglia di caratteri. |
| [LoadFontsFromFolder](../../aspose.note.fonts/fontssubsystem/loadfontsfromfolder/)(string) | Carica tutti i font TrueType dalla cartella specificata alla raccolta interna. |

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

* class [FontsSubsystem](../fontssubsystem/)
* spazio dei nomi [Aspose.Note.Fonts](../../aspose.note.fonts/)
* assemblea [Aspose.Note](../../)


