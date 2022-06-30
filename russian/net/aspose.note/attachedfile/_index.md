---
title: AttachedFile
second_title: Справочник по API Aspose.Note для .NET
description: Представляет прикрепленный файл.
type: docs
weight: 10
url: /ru/net/aspose.note/attachedfile/
---
## AttachedFile class

Представляет прикрепленный файл.

```csharp
public class AttachedFile : Node, IOutlineElementChildNode, IPageChildNode, ITaggable
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [AttachedFile](attachedfile#constructor)() | Инициализирует новый экземпляр класса[`AttachedFile`](../attachedfile). |
| [AttachedFile](attachedfile#constructor_6)(string, Stream) | Инициализирует новый экземпляр класса[`AttachedFile`](../attachedfile). |
| [AttachedFile](attachedfile#constructor_7)(string, Stream, ImageFormat) | Инициализирует новый экземпляр класса[`AttachedFile`](../attachedfile). |
| [AttachedFile](attachedfile#constructor_8)(string, Stream, Stream, ImageFormat) | Инициализирует новый экземпляр класса[`AttachedFile`](../attachedfile). |

## Характеристики

| Имя | Описание |
| --- | --- |
| [Alignment](../../aspose.note/attachedfile/alignment) { get; set; } | Получает или задает выравнивание. |
| [AlternativeTextDescription](../../aspose.note/attachedfile/alternativetextdescription) { get; set; } | Получает или задает тело альтернативного текста для иконки вложенного файла. |
| [AlternativeTextTitle](../../aspose.note/attachedfile/alternativetexttitle) { get; set; } | Получает или задает заголовок альтернативного текста для значка вложенного файла. |
| [Bytes](../../aspose.note/attachedfile/bytes) { get; } | Получает двоичные данные для встроенного файла. |
| [Document](../../aspose.note/node/document) { get; } | Получает документ узла. |
| [Extension](../../aspose.note/attachedfile/extension) { get; } | Получает расширение встроенного файла. |
| [FileName](../../aspose.note/attachedfile/filename) { get; } | Получает имя внедренного файла. |
| [FilePath](../../aspose.note/attachedfile/filepath) { get; } | Получает путь к исходному файлу. |
| [Height](../../aspose.note/attachedfile/height) { get; } | Получает исходную высоту встроенного значка файла. |
| [HorizontalOffset](../../aspose.note/attachedfile/horizontaloffset) { get; set; } | Получает или задает смещение по горизонтали. |
| [Icon](../../aspose.note/attachedfile/icon) { get; } | Получает двоичные данные для значка, связанного с внедренным файлом. |
| [IconExtension](../../aspose.note/attachedfile/iconextension) { get; } | Получает расширение значка. |
| virtual [IsComposite](../../aspose.note/node/iscomposite) { get; } | Получает значение, указывающее, является ли этот узел составным. Если true, узел может иметь дочерние узлы. |
| [IsPrintout](../../aspose.note/attachedfile/isprintout) { get; set; } | Получает или задает значение, указывающее, является ли представление файла распечатанным. |
| [IsSizeSetByUser](../../aspose.note/attachedfile/issizesetbyuser) { get; set; } | Получает или задает значение, указывающее, было ли значение размера значка обновлено пользователем явно. |
| [LastModifiedTime](../../aspose.note/attachedfile/lastmodifiedtime) { get; set; } | Получает или задает время последнего изменения. |
| [MaxHeight](../../aspose.note/attachedfile/maxheight) { get; set; } | Получает или задает максимальную высоту для отображения встроенного значка файла. |
| [MaxWidth](../../aspose.note/attachedfile/maxwidth) { get; set; } | Получает или задает максимальную ширину для отображения встроенного значка файла. |
| [NextSibling](../../aspose.note/node/nextsibling) { get; } | Получает следующий узел на том же уровне дерева узлов. |
| [NodeType](../../aspose.note/node/nodetype) { get; } | Получает тип узла. |
| [ParentNode](../../aspose.note/node/parentnode) { get; } | Получает родительский узел. |
| [PreviousSibling](../../aspose.note/node/previoussibling) { get; } | Получает предыдущий узел на том же уровне дерева узлов. |
| [Tags](../../aspose.note/attachedfile/tags) { get; } | Получает список всех тегов абзаца. |
| [Text](../../aspose.note/attachedfile/text) { get; set; } | Получает или задает текстовое представление встроенного файла. Строка НЕ ДОЛЖНА содержать символы со значением 10 (перевод строки) или 13 (возврат каретки). |
| [VerticalOffset](../../aspose.note/attachedfile/verticaloffset) { get; set; } | Получает или задает вертикальное смещение. |
| [Width](../../aspose.note/attachedfile/width) { get; } | Получает исходную ширину встроенного значка файла. |

## Методы

| Имя | Описание |
| --- | --- |
| override [Accept](../../aspose.note/attachedfile/accept)(DocumentVisitor) | Принимает посетителя узла. |

### Примеры

Показывает, как получить содержимое прикрепленного файла.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_Attachments();

// Загрузите документ в Aspose.Note.
Document oneFile = new Document(dataDir + "Sample1.one");

// Получаем список узлов прикрепленных файлов
IList<AttachedFile> nodes = oneFile.GetChildNodes<AttachedFile>();

// Перебираем все узлы
foreach (AttachedFile file in nodes)
{
    // Загружаем прикрепленный файл в объект потока
    using (Stream outputStream = new MemoryStream(file.Bytes))
    {
        // Создаем локальный файл
        using (Stream fileStream = System.IO.File.OpenWrite(String.Format(dataDir + file.FileName)))
        {
            // Копируем файловый поток
            CopyStream(outputStream, fileStream);
        }
    }
}
```

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_Attachments();

// Создаем объект класса Document
Document doc = new Document();

// Инициализировать объект класса Page
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Инициализировать объект класса Outline
Outline outline = new Outline(doc);

// Инициализировать объект класса OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

// Инициализировать объект класса AttachedFile
AttachedFile attachedFile = new AttachedFile(doc,  dataDir + "attachment.txt");

// Добавляем прикрепленный файл
outlineElem.AppendChildLast(attachedFile);

// Добавляем узел элемента контура
outline.AppendChildLast(outlineElem);

// Добавляем узел контура
page.AppendChildLast(outline);

// Добавляем узел страницы
doc.AppendChildLast(page);

dataDir = dataDir + "AttachFileByPath_out.one";
doc.Save(dataDir);
```

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_Attachments();

// Создаем объект класса Document
Document doc = new Document();

// Инициализировать объект класса Page
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Инициализировать объект класса Outline
Outline outline = new Outline(doc);

// Инициализировать объект класса OutlineElement
OutlineElement outlineElem = new OutlineElement(doc);

using (var stream = File.OpenRead(dataDir + "icon.jpg"))
{
    // Инициализируем объект класса AttachedFile, а также передаем путь к его значку
    AttachedFile attachedFile = new AttachedFile(doc, dataDir + "attachment.txt", stream, ImageFormat.Jpeg);

    // Добавляем прикрепленный файл
    outlineElem.AppendChildLast(attachedFile);
}

// Добавляем узел элемента контура
outline.AppendChildLast(outlineElem);

// Добавляем узел контура
page.AppendChildLast(outline);

// Добавляем узел страницы
doc.AppendChildLast(page);

dataDir = dataDir + "AttachFileAndSetIcon_out.one";
doc.Save(dataDir);
```

Показывает, как добавить файл в документ, используя путь к файлу.

Показывает, как добавить файл из потока в документ.

### Смотрите также

* class [Node](../node)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode)
* interface [IPageChildNode](../ipagechildnode)
* interface [ITaggable](../itaggable)
* пространство имен [Aspose.Note](../../aspose.note)
* сборка [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
