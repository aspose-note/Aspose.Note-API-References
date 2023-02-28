---
title: DocumentFontsSubsystem.UsingDefaultFontFromStream
second_title: Aspose.Note per .NET API Reference
description: DocumentFontsSubsystem metodo. Crea una nuova istanza DocumentFontsSubsystem utilizzando un font dallo stream specificato come predefinito.
type: docs
weight: 50
url: /it/net/aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromstream/
---
## DocumentFontsSubsystem.UsingDefaultFontFromStream method

Crea una nuova istanza DocumentFontsSubsystem utilizzando un font dallo stream specificato come predefinito.

```csharp
public static DocumentFontsSubsystem UsingDefaultFontFromStream(Stream defaultFontStream, 
    Dictionary<string, string> fontsSubstitutions = null)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| defaultFontStream | Stream | Il flusso contenente il nome del carattere predefinito. |
| fontsSubstitutions | Dictionary`2 | Le sostituzioni dei caratteri. |

### Valore di ritorno

Il[`DocumentFontsSubsystem`](../) .

### Esempi

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

* class [DocumentFontsSubsystem](../)
* spazio dei nomi [Aspose.Note.Fonts](../../documentfontssubsystem/)
* assemblea [Aspose.Note](../../../)


