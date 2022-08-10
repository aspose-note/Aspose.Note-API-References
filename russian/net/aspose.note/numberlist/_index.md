---
title: NumberList
second_title: Справочник по API Aspose.Note для .NET
description: Представляет нумерованный или маркированный список.
type: docs
weight: 420
url: /ru/net/aspose.note/numberlist/
---
## NumberList class

Представляет нумерованный или маркированный список.

```csharp
public class NumberList
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [NumberList](numberlist#constructor_1)(string, string, int) | Инициализирует новый экземпляр[`NumberList`](../numberlist) class. Этот экземпляр представляет собой маркированный список. |
| [NumberList](numberlist#constructor)(string, NumberFormat, string, int) | Инициализирует новый экземпляр[`NumberList`](../numberlist)class. Этот экземпляр представляет нумерованный список. |

## Характеристики

| Имя | Описание |
| --- | --- |
| [Font](../../aspose.note/numberlist/font) { get; set; } | Получает или задает имя шрифта. |
| [FontColor](../../aspose.note/numberlist/fontcolor) { get; set; } | Получает или задает цвет шрифта. |
| [FontSize](../../aspose.note/numberlist/fontsize) { get; set; } | Получает или задает размер шрифта. |
| [Format](../../aspose.note/numberlist/format) { get; set; } | Получает или задает формат заголовка строки. Для маркированных списков представляет собой символ маркера. |
| [IsBold](../../aspose.note/numberlist/isbold) { get; set; } | Получает или задает значение, указывающее, является ли текст полужирным. |
| [IsItalic](../../aspose.note/numberlist/isitalic) { get; set; } | Получает или задает значение, указывающее, является ли стиль текста курсивом. |
| [LastModifiedTime](../../aspose.note/numberlist/lastmodifiedtime) { get; set; } | Получает или устанавливает время последнего изменения. |
| [NumberFormat](../../aspose.note/numberlist/numberformat) { get; set; } | Получает или задает числовой формат, используемый для группы автоматически нумерованных объектов. Должно быть пустым для маркированных списков. |
| [Restart](../../aspose.note/numberlist/restart) { get; set; } | Получает или задает числовое значение, которое переопределяет автоматическое числовое значение элемента списка. |

## Методы

| Имя | Описание |
| --- | --- |
| [Equals](../../aspose.note/numberlist/equals#equals)(NumberList) | Определяет, равен ли указанный объект текущему объекту. |
| override [Equals](../../aspose.note/numberlist/equals#equals_1)(object) | Определяет, равен ли указанный объект текущему объекту. |
| override [GetHashCode](../../aspose.note/numberlist/gethashcode)() | Служит хеш-функцией для типа. |
| [GetNumberedListHeader](../../aspose.note/numberlist/getnumberedlistheader)(int) | Получает заголовок нумерованного списка. |

### Примеры

Показывает, как получить информацию о форматировании списка.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Загрузите документ в Aspose.Note.
Document oneFile = new Document(dataDir + "ApplyNumberingOnText.one");

// Извлекаем коллекцию узлов элемента схемы
IList<OutlineElement> nodes = oneFile.GetChildNodes<OutlineElement>();

// Итерация по каждому узлу
foreach (OutlineElement node in nodes)
{
    if (node.NumberList != null)
    {
        NumberList list = node.NumberList;

        // Получаем имя шрифта
        Console.WriteLine("Font Name: " + list.Font);

        // Получить длину шрифта
        Console.WriteLine("Font Length: " + list.Font.Length);

        // Получить размер шрифта
        Console.WriteLine("Font Size: " + list.FontSize);

        // Получаем цвет шрифта
        Console.WriteLine("Font Color: " + list.FontColor);

        // Получить формат
        Console.WriteLine("Font format: " + list.Format);

        // Проверяем полужирный
        Console.WriteLine("Is bold: " + list.IsBold);

        // Проверяем курсив
        Console.WriteLine("Is italic: " + list.IsItalic);
        Console.WriteLine();
    }
}
```

Показывает, как вставить новый список с китайской нумерацией.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Инициализировать документ OneNote
Aspose.Note.Document doc = new Aspose.Note.Document();

// Инициализировать страницу OneNote
Aspose.Note.Page page = new Aspose.Note.Page(doc);
Outline outline = new Outline(doc);

// Применяем настройки стиля текста
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Числа в одном контуре автоматически увеличиваются.
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

//---------------------------------------------------------------------
OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

//---------------------------------------------------------------------
OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.ChineseCounting, "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

//---------------------------------------------------------------------
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);
page.AppendChildLast(outline);
doc.AppendChildLast(page);

// Сохранить документ OneNote
dataDir = dataDir + "InsertChineseNumberList_out.one"; 
doc.Save(dataDir);
```

Показывает, как вставить новый список с нумерацией.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

// Создаем объект класса Document
Document doc = new Document();

// Инициализировать объект класса Page
Aspose.Note.Page page = new Aspose.Note.Page(doc);

// Инициализировать объект класса Outline
Outline outline = new Outline(doc);

// Инициализируем объект класса TextStyle и устанавливаем свойства форматирования
ParagraphStyle defaultStyle = new ParagraphStyle { FontColor = Color.Black, FontName = "Arial", FontSize = 10 };

// Инициализировать объекты класса OutlineElement и применить нумерацию
// Числа в одном контуре автоматически увеличиваются.
OutlineElement outlineElem1 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text1 = new RichText(doc) { Text = "First", ParagraphStyle = defaultStyle };
outlineElem1.AppendChildLast(text1);

OutlineElement outlineElem2 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text2 = new RichText(doc) { Text = "Second", ParagraphStyle = defaultStyle };
outlineElem2.AppendChildLast(text2);

OutlineElement outlineElem3 = new OutlineElement(doc) { NumberList = new NumberList("{0})", NumberFormat.DecimalNumbers, "Arial", 10) };
RichText text3 = new RichText(doc) { Text = "Third", ParagraphStyle = defaultStyle };
outlineElem3.AppendChildLast(text3);

// Добавляем элементы контура
outline.AppendChildLast(outlineElem1);
outline.AppendChildLast(outlineElem2);
outline.AppendChildLast(outlineElem3);

// Добавляем узел Outline
page.AppendChildLast(outline);

// Добавить узел страницы
doc.AppendChildLast(page);

// Сохранить документ OneNote
dataDir = dataDir + "ApplyNumberingOnText_out.one"; 
doc.Save(dataDir);
```

### Смотрите также

* пространство имен [Aspose.Note](../../aspose.note)
* сборка [Aspose.Note](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
