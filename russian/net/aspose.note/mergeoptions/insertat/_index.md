---
title: MergeOptions.InsertAt
second_title: Справочник по API Aspose.Note для .NET
description: MergeOptions свойство. Получает или задает позицию в которую будут вставлены импортированные страницы.
type: docs
weight: 40
url: /ru/net/aspose.note/mergeoptions/insertat/
---
## MergeOptions.InsertAt property

Получает или задает позицию, в которую будут вставлены импортированные страницы.

```csharp
public int InsertAt { get; set; }
```

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentOutOfRangeException |  |

### Примечания

Если значение больше количества страниц в целевом документе, импортированные страницы добавляются в конец документа.

### Примеры

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

### Смотрите также

* class [MergeOptions](../)
* пространство имен [Aspose.Note](../../mergeoptions/)
* сборка [Aspose.Note](../../../)


