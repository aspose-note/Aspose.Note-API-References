---
title: Document.Merge
second_title: Référence de l'API Aspose.Note pour .NET
description: Document méthode. Fusionne un ensemble de pages dans le document.
type: docs
weight: 120
url: /fr/net/aspose.note/document/merge/
---
## Document.Merge method

Fusionne un ensemble de pages dans le document.

```csharp
public Document Merge(IEnumerable<Page> pages, MergeOptions mergeOptions = null)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| pages | IEnumerable`1 | Un ensemble de pages. |
| mergeOptions | MergeOptions | Spécifie les options de fusion des pages fournies. |

### Return_Value

Renvoie la référence au document.

### Exemples

Montre comment importer toutes les pages d'un document PDF regroupant toutes les 5 pages sur une seule page OneNote.

```csharp
string dataDir = RunExamples.GetDataDir_Import();

var d = new Document();

var mergeOptions = new MergeOptions() { ImportAsSinglePage = true, PageSpacing = 100 };

IEnumerable<Page> pages = PdfImporter.Import(Path.Combine(dataDir, "SampleGrouping.pdf"));
while (pages.Any())
{
    d.Merge(pages.Take(5), mergeOptions);
    pages = pages.Skip(5);
}

d.Save(Path.Combine(dataDir, "sample_CustomMerge.one"));
```

### Voir également

* class [Page](../../page/)
* class [MergeOptions](../../mergeoptions/)
* class [Document](../)
* espace de noms [Aspose.Note](../../document/)
* Assemblée [Aspose.Note](../../../)


