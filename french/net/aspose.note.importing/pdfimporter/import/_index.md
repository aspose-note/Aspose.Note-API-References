---
title: PdfImporter.Import
second_title: Référence de l'API Aspose.Note pour .NET
description: PdfImporter méthode. Importe le contenu dun document PDF à partir dun flux fourni.
type: docs
weight: 10
url: /fr/net/aspose.note.importing/pdfimporter/import/
---
## Import(Stream, PdfImportOptions) {#import}

Importe le contenu d'un document PDF à partir d'un flux fourni.

```csharp
public static List<Page> Import(Stream stream, PdfImportOptions options = null)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| stream | Stream | Le flux. |
| options | PdfImportOptions | Les options. |

### Return_Value

Le[`PdfImporter`](../) .

### Voir également

* class [Page](../../../aspose.note/page/)
* class [PdfImportOptions](../../pdfimportoptions/)
* class [PdfImporter](../)
* espace de noms [Aspose.Note.Importing](../../pdfimporter/)
* Assemblée [Aspose.Note](../../../)

---

## Import(string, PdfImportOptions) {#import_1}

Importe le contenu d'un document PDF à partir d'un fichier spécifié.

```csharp
public static List<Page> Import(string file, PdfImportOptions options = null)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| file | String | Le fichier PDF. |
| options | PdfImportOptions | Les options. |

### Return_Value

Le[`PdfImporter`](../) .

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

* class [Page](../../../aspose.note/page/)
* class [PdfImportOptions](../../pdfimportoptions/)
* class [PdfImporter](../)
* espace de noms [Aspose.Note.Importing](../../pdfimporter/)
* Assemblée [Aspose.Note](../../../)


