---
title: Image
second_title: Справочник по API Aspose.Note для .NET
description: Представляет изображение.
type: docs
weight: 240
url: /ru/net/aspose.note/image/
---
## Image class

Представляет изображение.

```csharp
public sealed class Image : Node, IOutlineElementChildNode, IPageChildNode, ITaggable
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [Image](image#constructor)() | Инициализирует новый экземпляр[`Image`](../image) класс. |
| [Image](image#constructor_4)(string, Stream) | Инициализирует новый экземпляр[`Image`](../image) класс. |
| [Image](image#constructor_5)(string, string, string) | Инициализирует новый экземпляр[`Image`](../image) класс. |

## Характеристики

| Имя | Описание |
| --- | --- |
| [Alignment](../../aspose.note/image/alignment) { get; set; } | Получает или задает выравнивание. |
| [AlternativeTextDescription](../../aspose.note/image/alternativetextdescription) { get; set; } | Получает или задает текст альтернативного текста для изображения. |
| [AlternativeTextTitle](../../aspose.note/image/alternativetexttitle) { get; set; } | Получает или задает заголовок альтернативного текста для изображения. |
| [Bytes](../../aspose.note/image/bytes) { get; } | Получает хранилище данных изображения. |
| [Document](../../aspose.note/node/document) { get; } | Получает документ узла. |
| [FileName](../../aspose.note/image/filename) { get; } | Получает имя файла. |
| [FilePath](../../aspose.note/image/filepath) { get; } | Получает путь к файлу изображения. |
| [Format](../../aspose.note/image/format) { get; } | Получает формат изображения. |
| [Height](../../aspose.note/image/height) { get; set; } | Получает или задает высоту. Это реальная высота изображения в документе MS OneNote. |
| [HorizontalOffset](../../aspose.note/image/horizontaloffset) { get; set; } | Получает или задает смещение по горизонтали. |
| [HyperlinkUrl](../../aspose.note/image/hyperlinkurl) { get; set; } | Получает или задает гиперссылку, связанную с изображением. |
| [IsBackground](../../aspose.note/image/isbackground) { get; set; } | Получает, является ли изображение фоновым изображением. |
| virtual [IsComposite](../../aspose.note/node/iscomposite) { get; } | Получает значение, указывающее, является ли этот узел составным. Если true, узел может иметь дочерние узлы. |
| [LastModifiedTime](../../aspose.note/image/lastmodifiedtime) { get; set; } | Получает или устанавливает время последнего изменения. |
| [NextSibling](../../aspose.note/node/nextsibling) { get; } | Получает следующий узел на том же уровне дерева узлов. |
| [NodeType](../../aspose.note/node/nodetype) { get; } | Получает тип узла. |
| [OriginalHeight](../../aspose.note/image/originalheight) { get; } | Получает исходную высоту. Это исходная ширина изображения до изменения размера. |
| [OriginalWidth](../../aspose.note/image/originalwidth) { get; } | Получает исходную ширину. Это исходная ширина изображения до изменения размера. |
| [ParentNode](../../aspose.note/node/parentnode) { get; } | Получает родительский узел. |
| [PreviousSibling](../../aspose.note/node/previoussibling) { get; } | Получает предыдущий узел на том же уровне дерева узлов. |
| [Tags](../../aspose.note/image/tags) { get; } | Получает список всех тегов абзаца. |
| [VerticalOffset](../../aspose.note/image/verticaloffset) { get; set; } | Получает или задает вертикальное смещение. |
| [Width](../../aspose.note/image/width) { get; set; } | Получает или задает ширину. Это реальная ширина изображения в документе MS OneNote. |

## Методы

| Имя | Описание |
| --- | --- |
| override [Accept](../../aspose.note/image/accept)(DocumentVisitor) | Принимает посетителя узла. |

### Примеры

Показывает, как привязать гиперссылку к изображению.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_Images(); 

var document = new Document();

var page = new Page(document);

var image = new Image(document, dataDir + "image.jpg") { HyperlinkUrl = "http://image.com" };

page.AppendChildLast(image);

document.AppendChildLast(page);

document.Save(dataDir + "Image with Hyperlink_out.one");
```

Показывает, как установить текстовое описание для изображения.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_Images();

var document = new Document();
var page = new Page(document);
var image = new Image(document, dataDir + "image.jpg")
            {
                AlternativeTextTitle = "This is an image's title!",
                AlternativeTextDescription = "And this is an image's description!"
            };
page.AppendChildLast(image);
document.AppendChildLast(page);

dataDir = dataDir + "ImageAlternativeText_out.one";
document.Save(dataDir);
```

Показывает, как получить изображение из документа.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_Images();

// Загрузите документ в Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Получить все узлы изображения
IList<Aspose.Note.Image> nodes = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in nodes)
{
    using (MemoryStream stream = new MemoryStream(image.Bytes))
    {
        using (Bitmap bitMap = new Bitmap(stream))
        {
            // Сохраняем байты изображения в файл
            bitMap.Save(String.Format(dataDir + "{0}", Path.GetFileName(image.FileName)));
        }
    }
}
```

Показывает, как получить метаинформацию изображения.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_Images();

// Загрузите документ в Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

// Получить все узлы изображения
IList<Aspose.Note.Image> images = oneFile.GetChildNodes<Aspose.Note.Image>();

foreach (Aspose.Note.Image image in images)
{
    Console.WriteLine("Width: {0}", image.Width);
    Console.WriteLine("Height: {0}", image.Height);
    Console.WriteLine("OriginalWidth: {0}", image.OriginalWidth);
    Console.WriteLine("OriginalHeight: {0}", image.OriginalHeight);
    Console.WriteLine("FileName: {0}", image.FileName);
    Console.WriteLine("LastModifiedTime: {0}", image.LastModifiedTime);
    Console.WriteLine();
}
```

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

* class [Node](../node)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode)
* interface [IPageChildNode](../ipagechildnode)
* interface [ITaggable](../itaggable)
* пространство имен [Aspose.Note](../../aspose.note)
* сборка [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
