---
title: MergeOptions.ImportAsSinglePage
second_title: Référence de l'API Aspose.Note pour .NET
description: MergeOptions propriété. Obtient ou définit une valeur indiquant sil faut importer les pages fournies en tant que page unique.
type: docs
weight: 20
url: /fr/net/aspose.note/mergeoptions/importassinglepage/
---
## MergeOptions.ImportAsSinglePage property

Obtient ou définit une valeur indiquant s'il faut importer les pages fournies en tant que page unique.

```csharp
public bool ImportAsSinglePage { get; set; }
```

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

Montre comment importer tout le contenu d'un ensemble de documents PDF tout en fusionnant les pages de chaque document PDF en une seule page OneNote.

```csharp
string dataDir = RunExamples.GetDataDir_Import();

var d = new Document();

var importOptions = new PdfImportOptions();
var mergeOptions = new MergeOptions() { ImportAsSinglePage = true, PageSpacing = 100 };

d.Import(Path.Combine(dataDir, "sampleText.pdf"), importOptions, mergeOptions)
 .Import(Path.Combine(dataDir, "sampleImage.pdf"), importOptions, mergeOptions)
 .Import(Path.Combine(dataDir, "sampleTable.pdf"), importOptions, mergeOptions);

d.Save(Path.Combine(dataDir, "sample_SinglePageMerge.one"));
```

### Voir également

* class [MergeOptions](../)
* espace de noms [Aspose.Note](../../mergeoptions/)
* Assemblée [Aspose.Note](../../../)


