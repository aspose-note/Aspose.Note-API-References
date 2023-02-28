---
title: Page.IsConflictPage
second_title: Aspose.Note voor .NET API-referentie
description: Page eigendom. Haalt of stelt een waarde in die aangeeft of deze pagina een conflictpagina is.
type: docs
weight: 50
url: /nl/net/aspose.note/page/isconflictpage/
---
## Page.IsConflictPage property

Haalt of stelt een waarde in die aangeeft of deze pagina een conflictpagina is.

```csharp
public bool IsConflictPage { get; set; }
```

### Opmerkingen

De conflictpagina ontstaat wanneer twee gebruikers dezelfde inhoud proberen bij te werken. In dit geval worden de wijzigingen van de eerste gebruiker zoals gewoonlijk geschreven. Maar wijzigingen van een andere gebruiker kunnen niet worden samengevoegd. Er wordt dus gewoon een kopie van de pagina gemaakt en gemarkeerd als conflict.

In deze versie worden de conflicten opgelost ten gunste van de wijzigingen van de eerste gebruiker. Dus als het document conflicterende pagina's heeft, worden deze in de geschiedenis weergegeven, maar worden ze overgeslagen bij het opslaan. Het is mogelijk om deze vlag opnieuw in te stellen om deze pagina's op te slaan in de geschiedenis zoals gewoonlijk.

Gedetailleerd voorbeeld van manipuleren door conflictpagina is te vinden in de online documentatie.

### Voorbeelden

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

* class [Page](../)
* naamruimte [Aspose.Note](../../page/)
* montage [Aspose.Note](../../../)


