---
title: PrintOptions.PageSplittingAlgorithm
second_title: Справочник по API Aspose.Note для .NET
description: PrintOptions свойство. Получает или задает алгоритм используемый для разбиения страницы.
type: docs
weight: 30
url: /ru/net/aspose.note.saving/printoptions/pagesplittingalgorithm/
---
## PrintOptions.PageSplittingAlgorithm property

Получает или задает алгоритм, используемый для разбиения страницы.

```csharp
public PageSplittingAlgorithm PageSplittingAlgorithm { get; set; }
```

### Стоимость имущества

`PageSplittingAlgorithm` .

### Примеры

Показывает, как отправить документ на принтер, используя стандартный диалог Windows с заданными параметрами.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

var document = new Aspose.Note.Document(dataDir + "Aspose.one");

var printerSettings = new PrinterSettings() { FromPage = 0, ToPage = 10 };
printerSettings.DefaultPageSettings.Landscape = true;
printerSettings.DefaultPageSettings.Margins = new System.Drawing.Printing.Margins(50, 50, 150, 50);

document.Print(new PrintOptions()
               {
                   PrinterSettings = printerSettings,
                   Resolution = 1200,
                   PageSplittingAlgorithm = new KeepSolidObjectsAlgorithm(),
                   DocumentName = "Test.one"
               });
```

### Смотрите также

* class [PageSplittingAlgorithm](../../pagesplittingalgorithm/)
* class [PrintOptions](../)
* пространство имен [Aspose.Note.Saving](../../printoptions/)
* сборка [Aspose.Note](../../../)


