---
title: Document.AutomaticLayoutChangesDetectionEnabled
second_title: Справочник по API Aspose.Note для .NET
description: Document свойство. Получает или задает значение указывающее выполняет ли Aspose.Note автоматическое обнаружение изменений макета. Значение по умолчаниюистинный .
type: docs
weight: 20
url: /ru/net/aspose.note/document/automaticlayoutchangesdetectionenabled/
---
## Document.AutomaticLayoutChangesDetectionEnabled property

Получает или задает значение, указывающее, выполняет ли Aspose.Note автоматическое обнаружение изменений макета. Значение по умолчанию:`истинный` .

```csharp
public bool AutomaticLayoutChangesDetectionEnabled { get; set; }
```

### Примеры

Показывает, как сохранить документ в различных форматах.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// Инициализировать новый документ
Document doc = new Document() { AutomaticLayoutChangesDetectionEnabled = false };

// Инициализировать новую страницу
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Стиль по умолчанию для всего текста в документе.
ParagraphStyle textStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };
page.Title = new Title(doc)
             {
                 TitleText = new RichText(doc) { Text = "Title text.", ParagraphStyle = textStyle },
                 TitleDate = new RichText(doc) { Text = new DateTime(2011, 11, 11).ToString("D", CultureInfo.InvariantCulture), ParagraphStyle = textStyle },
                 TitleTime = new RichText(doc) { Text = "12:34", ParagraphStyle = textStyle }
             };

// Добавляем узел страницы
doc.AppendChildLast(page);

// Сохранение документа OneNote в разных форматах, установка размера шрифта текста и обнаружение изменений макета вручную.
doc.Save(dataDir + "ConsequentExportOperations_out.html");            
doc.Save(dataDir + "ConsequentExportOperations_out.pdf");            
doc.Save(dataDir + "ConsequentExportOperations_out.jpg");            
textStyle.FontSize = 11;           
doc.DetectLayoutChanges();            
doc.Save(dataDir + "ConsequentExportOperations_out.bmp");
```

### Смотрите также

* class [Document](../)
* пространство имен [Aspose.Note](../../document/)
* сборка [Aspose.Note](../../../)


