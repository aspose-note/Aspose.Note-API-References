---
title: RevisionSummary.LastModifiedTime
second_title: Référence de l'API Aspose.Note pour .NET
description: RevisionSummary propriété. Obtient ou définit lheure de la dernière modification.
type: docs
weight: 30
url: /fr/net/aspose.note/revisionsummary/lastmodifiedtime/
---
## RevisionSummary.LastModifiedTime property

Obtient ou définit l'heure de la dernière modification.

```csharp
public DateTime LastModifiedTime { get; set; }
```

### Exemples

Montre comment modifier les méta-informations de la page.

```csharp
// Le chemin d'accès au répertoire des documents.
string dataDir = RunExamples.GetDataDir_Pages();

// Charger le document OneNote et obtenir le premier enfant           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

// Lecture du résumé de la révision du contenu pour cette page
var pageRevisionInfo = page.PageContentRevisionSummary;

Console.WriteLine(string.Format(
    "Author:\t{0}\nModified:\t{1}",
    pageRevisionInfo.AuthorMostRecent,
    pageRevisionInfo.LastModifiedTime.ToString("dd.MM.yyyy HH:mm:ss")));

// Mettre à jour le résumé de révision de la page pour cette page
pageRevisionInfo.AuthorMostRecent = "New Author";
pageRevisionInfo.LastModifiedTime = DateTime.Now;

document.Save(dataDir + "WorkingWithPageRevisions_out.one");
```

Montre comment vérifier si une page est une page en conflit (c'est-à-dire qu'elle contient des modifications que OneNote n'a pas pu fusionner automatiquement).

```csharp
string dataDir = RunExamples.GetDataDir_Pages();

// Charger le document OneNote
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

    // Par défaut, les pages en conflit sont simplement ignorées lors de l'enregistrement.
    // Si vous le marquez comme non conflictuel, il sera enregistré comme d'habitude dans l'historique.
    if (historyPage.IsConflictPage)
        historyPage.IsConflictPage = false;
}

doc.Save(dataDir + "ConflictPageManipulation_out.one", SaveFormat.One);
```

### Voir également

* class [RevisionSummary](../)
* espace de noms [Aspose.Note](../../revisionsummary/)
* Assemblée [Aspose.Note](../../../)


