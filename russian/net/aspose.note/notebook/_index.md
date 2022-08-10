---
title: Notebook
second_title: Справочник по API Aspose.Note для .NET
description: Представляет записную книжку Aspose.Note.
type: docs
weight: 390
url: /ru/net/aspose.note/notebook/
---
## Notebook class

Представляет записную книжку Aspose.Note.

```csharp
public class Notebook : IEnumerable<INotebookChildNode>, INotebookChildNode
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [Notebook](notebook#constructor)() | Инициализирует новый экземпляр[`Notebook`](../notebook) класс. |
| [Notebook](notebook#constructor_1)(Stream) | Инициализирует новый экземпляр[`Notebook`](../notebook) class. Открывает существующую записную книжку OneNote из потока. |
| [Notebook](notebook#constructor_3)(string) | Инициализирует новый экземпляр[`Notebook`](../notebook) class. Открывает существующую записную книжку OneNote из файла. |
| [Notebook](notebook#constructor_2)(Stream, NotebookLoadOptions) | Инициализирует новый экземпляр[`Notebook`](../notebook) class. Открывает существующую записную книжку OneNote из потока. Позволяет указать дополнительные параметры загрузки. |
| [Notebook](notebook#constructor_4)(string, NotebookLoadOptions) | Инициализирует новый экземпляр[`Notebook`](../notebook)class. Открывает существующую записную книжку OneNote из файла. Позволяет указать дополнительные параметры, такие как стратегия загрузки детей («ленивый»/мгновенный). |

## Характеристики

| Имя | Описание |
| --- | --- |
| [Color](../../aspose.note/notebook/color) { get; set; } | Получает или задает цвет. |
| [Count](../../aspose.note/notebook/count) { get; } | Получает количество элементов, содержащихся в[`Notebook`](../notebook) . |
| [DisplayName](../../aspose.note/notebook/displayname) { get; set; } | Получает или задает отображаемое имя. |
| [FileFormat](../../aspose.note/notebook/fileformat) { get; } | Получает формат файла (OneNote 2010, OneNote Online). |
| [Guid](../../aspose.note/notebook/guid) { get; } | Получает глобально уникальный идентификатор объекта. |
| [IsHistoryEnabled](../../aspose.note/notebook/ishistoryenabled) { get; set; } | Получает или задает значение, указывающее, включена ли история. |
| [Item](../../aspose.note/notebook/item) { get; } | Получает дочерний узел ноутбука по заданному индексу. |

## Методы

| Имя | Описание |
| --- | --- |
| [AppendChild](../../aspose.note/notebook/appendchild)(INotebookChildNode) | Добавляет узел в конец списка. |
| [GetChildNodes&lt;T1&gt;](../../aspose.note/notebook/getchildnodes)() | Получить все дочерние узлы по типу узла. |
| [GetEnumerator](../../aspose.note/notebook/getenumerator)() | Возвращает перечислитель, который перебирает дочерние узлы[`Notebook`](../notebook) . |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument#loadchilddocument)(Stream) | Добавляет узел дочернего документа. Открывает существующий документ OneNote из потока. |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument#loadchilddocument_2)(string) | Добавляет узел дочернего документа. Открывает существующий документ OneNote из файла. |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument#loadchilddocument_1)(Stream, LoadOptions) | Добавляет дочерний узел документа. Открывает существующий документ OneNote из потока. Позволяет указать дополнительные параметры загрузки. |
| [LoadChildDocument](../../aspose.note/notebook/loadchilddocument#loadchilddocument_3)(string, LoadOptions) | Добавляет дочерний узел документа. Открывает существующий документ OneNote из файла. Позволяет указать дополнительные параметры загрузки. |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook#loadchildnotebook)(Stream) | Добавляет узел дочерней записной книжки. Открывает существующую записную книжку OneNote из потока. |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook#loadchildnotebook_2)(string) | Добавляет узел дочерней записной книжки. Открывает существующую записную книжку OneNote из файла. |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook#loadchildnotebook_1)(Stream, NotebookLoadOptions) | Добавляет узел дочерней записной книжки. Открывает существующую записную книжку OneNote из потока. Позволяет указать дополнительные параметры загрузки. |
| [LoadChildNotebook](../../aspose.note/notebook/loadchildnotebook#loadchildnotebook_3)(string, NotebookLoadOptions) | Добавляет узел дочерней записной книжки. Открывает существующую записную книжку OneNote из файла. Позволяет указать дополнительные параметры загрузки. |
| [RemoveChild](../../aspose.note/notebook/removechild)(INotebookChildNode) | Удаляет дочерний узел. |
| [Save](../../aspose.note/notebook/save#save)(Stream) | Сохраняет документ OneNote в поток. |
| [Save](../../aspose.note/notebook/save#save_3)(string) | Сохраняет документ OneNote в файл. |
| [Save](../../aspose.note/notebook/save#save_2)(Stream, NotebookSaveOptions) | Сохраняет документ OneNote в поток, используя указанные параметры сохранения. |
| [Save](../../aspose.note/notebook/save#save_1)(Stream, SaveFormat) | Сохраняет документ OneNote в поток в указанном формате. |
| [Save](../../aspose.note/notebook/save#save_5)(string, NotebookSaveOptions) | Сохраняет документ OneNote в файл, используя указанные параметры сохранения. |
| [Save](../../aspose.note/notebook/save#save_4)(string, SaveFormat) | Сохраняет документ OneNote в файл в указанном формате. |

### Примеры

Показывает, как сохранить блокнот.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_NoteBook();

var notebook = new Notebook();

dataDir = dataDir + "test_out.onetoc2";

// Сохраняем блокнот
notebook.Save(dataDir);
```

Показывает, как сохранить блокнот в формате pdf.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Загрузить блокнот OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

dataDir = dataDir + "ConvertToPDF_out.pdf";

// Сохраняем блокнот
notebook.Save(dataDir);
```

Показывает, как сохранить блокнот как изображение.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Загрузить блокнот OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

dataDir = dataDir + "ConvertToImage_out.png";

// Сохраняем блокнот
notebook.Save(dataDir);
```

Показывает, как получить весь текст из записной книжки.

```csharp
string inputFile = "notebook.onetoc2";
string dataDir = RunExamples.GetDataDir_NoteBook();

Notebook rootNotebook = new Notebook(dataDir + inputFile);

IList<RichText> allRichTextNodes = rootNotebook.GetChildNodes<RichText>();
foreach (RichText richTextNode in allRichTextNodes)
{
    Console.WriteLine(richTextNode.Text);
}
```

Показывает, как сохранить плоский блокнот в формате pdf.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Загрузить блокнот OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

// Сохраняем блокнот
dataDir = dataDir + "ConvertToPDFAsFlattened_out.pdf";
notebook.Save(
    dataDir,
    new NotebookPdfSaveOptions
    {
        Flatten = true
    });
```

Показывает, как перебирать документы блокнота, загружая их лениво.

```csharp
string inputFile = "Notizbuch öffnen.onetoc2";
string dataDir = RunExamples.GetDataDir_NoteBook();

// По умолчанию загрузка детей «ленивая».
Notebook notebook = new Notebook(dataDir + inputFile);

foreach (var notebookChildNode in notebook.OfType<Document>()) 
{
    // Фактическая загрузка дочернего документа происходит только здесь.
    // Делаем что-то с дочерним документом
}
```

Показывает, как добавить новый раздел в записную книжку.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Загрузить блокнот OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

// Добавляем новый дочерний элемент в Блокнот
notebook.AppendChild(new Document(dataDir + "Neuer Abschnitt 1.one"));

dataDir = dataDir + "AddChildNode_out.onetoc2";

// Сохраняем блокнот
notebook.Save(dataDir);
```

Показывает, как загрузить блокнот из потока.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_NoteBook();

FileStream stream = new FileStream(dataDir + "Notizbuch öffnen.onetoc2", FileMode.Open);

var notebook = new Notebook(stream);

using (FileStream childStream = new FileStream(dataDir + "Aspose.one", FileMode.Open))
{
    notebook.LoadChildDocument(childStream);
}

notebook.LoadChildDocument(dataDir + "Sample1.one");
```

Показывает, как зашифровать блокнот.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_NoteBook();
var notebook = new Notebook(dataDir + "test.onetoc2", new NotebookLoadOptions() { DeferredLoading = true });

notebook.LoadChildDocument(dataDir + "Aspose.one");  
notebook.LoadChildDocument(dataDir + "Locked Pass1.one", new LoadOptions() { DocumentPassword = "pass" });
notebook.LoadChildDocument(dataDir + "Locked Pass2.one", new LoadOptions() { DocumentPassword = "pass2" });
```

Показывает, как сохранить записную книжку как изображение с указанными параметрами.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Загрузить блокнот OneNote
var notebook = new Notebook(dataDir + "Notizbuch �ffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;

dataDir = dataDir + "ConvertToImageWithOptions_out.png";

// Сохраняем блокнот
notebook.Save(dataDir, notebookSaveOptions);
```

Показывает, как сохранить плоский блокнот как изображение.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Загрузить блокнот OneNote
var notebook = new Notebook(dataDir + "Notizbuch öffnen.onetoc2");

var notebookSaveOptions = new NotebookImageSaveOptions(SaveFormat.Png);

var documentSaveOptions = notebookSaveOptions.DocumentSaveOptions;

documentSaveOptions.Resolution = 400;
notebookSaveOptions.Flatten = true;

dataDir = dataDir + "ConvertToImageAsFlattenedNotebook_out.png";

// Сохраняем блокнот
notebook.Save(dataDir, notebookSaveOptions);
```

Показывает, как удалить раздел из блокнота.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_NoteBook();

// Загрузить блокнот OneNote
var notebook = new Notebook(dataDir + "test.onetoc2");

// Проходим через его дочерние узлы для поиска нужного дочернего элемента
foreach (var child in new List<INotebookChildNode>(notebook))
{
    if (child.DisplayName == "Remove Me")
    {
        // Удалить дочерний элемент из блокнота
        notebook.RemoveChild(child);
    }
}

dataDir = dataDir + "RemoveChildNode_out.onetoc2";

// Сохраняем блокнот
notebook.Save(dataDir);
```

Показывает, как перебирать предварительно загруженные документы записной книжки.

```csharp
// По умолчанию загрузка детей «ленивая».
// Поэтому для мгновенной загрузки произошла,
// необходимо установить флаг NotebookLoadOptions.InstantLoading.
NotebookLoadOptions loadOptions = new NotebookLoadOptions { InstantLoading = true };

String inputFile = "Notizbuch öffnen.onetoc2";
String dataDir = RunExamples.GetDataDir_NoteBook();
Notebook notebook = new Notebook(dataDir + inputFile, loadOptions);

// Все дочерние документы уже загружены.
foreach (INotebookChildNode notebookChildNode in notebook.OfType<Document>()) 
{
   // Делаем что-то с дочерним документом
}
```

Показывает, как пройти через содержимое записной книжки.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = "Open Notebook.onetoc2";
try
{
    var notebook = new Notebook(dataDir + fileName);
    foreach (var notebookChildNode in notebook)
    {
        Console.WriteLine(notebookChildNode.DisplayName);
        if (notebookChildNode is Document)
        {
            // Делаем что-то с дочерним документом
        }
        else if (notebookChildNode is Notebook)
        {
            // Делаем что-нибудь с дочерним блокнотом
        }
    }
}
catch (Exception ex)
{
    Console.WriteLine(ex.Message);
}
```

### Смотрите также

* interface [INotebookChildNode](../inotebookchildnode)
* пространство имен [Aspose.Note](../../aspose.note)
* сборка [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
