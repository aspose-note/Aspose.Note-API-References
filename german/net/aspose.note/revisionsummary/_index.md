---
title: Class RevisionSummary
second_title: Aspose.Note für .NET-API-Referenz
description: Aspose.Note.RevisionSummary klas. Stellt eine Zusammenfassung für die Revision des Knotens dar.
type: docs
weight: 520
url: /de/net/aspose.note/revisionsummary/
---
## RevisionSummary class

Stellt eine Zusammenfassung für die Revision des Knotens dar.

```csharp
public class RevisionSummary
```

## Konstrukteure

| Name | Beschreibung |
| --- | --- |
| [RevisionSummary](revisionsummary/)() | Default_Constructor |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AuthorMostRecent](../../aspose.note/revisionsummary/authormostrecent/) { get; set; } | Ruft den neuesten Autor ab oder legt ihn fest. |
| [LastModifiedTime](../../aspose.note/revisionsummary/lastmodifiedtime/) { get; set; } | Ruft die letzte Änderungszeit ab oder setzt sie. |

### Beispiele

Zeigt, wie die Metainformationen der Seite bearbeitet werden.

```csharp
// Der Pfad zum Dokumentenverzeichnis.
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote-Dokument laden und erstes untergeordnetes Element abrufen           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

// Zusammenfassung der Inhaltsrevision für diese Seite lesen
var pageRevisionInfo = page.PageContentRevisionSummary;

Console.WriteLine(string.Format(
    "Author:\t{0}\nModified:\t{1}",
    pageRevisionInfo.AuthorMostRecent,
    pageRevisionInfo.LastModifiedTime.ToString("dd.MM.yyyy HH:mm:ss")));

// Zusammenfassung der Seitenrevision für diese Seite aktualisieren
pageRevisionInfo.AuthorMostRecent = "New Author";
pageRevisionInfo.LastModifiedTime = DateTime.Now;

document.Save(dataDir + "WorkingWithPageRevisions_out.one");
```

Zeigt, wie überprüft wird, ob es sich bei einer Seite um eine Konfliktseite handelt (d. h. sie enthält Änderungen, die OneNote nicht automatisch zusammenführen konnte).

```csharp
string dataDir = RunExamples.GetDataDir_Pages();

// OneNote-Dokument laden
Document doc = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

var history = doc.GetPageHistory(doc.FirstChild);
for (int i = 0; i < history.Count; i++)
{
    var historyPage = history[i];
    Console.Write("    {0}. Author: {1}, {2:dd.MM.yyyy hh.mm.ss}",
                    i,
                    historyPage.PageContentRevisionSummary.AuthorMostRecent,
                    historyPage.PageContentRevisionSummary.LastModifiedTime);
    Console.WriteLine(historyPage.IsConflictPage ? ", IsConflict: true" : string.Empty);

    // Standardmäßig werden Konfliktseiten beim Speichern einfach übersprungen.
    // Wenn es als Nicht-Konflikt markiert wird, wird es wie gewohnt im Verlauf gespeichert.
    if (historyPage.IsConflictPage)
        historyPage.IsConflictPage = false;
}

doc.Save(dataDir + "ConflictPageManipulation_out.one", SaveFormat.One);
```

### Siehe auch

* namensraum [Aspose.Note](../../aspose.note/)
* Montage [Aspose.Note](../../)


