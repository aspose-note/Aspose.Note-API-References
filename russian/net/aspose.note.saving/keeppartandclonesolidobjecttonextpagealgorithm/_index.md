---
title: Class KeepPartAndCloneSolidObjectToNextPageAlgorithm
second_title: Справочник по API Aspose.Note для .NET
description: Aspose.Note.Saving.KeepPartAndCloneSolidObjectToNextPageAlgorithm сорт. Добавляет верхнюю часть объекта в нижнюю часть страницы и клонирует весь объект на следующую страницу если он не помещается на исходной странице.
type: docs
weight: 730
url: /ru/net/aspose.note.saving/keeppartandclonesolidobjecttonextpagealgorithm/
---
## KeepPartAndCloneSolidObjectToNextPageAlgorithm class

Добавляет верхнюю часть объекта в нижнюю часть страницы и клонирует весь объект на следующую страницу, если он не помещается на исходной странице.

```csharp
public class KeepPartAndCloneSolidObjectToNextPageAlgorithm : PageSplittingAlgorithm
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [KeepPartAndCloneSolidObjectToNextPageAlgorithm](keeppartandclonesolidobjecttonextpagealgorithm/#constructor)() | Инициализирует новый экземпляр`KeepPartAndCloneSolidObjectToNextPageAlgorithm` class, используя предел высоты клонированной части по умолчанию. |
| [KeepPartAndCloneSolidObjectToNextPageAlgorithm](keeppartandclonesolidobjecttonextpagealgorithm/#constructor_1)(float) | Инициализирует новый экземпляр`KeepPartAndCloneSolidObjectToNextPageAlgorithm` класс, используя определенный предел высоты клонированной части. |

## Характеристики

| Имя | Описание |
| --- | --- |
| [HeightLimitOfClonedPart](../../aspose.note.saving/keeppartandclonesolidobjecttonextpagealgorithm/heightlimitofclonedpart/) { get; } | Получает предел высоты клонированной детали. |

## Поля

| Имя | Описание |
| --- | --- |
| const [DefaultHeightLimitOfClonedPart](../../aspose.note.saving/keeppartandclonesolidobjecttonextpagealgorithm/defaultheightlimitofclonedpart/) | Максимальный размер клонируемой детали по умолчанию. |

### Примеры

Когда длинные страницы OneNote сохраняются в формате PDF, они разбиваются на страницы. В примере показано, как настроить логику разделения объектов, расположенных на разрывах страниц.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Загрузите документ в Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");

var pdfSaveOptions = new PdfSaveOptions();

pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(100);
// или
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(400);

dataDir = dataDir + "PageSplittUsingKeepPartAndCloneSolidObjectToNextPageAlgorithm_out.pdf";
doc.Save(dataDir);
```

Когда длинные страницы OneNote сохраняются в формате PDF, они разбиваются на страницы. В примере показано, как настроить логику разделения объектов, расположенных на разрывах страниц.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Загрузите документ в Aspose.Note.
Document doc = new Document(dataDir + "Aspose.one");
var pdfSaveOptions = new PdfSaveOptions();
pdfSaveOptions.PageSplittingAlgorithm = new AlwaysSplitObjectsAlgorithm();
// Или
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm();
// Или
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm();

float heightLimitOfClonedPart = 500;
pdfSaveOptions.PageSplittingAlgorithm = new KeepPartAndCloneSolidObjectToNextPageAlgorithm(heightLimitOfClonedPart);
// Или
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(heightLimitOfClonedPart);

pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(100);
// Или
pdfSaveOptions.PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(400);

dataDir = dataDir + "UsingKeepSOlidObjectsAlgorithm_out.pdf";
doc.Save(dataDir);
```

### Смотрите также

* class [PageSplittingAlgorithm](../pagesplittingalgorithm/)
* пространство имен [Aspose.Note.Saving](../../aspose.note.saving/)
* сборка [Aspose.Note](../../)


