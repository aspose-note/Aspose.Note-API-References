---
title: PageSettings.Letter
second_title: Aspose.Note für .NET-API-Referenz
description: PageSettings eigendom. Ruft Einstellungen für die Seite im LetterFormat ab.
type: docs
weight: 30
url: /de/net/aspose.note.saving/pagesettings/letter/
---
## PageSettings.Letter property

Ruft Einstellungen für die Seite im Letter-Format ab.

```csharp
public static PageSettings Letter { get; }
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

### Siehe auch

* class [PageSettings](../)
* namensraum [Aspose.Note.Saving](../../pagesettings/)
* Montage [Aspose.Note](../../../)


