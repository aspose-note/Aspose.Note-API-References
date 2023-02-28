---
title: Class MergeOptions
second_title: Aspose.Note para la referencia de la API de .NET
description: Aspose.Note.MergeOptions clase. Las opciones para fusionar una colección de páginas.
type: docs
weight: 340
url: /es/net/aspose.note/mergeoptions/
---
## MergeOptions class

Las opciones para fusionar una colección de páginas.

```csharp
public class MergeOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [MergeOptions](mergeoptions/)() | Constructor predeterminado |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [ImportAsSinglePage](../../aspose.note/mergeoptions/importassinglepage/) { get; set; } | Obtiene o establece un valor que indica si se importan las páginas proporcionadas como una sola página. |
| [InsertAsChild](../../aspose.note/mergeoptions/insertaschild/) { get; set; } | Obtiene o establece un valor que indica si las páginas insertadas se deben agregar como elementos secundarios de la página anterior. |
| [InsertAt](../../aspose.note/mergeoptions/insertat/) { get; set; } | Obtiene o establece la posición donde se insertarán las páginas importadas. |
| [PageSpacing](../../aspose.note/mergeoptions/pagespacing/) { get; set; } | Obtiene o establece el espaciado entre páginas cuando se importa como una sola página. |

### Ejemplos

Muestra cómo importar todas las páginas de un documento PDF agrupando cada 5 páginas en una sola página de OneNote.

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

Muestra cómo importar todas las páginas de un conjunto de documentos PDF mientras inserta páginas de cada documento PDF como elementos secundarios de una página de OneNote de nivel superior.

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

Muestra cómo importar todo el contenido de un conjunto de documentos PDF mientras combina páginas de cada documento PDF en una sola página de OneNote.

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

### Ver también

* espacio de nombres [Aspose.Note](../../aspose.note/)
* asamblea [Aspose.Note](../../)


