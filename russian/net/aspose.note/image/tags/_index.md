---
title: Image.Tags
second_title: Справочник по API Aspose.Note для .NET
description: Image свойство. Получает список всех тегов абзаца.
type: docs
weight: 160
url: /ru/net/aspose.note/image/tags/
---
## Image.Tags property

Получает список всех тегов абзаца.

```csharp
public List<ITag> Tags { get; }
```

### Примеры

Показывает, как добавить новое изображение с тегом.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_Tags();

// Создаем объект класса Document
Document doc = new Document();

// Инициализировать объект класса Page
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Инициализировать объект класса Outline
Outline outline = new Outline(doc);

// Инициализировать объект класса OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

// Загружаем изображение
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "icon.jpg");

// Вставляем изображение в узел документа
outlineElem.AppendChildLast(image);
image.Tags.Add(NoteTag.CreateYellowStar());

// Добавляем узел элемента контура
outline.AppendChildLast(outlineElem);

// Добавляем узел контура
page.AppendChildLast(outline);

// Добавляем узел страницы
doc.AppendChildLast(page);

// Сохранить документ OneNote
dataDir = dataDir + "AddImageNodeWithTag_out.one";
doc.Save(dataDir);
```

### Смотрите также

* interface [ITag](../../itag/)
* class [Image](../)
* пространство имен [Aspose.Note](../../image/)
* сборка [Aspose.Note](../../../)


