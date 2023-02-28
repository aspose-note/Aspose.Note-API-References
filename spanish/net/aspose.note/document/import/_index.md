---
title: Document.Import
second_title: Aspose.Note para la referencia de la API de .NET
description: Document método. Importa un conjunto de páginas del documento PDF proporcionado.
type: docs
weight: 110
url: /es/net/aspose.note/document/import/
---
## Import(Stream, PdfImportOptions, MergeOptions) {#import}

Importa un conjunto de páginas del documento PDF proporcionado.

```csharp
public Document Import(Stream stream, PdfImportOptions importOptions = null, 
    MergeOptions mergeOptions = null)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| stream | Stream | Un stream con documento PDF. |
| importOptions | PdfImportOptions | Especifica las opciones sobre cómo importar páginas desde un documento PDF. |
| mergeOptions | MergeOptions | Especifica las opciones sobre cómo combinar las páginas proporcionadas. |

### Valor_devuelto

Devuelve la referencia al documento.

### Ver también

* class [PdfImportOptions](../../../aspose.note.importing/pdfimportoptions/)
* class [MergeOptions](../../mergeoptions/)
* class [Document](../)
* espacio de nombres [Aspose.Note](../../document/)
* asamblea [Aspose.Note](../../../)

---

## Import(string, PdfImportOptions, MergeOptions) {#import_1}

Importa un conjunto de páginas del documento PDF proporcionado.

```csharp
public Document Import(string file, PdfImportOptions importOptions = null, 
    MergeOptions mergeOptions = null)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| file | String | Un archivo con documento PDF. |
| importOptions | PdfImportOptions | Especifica las opciones sobre cómo importar páginas desde un documento PDF. |
| mergeOptions | MergeOptions | Especifica las opciones sobre cómo combinar las páginas proporcionadas. |

### Valor_devuelto

Devuelve la referencia al documento.

### Ejemplos

Muestra cómo importar todas las páginas de un conjunto de documentos PDF página por página.

```csharp
string dataDir = RunExamples.GetDataDir_Import();

var d = new Document();

d.Import(Path.Combine(dataDir, "sampleText.pdf"))
 .Import(Path.Combine(dataDir, "sampleImage.pdf"))
 .Import(Path.Combine(dataDir, "sampleTable.pdf"));

d.Save(Path.Combine(dataDir, "sample_SimpleMerge.one"));
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

* class [PdfImportOptions](../../../aspose.note.importing/pdfimportoptions/)
* class [MergeOptions](../../mergeoptions/)
* class [Document](../)
* espacio de nombres [Aspose.Note](../../document/)
* asamblea [Aspose.Note](../../../)


