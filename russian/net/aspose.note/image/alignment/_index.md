---
title: Image.Alignment
second_title: Справочник по API Aspose.Note для .NET
description: Image свойство. Получает или задает выравнивание.
type: docs
weight: 20
url: /ru/net/aspose.note/image/alignment/
---
## Image.Alignment property

Получает или задает выравнивание.

```csharp
public HorizontalAlignment Alignment { get; set; }
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

Показывает, как добавить изображение из потока в документ.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_Images();

// Создаем объект класса Document
Document doc = new Document();

// Инициализировать объект класса Page
Aspose.Note.Page page = new Aspose.Note.Page(doc);

Outline outline1 = new Outline(doc);
OutlineElement outlineElem1 = new OutlineElement(doc);

using (FileStream fs = File.OpenRead(dataDir + "image.jpg"))
{

    // Загружаем второе изображение, используя имя изображения, расширение и поток.
    Aspose.Note.Image image1 = new Aspose.Note.Image(doc, "Penguins.jpg", fs)
                                   {
                                       // Установить выравнивание изображения
                                       Alignment = HorizontalAlignment.Right
                                   };

    outlineElem1.AppendChildLast(image1);
}

outline1.AppendChildLast(outlineElem1);
page.AppendChildLast(outline1);

doc.AppendChildLast(page);

// Сохранить документ OneNote
dataDir = dataDir + "BuildDocAndInsertImageUsingImageStream_out.one";
doc.Save(dataDir);
```

Показывает, как добавить изображение из файла в документ.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_Images();

// Создаем объект класса Document
Document doc = new Document();

// Инициализировать объект класса Page
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Инициализируем объект класса Outline и устанавливаем свойства смещения
Outline outline = new Outline(doc);

// Инициализировать объект класса OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

// Загрузить изображение по пути к файлу.
Aspose.Note.Image image = new Aspose.Note.Image(doc, dataDir + "image.jpg")
                          {
                              // Установить выравнивание изображения
                              Alignment = HorizontalAlignment.Right
                          };

// Добавляем изображение
outlineElem.AppendChildLast(image);

// Добавляем элементы контура
outline.AppendChildLast(outlineElem);

// Добавляем узел Outline
page.AppendChildLast(outline);

// Добавить узел страницы
doc.AppendChildLast(page);

// Сохранить документ OneNote
dataDir = dataDir + "BuildDocAndInsertImage_out.one";
doc.Save(dataDir);
```

### Смотрите также

* enum [HorizontalAlignment](../../horizontalalignment/)
* class [Image](../)
* пространство имен [Aspose.Note](../../image/)
* сборка [Aspose.Note](../../../)


