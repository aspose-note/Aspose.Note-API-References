---
title: PageSettings.A4NoHeightLimit
second_title: Aspose.Note für .NET-API-Referenz
description: PageSettings eigendom. Ruft Einstellungen für die Seite im A4Format mit unbegrenzter Höhe ab.
type: docs
weight: 20
url: /de/net/aspose.note.saving/pagesettings/a4noheightlimit/
---
## PageSettings.A4NoHeightLimit property

Ruft Einstellungen für die Seite im A4-Format mit unbegrenzter Höhe ab.

```csharp
public static PageSettings A4NoHeightLimit { get; }
```

### Beispiele

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

* class [PageSettings](../)
* namensraum [Aspose.Note.Saving](../../pagesettings/)
* Montage [Aspose.Note](../../../)


