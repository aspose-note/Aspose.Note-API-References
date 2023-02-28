---
title: Class PrintOptions
second_title: Справочник по API Aspose.Note для .NET
description: Aspose.Note.Saving.PrintOptions сорт. Параметры используемые для печати документа.
type: docs
weight: 860
url: /ru/net/aspose.note.saving/printoptions/
---
## PrintOptions class

Параметры, используемые для печати документа.

```csharp
public class PrintOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [PrintOptions](printoptions/)() | Конструктор по умолчанию. |

## Характеристики

| Имя | Описание |
| --- | --- |
| [DocumentName](../../aspose.note.saving/printoptions/documentname/) { get; set; } | Получает или задает имя документа для отображения (например, в диалоговом окне состояния печати или в очереди печати) при печати документа. |
| [PageSplittingAlgorithm](../../aspose.note.saving/printoptions/pagesplittingalgorithm/) { get; set; } | Получает или задает алгоритм, используемый для разбиения страницы. |
| [PrinterSettings](../../aspose.note.saving/printoptions/printersettings/) { get; set; } | Получает или устанавливает параметры принтера. |
| [Resolution](../../aspose.note.saving/printoptions/resolution/) { get; set; } | Получает или задает разрешение сгенерированных изображений в точках на дюйм. |

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

* пространство имен [Aspose.Note.Saving](../../aspose.note.saving/)
* сборка [Aspose.Note](../../)


