---
title: Page.PageContentRevisionSummary
second_title: Aspose.Note für .NET-API-Referenz
description: Page eigendom. Ruft die Überarbeitungszusammenfassung für die Seite und ihre untergeordneten Knoten ab oder legt sie fest.
type: docs
weight: 90
url: /de/net/aspose.note/page/pagecontentrevisionsummary/
---
## Page.PageContentRevisionSummary property

Ruft die Überarbeitungszusammenfassung für die Seite und ihre untergeordneten Knoten ab oder legt sie fest.

```csharp
public RevisionSummary PageContentRevisionSummary { get; set; }
```

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

* class [RevisionSummary](../../revisionsummary/)
* class [Page](../)
* namensraum [Aspose.Note](../../page/)
* Montage [Aspose.Note](../../../)


