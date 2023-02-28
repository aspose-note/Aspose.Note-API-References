---
title: Class MergeOptions
second_title: Référence de l'API Aspose.Note pour .NET
description: Aspose.Note.MergeOptions classe. Les options de fusion dune collection de pages.
type: docs
weight: 340
url: /fr/net/aspose.note/mergeoptions/
---
## MergeOptions class

Les options de fusion d'une collection de pages.

```csharp
public class MergeOptions
```

## Constructeurs

| Nom | La description |
| --- | --- |
| [MergeOptions](mergeoptions/)() | Default_Constructor |

## Propriétés

| Nom | La description |
| --- | --- |
| [ImportAsSinglePage](../../aspose.note/mergeoptions/importassinglepage/) { get; set; } | Obtient ou définit une valeur indiquant s'il faut importer les pages fournies en tant que page unique. |
| [InsertAsChild](../../aspose.note/mergeoptions/insertaschild/) { get; set; } | Obtient ou définit une valeur indiquant si les pages insérées doivent être ajoutées en tant qu'enfants de la page précédente. |
| [InsertAt](../../aspose.note/mergeoptions/insertat/) { get; set; } | Obtient ou définit la position où les pages importées seront insérées. |
| [PageSpacing](../../aspose.note/mergeoptions/pagespacing/) { get; set; } | Obtient ou définit l'espacement entre les pages lors de l'importation en tant que page unique. |

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

Montre comment importer toutes les pages d'un ensemble de documents PDF tout en insérant des pages de chaque document PDF en tant qu'enfants d'une page OneNote de niveau supérieur.

```csharp
string dataDir = RunExamples.GetDataDir_Import();

var d = new Document();

foreach (var file in new[] { "sampleText.pdf", "sampleImage.pdf", "sampleTable.pdf" })
{
    d.AppendChildLast(new Page()).Title = new Title() { TitleText = new RichText() { ParagraphStyle = ParagraphStyle.Default }.Append(file) };
    d.Import(Path.Combine(dataDir, file), new PdfImportOptions(), new MergeOptions() { InsertAt = int.MaxValue, InsertAsChild = true });
}

d.Save(Path.Combine(dataDir, "sample_StructuredMerge.one"));
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

* espace de noms [Aspose.Note](../../aspose.note/)
* Assemblée [Aspose.Note](../../)


