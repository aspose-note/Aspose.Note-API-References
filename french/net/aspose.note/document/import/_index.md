---
title: Document.Import
second_title: Référence de l'API Aspose.Note pour .NET
description: Document méthode. Importe un ensemble de pages à partir du document PDF fourni.
type: docs
weight: 110
url: /fr/net/aspose.note/document/import/
---
## Import(Stream, PdfImportOptions, MergeOptions) {#import}

Importe un ensemble de pages à partir du document PDF fourni.

```csharp
public Document Import(Stream stream, PdfImportOptions importOptions = null, 
    MergeOptions mergeOptions = null)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| stream | Stream | Un flux avec un document PDF. |
| importOptions | PdfImportOptions | Spécifie les options d'importation de pages à partir d'un document PDF. |
| mergeOptions | MergeOptions | Spécifie les options de fusion des pages fournies. |

### Return_Value

Renvoie la référence au document.

### Voir également

* class [PdfImportOptions](../../../aspose.note.importing/pdfimportoptions/)
* class [MergeOptions](../../mergeoptions/)
* class [Document](../)
* espace de noms [Aspose.Note](../../document/)
* Assemblée [Aspose.Note](../../../)

---

## Import(string, PdfImportOptions, MergeOptions) {#import_1}

Importe un ensemble de pages à partir du document PDF fourni.

```csharp
public Document Import(string file, PdfImportOptions importOptions = null, 
    MergeOptions mergeOptions = null)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| file | String | Un fichier avec document PDF. |
| importOptions | PdfImportOptions | Spécifie les options d'importation de pages à partir d'un document PDF. |
| mergeOptions | MergeOptions | Spécifie les options de fusion des pages fournies. |

### Return_Value

Renvoie la référence au document.

### Exemples

Montre comment importer toutes les pages d'un ensemble de documents PDF page par page.

```csharp
string dataDir = RunExamples.GetDataDir_Import();

var d = new Document();

d.Import(Path.Combine(dataDir, "sampleText.pdf"))
 .Import(Path.Combine(dataDir, "sampleImage.pdf"))
 .Import(Path.Combine(dataDir, "sampleTable.pdf"));

d.Save(Path.Combine(dataDir, "sample_SimpleMerge.one"));
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

* class [PdfImportOptions](../../../aspose.note.importing/pdfimportoptions/)
* class [MergeOptions](../../mergeoptions/)
* class [Document](../)
* espace de noms [Aspose.Note](../../document/)
* Assemblée [Aspose.Note](../../../)


