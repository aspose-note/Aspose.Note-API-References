---
title: PdfImporter.Import
second_title: Справочник по API Aspose.Note для .NET
description: PdfImporter метод. Импортирует содержимое документа PDF из предоставленного потока.
type: docs
weight: 10
url: /ru/net/aspose.note.importing/pdfimporter/import/
---
## Import(Stream, PdfImportOptions) {#import}

Импортирует содержимое документа PDF из предоставленного потока.

```csharp
public static List<Page> Import(Stream stream, PdfImportOptions options = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | Stream | Поток. |
| options | PdfImportOptions | Опции. |

### Возвращаемое значение

[`PdfImporter`](../) .

### Смотрите также

* class [Page](../../../aspose.note/page/)
* class [PdfImportOptions](../../pdfimportoptions/)
* class [PdfImporter](../)
* пространство имен [Aspose.Note.Importing](../../pdfimporter/)
* сборка [Aspose.Note](../../../)

---

## Import(string, PdfImportOptions) {#import_1}

Импортирует содержимое документа PDF из указанного файла.

```csharp
public static List<Page> Import(string file, PdfImportOptions options = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| file | String | PDF-файл. |
| options | PdfImportOptions | Опции. |

### Возвращаемое значение

[`PdfImporter`](../) .

### Примеры

Показывает, как импортировать все страницы из документа PDF, группирующего каждые 5 страниц, в одну страницу OneNote.

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

### Смотрите также

* class [Page](../../../aspose.note/page/)
* class [PdfImportOptions](../../pdfimportoptions/)
* class [PdfImporter](../)
* пространство имен [Aspose.Note.Importing](../../pdfimporter/)
* сборка [Aspose.Note](../../../)


