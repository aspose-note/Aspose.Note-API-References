---
title: DocumentFontsSubsystem
second_title: Aspose.Note für .NET-API-Referenz
description: Einfache Implementierung von Aspose.Note.Fonts.FontsSubsystem. Ruft abFontFamily Objekt von OS.
type: docs
weight: 100
url: /de/net/aspose.note.fonts/documentfontssubsystem/
---
## DocumentFontsSubsystem class

Einfache Implementierung von Aspose.Note.Fonts.FontsSubsystem. Ruft abFontFamily Objekt von OS.

```csharp
public class DocumentFontsSubsystem : FontsSubsystem
```

## Konstrukteure

| Name | Beschreibung |
| --- | --- |
| [DocumentFontsSubsystem](documentfontssubsystem#constructor)(Dictionary&lt;string, string&gt;) | Initialisiert eine neue Instanz von[`DocumentFontsSubsystem`](../documentfontssubsystem) Klasse. |
| [DocumentFontsSubsystem](documentfontssubsystem#constructor_1)(Stream, Dictionary&lt;string, string&gt;) | Initialisiert eine neue Instanz von[`DocumentFontsSubsystem`](../documentfontssubsystem) Klasse. |
| [DocumentFontsSubsystem](documentfontssubsystem#constructor_2)(string, Dictionary&lt;string, string&gt;) | Initialisiert eine neue Instanz von[`DocumentFontsSubsystem`](../documentfontssubsystem) Klasse. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| static [Default](../../aspose.note.fonts/documentfontssubsystem/default) { get; set; } | Ruft die statische Standardinstanz ab oder legt sie fest. |
| [DefaultFont](../../aspose.note.fonts/fontssubsystem/defaultfont) { get; } | Ruft die Standardschriftart ab oder legt sie fest. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| static [UsingDefaultFont](../../aspose.note.fonts/documentfontssubsystem/usingdefaultfont)(string, Dictionary&lt;string, string&gt;) | Erstellt eine neue DocumentFontsSubsystem-Instanz unter Verwendung des angegebenen Standardschriftartnamens. |
| static [UsingDefaultFontFromFile](../../aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromfile)(string, Dictionary&lt;string, string&gt;) | Erstellt eine neue DocumentFontsSubsystem-Instanz unter Verwendung einer Schriftart aus der angegebenen Datei als Standard. |
| static [UsingDefaultFontFromStream](../../aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromstream)(Stream, Dictionary&lt;string, string&gt;) | Erstellt eine neue DocumentFontsSubsystem-Instanz unter Verwendung einer Schriftart aus dem angegebenen Stream als Standard. |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont)(Stream) | Schriftart hinzufügen. |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont)(string) | Schriftart hinzufügen. |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont)(Stream, string) | Schriftart hinzufügen. |
| [AddFontSubstitution](../../aspose.note.fonts/fontssubsystem/addfontsubstitution)(string, string) | Fügt Schriftersatz hinzu. |
| virtual [GetFontFamily](../../aspose.note.fonts/fontssubsystem/getfontfamily)(string) | Ruft die Schriftfamilie ab. |
| [LoadFontsFromFolder](../../aspose.note.fonts/fontssubsystem/loadfontsfromfolder)(string) | Lädt alle TrueType-Schriftarten aus dem angegebenen Ordner in die interne Sammlung. |

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

* class [FontsSubsystem](../fontssubsystem)
* namensraum [Aspose.Note.Fonts](../../aspose.note.fonts)
* Montage [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
