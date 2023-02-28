---
title: NumberList.Format
second_title: Справочник по API Aspose.Note для .NET
description: NumberList свойство. Получает или задает формат заголовка строки. Для маркированных списков представляет собой символ маркера.
type: docs
weight: 50
url: /ru/net/aspose.note/numberlist/format/
---
## NumberList.Format property

Получает или задает формат заголовка строки. Для маркированных списков представляет собой символ маркера.

```csharp
public string Format { get; set; }
```

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

### Смотрите также

* class [NumberList](../)
* пространство имен [Aspose.Note](../../numberlist/)
* сборка [Aspose.Note](../../../)


