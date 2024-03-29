---
title: Image.HorizontalOffset
second_title: Справочник по API Aspose.Note для .NET
description: Image свойство. Получает или задает смещение по горизонтали.
type: docs
weight: 100
url: /ru/net/aspose.note/image/horizontaloffset/
---
## Image.HorizontalOffset property

Получает или задает смещение по горизонтали.

```csharp
public float HorizontalOffset { get; set; }
```

### Примеры

Показывает, как добавить изображение из файла в документ с заданными пользователем свойствами.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_Images();

// Загружаем документ из потока.
Document doc = new Document(dataDir + "Aspose.one");

// Получить первую страницу документа.
Aspose.Note.Page page = doc.FirstChild;

// Загружаем изображение из файла.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // Измените размер изображения в соответствии с вашими потребностями (необязательно).
                              Width = 100,
                              Height = 100,

                              // Установить положение изображения на странице (необязательно).
                              HorizontalOffset = 100,
                              VerticalOffset = 400,

                              // Установить выравнивание изображения
                              Alignment = HorizontalAlignment.Right
                          };

// Добавляем изображение на страницу.
page.AppendChildLast(image);
```

### Смотрите также

* class [Image](../)
* пространство имен [Aspose.Note](../../image/)
* сборка [Aspose.Note](../../../)


