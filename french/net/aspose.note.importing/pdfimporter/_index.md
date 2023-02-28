---
title: Class PdfImporter
second_title: Référence de l'API Aspose.Note pour .NET
description: Aspose.Note.Importing.PdfImporter classe. La classe fournissant lapi pour importer le contenu de documents au format PDF. Lapi permet dimporter à partir dun document PDF situé soit dans un fichier soit dans un flux en utilisant les options spécifiées. Les options dimportation sont passées en utilisantPdfImportOptions .
type: docs
weight: 270
url: /fr/net/aspose.note.importing/pdfimporter/
---
## PdfImporter class

La classe fournissant l'api pour importer le contenu de documents au format PDF. L'api permet d'importer à partir d'un document PDF situé soit dans un fichier, soit dans un flux en utilisant les options spécifiées. Les options d'importation sont passées en utilisant[`PdfImportOptions`](../pdfimportoptions/) .

```csharp
public static class PdfImporter
```

## Méthodes

| Nom | La description |
| --- | --- |
| static [Import](../../aspose.note.importing/pdfimporter/import/#import)(Stream, PdfImportOptions) | Importe le contenu d'un document PDF à partir d'un flux fourni. |
| static [Import](../../aspose.note.importing/pdfimporter/import/#import_1)(string, PdfImportOptions) | Importe le contenu d'un document PDF à partir d'un fichier spécifié. |

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

* espace de noms [Aspose.Note.Importing](../../aspose.note.importing/)
* Assemblée [Aspose.Note](../../)


