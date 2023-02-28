---
title: Class AlwaysSplitObjectsAlgorithm
second_title: Справочник по API Aspose.Note для .NET
description: Aspose.Note.Saving.AlwaysSplitObjectsAlgorithm сорт. Разбивает объект на несколько частей если он не помещается на исходной странице.
type: docs
weight: 550
url: /ru/net/aspose.note.saving/alwayssplitobjectsalgorithm/
---
## AlwaysSplitObjectsAlgorithm class

Разбивает объект на несколько частей, если он не помещается на исходной странице.

```csharp
public class AlwaysSplitObjectsAlgorithm : PageSplittingAlgorithm
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [AlwaysSplitObjectsAlgorithm](alwayssplitobjectsalgorithm/)() | Конструктор по умолчанию. |

### Примеры

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


