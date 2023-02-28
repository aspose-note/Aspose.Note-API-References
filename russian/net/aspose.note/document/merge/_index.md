---
title: Document.Merge
second_title: Справочник по API Aspose.Note для .NET
description: Document метод. Объединяет набор страниц в документ.
type: docs
weight: 120
url: /ru/net/aspose.note/document/merge/
---
## Document.Merge method

Объединяет набор страниц в документ.

```csharp
public Document Merge(IEnumerable<Page> pages, MergeOptions mergeOptions = null)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| pages | IEnumerable`1 | Набор страниц. |
| mergeOptions | MergeOptions | Указывает параметры объединения предоставленных страниц. |

### Возвращаемое значение

Возвращает ссылку на документ.

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

* class [Page](../../page/)
* class [MergeOptions](../../mergeoptions/)
* class [Document](../)
* пространство имен [Aspose.Note](../../document/)
* сборка [Aspose.Note](../../../)


