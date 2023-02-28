---
title: PrintOptions.DocumentName
second_title: Справочник по API Aspose.Note для .NET
description: PrintOptions свойство. Получает или задает имя документа для отображения например в диалоговом окне состояния печати или в очереди печати при печати документа.
type: docs
weight: 20
url: /ru/net/aspose.note.saving/printoptions/documentname/
---
## PrintOptions.DocumentName property

Получает или задает имя документа для отображения (например, в диалоговом окне состояния печати или в очереди печати) при печати документа.

```csharp
public string DocumentName { get; set; }
```

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

* class [PrintOptions](../)
* пространство имен [Aspose.Note.Saving](../../printoptions/)
* сборка [Aspose.Note](../../../)


