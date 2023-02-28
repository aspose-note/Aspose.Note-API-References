---
title: PdfSaveOptions.PageSettings
second_title: Aspose.Note für .NET-API-Referenz
description: PdfSaveOptions eigendom. Ruft die Seiteneinstellungen für jede Seite im Dokument ab oder legt sie fest. Standardmäßig abhängig von CurrentUICulture USKulturen haben LetterEinstellungen andere haben A4Einstellungen.
type: docs
weight: 40
url: /de/net/aspose.note.saving/pdfsaveoptions/pagesettings/
---
## PdfSaveOptions.PageSettings property

Ruft die Seiteneinstellungen für jede Seite im Dokument ab oder legt sie fest. Standardmäßig abhängig von CurrentUICulture, *US-Kulturen haben Letter-Einstellungen, andere haben A4-Einstellungen.

```csharp
public PageSettings PageSettings { get; set; }
```

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

* class [PageSettings](../../pagesettings/)
* class [PdfSaveOptions](../)
* namensraum [Aspose.Note.Saving](../../pdfsaveoptions/)
* Montage [Aspose.Note](../../../)


