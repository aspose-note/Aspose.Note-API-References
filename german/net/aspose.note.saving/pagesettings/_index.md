---
title: Class PageSettings
second_title: Aspose.Note für .NET-API-Referenz
description: Aspose.Note.Saving.PageSettings klas. Repräsentiert die Layouteinstellungen für eine Seite.
type: docs
weight: 820
url: /de/net/aspose.note.saving/pagesettings/
---
## PageSettings class

Repräsentiert die Layouteinstellungen für eine Seite.

```csharp
public class PageSettings
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| static [A4](../../aspose.note.saving/pagesettings/a4/) { get; } | Ruft Einstellungen für die Seite im A4-Format ab. |
| static [A4NoHeightLimit](../../aspose.note.saving/pagesettings/a4noheightlimit/) { get; } | Ruft Einstellungen für die Seite im A4-Format mit unbegrenzter Höhe ab. |
| static [Letter](../../aspose.note.saving/pagesettings/letter/) { get; } | Ruft Einstellungen für die Seite im Letter-Format ab. |
| static [LetterNoHeightLimit](../../aspose.note.saving/pagesettings/letternoheightlimit/) { get; } | Ruft Einstellungen für die Seite im Letter-Format mit unbegrenzter Höhe ab. |

### Beispiele

Zeigt, wie ein Dokument im PDF-Format mit dem Seitenlayout "Letter" gespeichert wird.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laden Sie das Dokument in Aspose.Note.
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingLetterPageSettings.pdf");

// Speichern Sie das Dokument.
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.Letter });
```

Zeigt, wie Sie ein Dokument im Pdf-Format mit A4-Seitenlayout ohne Höhenbegrenzung speichern.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Laden Sie das Dokument in Aspose.Note.
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingA4PageSettingsWithoutHeightLimit.pdf");

// Speichern Sie das Dokument.
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.A4NoHeightLimit });
```

### Siehe auch

* namensraum [Aspose.Note.Saving](../../aspose.note.saving/)
* Montage [Aspose.Note](../../)


