---
title: DocumentFontsSubsystem.UsingDefaultFontFromStream
second_title: Aspose.Note für .NET-API-Referenz
description: DocumentFontsSubsystem methode. Erstellt eine neue DocumentFontsSubsystemInstanz unter Verwendung einer Schriftart aus dem angegebenen Stream als Standard.
type: docs
weight: 50
url: /de/net/aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromstream/
---
## DocumentFontsSubsystem.UsingDefaultFontFromStream method

Erstellt eine neue DocumentFontsSubsystem-Instanz unter Verwendung einer Schriftart aus dem angegebenen Stream als Standard.

```csharp
public static DocumentFontsSubsystem UsingDefaultFontFromStream(Stream defaultFontStream, 
    Dictionary<string, string> fontsSubstitutions = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| defaultFontStream | Stream | Der Stream, der den Namen der Standardschriftart enthält. |
| fontsSubstitutions | Dictionary`2 | Die Schriftersetzungen. |

### Rückgabewert

Die[`DocumentFontsSubsystem`](../) .

### Beispiele

Zeigt, wie ein Dokument im PDF-Format mit Standardschriftart aus einem Stream gespeichert wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// Laden Sie das Dokument in Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Dokument als PDF speichern
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromStream_out.pdf";

using (var stream = File.Open(fontFile, FileMode.Open, FileAccess.Read, FileShare.Read))
{
    oneFile.Save(dataDir, new PdfSaveOptions()
                              {
                                  FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromStream(stream)
                              });
}
```

### Siehe auch

* class [DocumentFontsSubsystem](../)
* namensraum [Aspose.Note.Fonts](../../documentfontssubsystem/)
* Montage [Aspose.Note](../../../)


