---
title: Document.GetPageHistory
second_title: Aspose.Note voor .NET API-referentie
description: Document methode. Krijgt dePageHistory die de volledige geschiedenis bevat voor elke pagina die in een document wordt gepresenteerd de vroegste op index 0. De huidige paginarevisie is toegankelijk alsCurrent en afzonderlijk opgenomen in de verzameling historische versies.
type: docs
weight: 100
url: /nl/net/aspose.note/document/getpagehistory/
---
## Document.GetPageHistory method

Krijgt de[`PageHistory`](../../pagehistory/) die de volledige geschiedenis bevat voor elke pagina die in een document wordt gepresenteerd (de vroegste op index 0). De huidige paginarevisie is toegankelijk als[`Current`](../../pagehistory/current/) en afzonderlijk opgenomen in de verzameling historische versies.

```csharp
public PageHistory GetPageHistory(Page page)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| page | Page | De huidige revisie van een pagina. |

### Winstwaarde

De[`PageHistory`](../../pagehistory/) .

### Voorbeelden

Laat zien hoe u de vorige versie van een pagina kunt herstellen.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Pages();

// Laad een OneNote-document en krijg het eerste kind           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;           
Page previousPageVersion = document.GetPageHistory(page).Last();

document.RemoveChild(page);
document.AppendChildLast(previousPageVersion);

document.Save(dataDir + "RollBackRevisions_out.one");
```

Laat zien hoe u de geschiedenis van de pagina kunt bewerken.

```csharp
// Het pad naar de documentenmap.
string dataDir = RunExamples.GetDataDir_Pages();

// Laad een OneNote-document en krijg het eerste kind           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

var pageHistory = document.GetPageHistory(page);

pageHistory.RemoveRange(0, 1);

pageHistory[0] = new Page(document);
if (pageHistory.Count > 1)
{
    pageHistory[1].Title.TitleText.Text = "New Title";

    pageHistory.Add(new Page(document));

    pageHistory.Insert(1, new Page(document));

    document.Save(dataDir + "ModifyPageHistory_out.one");
}
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

* class [PageHistory](../../pagehistory/)
* class [Page](../../page/)
* class [Document](../)
* naamruimte [Aspose.Note](../../document/)
* montage [Aspose.Note](../../../)


