---
title: Page.PageContentRevisionSummary
second_title: Aspose.Note voor .NET API-referentie
description: Page eigendom. Haalt of stelt het revisieoverzicht voor de pagina en de onderliggende knooppunten in.
type: docs
weight: 90
url: /nl/net/aspose.note/page/pagecontentrevisionsummary/
---
## Page.PageContentRevisionSummary property

Haalt of stelt het revisieoverzicht voor de pagina en de onderliggende knooppunten in.

```csharp
public RevisionSummary PageContentRevisionSummary { get; set; }
```

### Voorbeelden

Laat zien hoe u de meta-informatie van de pagina kunt bewerken.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Pages();

// Laad een OneNote-document en krijg het eerste kind           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

// Samenvatting inhoudsrevisie voor deze pagina lezen
var pageRevisionInfo = page.PageContentRevisionSummary;

Console.WriteLine(string.Format(
    "Author:\t{0}\nModified:\t{1}",
    pageRevisionInfo.AuthorMostRecent,
    pageRevisionInfo.LastModifiedTime.ToString("dd.MM.yyyy HH:mm:ss")));

// Werk de samenvatting van de paginarevisie bij voor deze pagina
pageRevisionInfo.AuthorMostRecent = "New Author";
pageRevisionInfo.LastModifiedTime = DateTime.Now;

document.Save(dataDir + "WorkingWithPageRevisions_out.one");
```

Laat zien hoe u kunt controleren of een pagina een conflictpagina is (dwz dat deze wijzigingen bevat die OneNote niet automatisch kan samenvoegen).

```csharp
string dataDir = RunExamples.GetDataDir_Pages();

// Laad OneNote-document
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

    // Standaard worden conflictpagina's gewoon overgeslagen bij het opslaan.
    // Als u het als niet-conflict markeert, wordt het zoals gebruikelijk in de geschiedenis opgeslagen.
    if (historyPage.IsConflictPage)
        historyPage.IsConflictPage = false;
}

doc.Save(dataDir + "ConflictPageManipulation_out.one", SaveFormat.One);
```

### Zie ook

* class [RevisionSummary](../../revisionsummary/)
* class [Page](../)
* naamruimte [Aspose.Note](../../page/)
* montage [Aspose.Note](../../../)


