---
title: DocumentFontsSubsystem.UsingDefaultFont
second_title: Aspose.Note für .NET-API-Referenz
description: DocumentFontsSubsystem methode. Erstellt eine neue DocumentFontsSubsystemInstanz unter Verwendung des angegebenen Standardschriftartnamens.
type: docs
weight: 30
url: /de/net/aspose.note.fonts/documentfontssubsystem/usingdefaultfont/
---
## DocumentFontsSubsystem.UsingDefaultFont method

Erstellt eine neue DocumentFontsSubsystem-Instanz unter Verwendung des angegebenen Standardschriftartnamens.

```csharp
public static DocumentFontsSubsystem UsingDefaultFont(string defaultFontName, 
    Dictionary<string, string> fontsSubstitutions = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| defaultFontName | String | Der Name der Standardschriftart. |
| fontsSubstitutions | Dictionary`2 | Die Schriftersetzungen. |

### Rückgabewert

Die[`DocumentFontsSubsystem`](../) .

### Beispiele

Zeigt, wie ein Dokument im PDF-Format mit einer angegebenen Standardschriftart gespeichert wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laden Sie das Dokument in Aspose.Note.
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// Dokument als PDF speichern
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontName_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions() 
                      {
                          FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFont("Times New Roman")
                      });
```

### Siehe auch

* class [DocumentFontsSubsystem](../)
* namensraum [Aspose.Note.Fonts](../../documentfontssubsystem/)
* Montage [Aspose.Note](../../../)


