---
title: Class PdfImporter
second_title: Aspose.Note para la referencia de la API de .NET
description: Aspose.Note.Importing.PdfImporter clase. La clase que proporciona api para importar contenido de documentos en formato PDF. La api permite importar desde documentos PDF ubicados en un archivo o en una secuencia usando opciones específicas. Las opciones de importación se pasan usandoPdfImportOptions .
type: docs
weight: 270
url: /es/net/aspose.note.importing/pdfimporter/
---
## PdfImporter class

La clase que proporciona api para importar contenido de documentos en formato PDF. La api permite importar desde documentos PDF ubicados en un archivo o en una secuencia usando opciones específicas. Las opciones de importación se pasan usando[`PdfImportOptions`](../pdfimportoptions/) .

```csharp
public static class PdfImporter
```

## Métodos

| Nombre | Descripción |
| --- | --- |
| static [Import](../../aspose.note.importing/pdfimporter/import/#import)(Stream, PdfImportOptions) | Importa el contenido de un documento PDF desde un flujo proporcionado. |
| static [Import](../../aspose.note.importing/pdfimporter/import/#import_1)(string, PdfImportOptions) | Importa el contenido de un documento PDF desde un archivo especificado. |

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

### Ver también

* espacio de nombres [Aspose.Note.Importing](../../aspose.note.importing/)
* asamblea [Aspose.Note](../../)


