---
title: DocumentFontsSubsystem.UsingDefaultFontFromFile
second_title: Aspose.Note für .NET-API-Referenz
description: DocumentFontsSubsystem methode. Erstellt eine neue DocumentFontsSubsystemInstanz unter Verwendung einer Schriftart aus der angegebenen Datei als Standard.
type: docs
weight: 40
url: /de/net/aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromfile/
---
## DocumentFontsSubsystem.UsingDefaultFontFromFile method

Erstellt eine neue DocumentFontsSubsystem-Instanz unter Verwendung einer Schriftart aus der angegebenen Datei als Standard.

```csharp
public static DocumentFontsSubsystem UsingDefaultFontFromFile(string filePath, 
    Dictionary<string, string> fontsSubstitutions = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| filePath | String | Die Datei mit dem Namen der Standardschriftart. |
| fontsSubstitutions | Dictionary`2 | Die Schriftersetzungen. |

### Rückgabewert

Die[`DocumentFontsSubsystem`](../) .

### Beispiele

Zeigt, wie ein Dokument im PDF-Format mit Standardschriftart aus einer Datei gespeichert wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// Laden Sie das Dokument in Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Dokument als PDF speichern
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromFile_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions()
                          {
                              FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromFile(fontFile)
                          });
```

### Siehe auch

* class [DocumentFontsSubsystem](../)
* namensraum [Aspose.Note.Fonts](../../documentfontssubsystem/)
* Montage [Aspose.Note](../../../)


