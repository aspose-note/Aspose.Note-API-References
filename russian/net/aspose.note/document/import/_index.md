---
title: Document.Import
second_title: Справочник по API Aspose.Note для .NET
description: Document метод. Импортирует набор страниц из предоставленного документа PDF.
type: docs
weight: 110
url: /ru/net/aspose.note/document/import/
---
## Import(Stream, PdfImportOptions, MergeOptions) {#import}

Импортирует набор страниц из предоставленного документа PDF.

```csharp
public Document Import(Stream stream, PdfImportOptions importOptions = null, 
    MergeOptions mergeOptions = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | Stream | Поток с PDF-документом. |
| importOptions | PdfImportOptions | Указывает параметры импорта страниц из документа PDF. |
| mergeOptions | MergeOptions | Указывает параметры объединения предоставленных страниц. |

### Возвращаемое значение

Возвращает ссылку на документ.

### Смотрите также

* class [PdfImportOptions](../../../aspose.note.importing/pdfimportoptions/)
* class [MergeOptions](../../mergeoptions/)
* class [Document](../)
* пространство имен [Aspose.Note](../../document/)
* сборка [Aspose.Note](../../../)

---

## Import(string, PdfImportOptions, MergeOptions) {#import_1}

Импортирует набор страниц из предоставленного документа PDF.

```csharp
public Document Import(string file, PdfImportOptions importOptions = null, 
    MergeOptions mergeOptions = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| file | String | Файл с документом PDF. |
| importOptions | PdfImportOptions | Указывает параметры импорта страниц из документа PDF. |
| mergeOptions | MergeOptions | Указывает параметры объединения предоставленных страниц. |

### Возвращаемое значение

Возвращает ссылку на документ.

### Примеры

Показывает, как импортировать все страницы из набора PDF-документов постранично.

```csharp
string dataDir = RunExamples.GetDataDir_Import();

var d = new Document();

d.Import(Path.Combine(dataDir, "sampleText.pdf"))
 .Import(Path.Combine(dataDir, "sampleImage.pdf"))
 .Import(Path.Combine(dataDir, "sampleTable.pdf"));

d.Save(Path.Combine(dataDir, "sample_SimpleMerge.one"));
```

Показывает, как импортировать все страницы из набора документов PDF при вставке страниц из каждого документа PDF в качестве дочерних элементов страницы OneNote верхнего уровня.

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

Показывает, как импортировать все содержимое из набора документов PDF при объединении страниц из каждого документа PDF в одну страницу OneNote.

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

### Смотрите также

* class [PdfImportOptions](../../../aspose.note.importing/pdfimportoptions/)
* class [MergeOptions](../../mergeoptions/)
* class [Document](../)
* пространство имен [Aspose.Note](../../document/)
* сборка [Aspose.Note](../../../)


