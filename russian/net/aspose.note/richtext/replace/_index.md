---
title: RichText.Replace
second_title: Справочник по API Aspose.Note для .NET
description: RichText метод. Заменяет все вхождения указанного символа Unicode в этом экземпляре другим указанным символом Unicode.
type: docs
weight: 200
url: /ru/net/aspose.note/richtext/replace/
---
## Replace(char, char) {#replace}

Заменяет все вхождения указанного символа Unicode в этом экземпляре другим указанным символом Unicode.

```csharp
public RichText Replace(char oldChar, char newChar)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| oldChar | Char | Старый символ. |
| newChar | Char | Новый символ. |

### Возвращаемое значение

[`RichText`](../) .

### Смотрите также

* class [RichText](../)
* пространство имен [Aspose.Note](../../richtext/)
* сборка [Aspose.Note](../../../)

---

## Replace(string, string) {#replace_1}

Заменяет все вхождения указанной строки в текущем экземпляре другой указанной строкой.

```csharp
public RichText Replace(string oldValue, string newValue)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| oldValue | String | Старое значение. |
| newValue | String | Новое значение. |

### Возвращаемое значение

[`RichText`](../) .

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException |  |
| ArgumentException |  |

### Примеры

Показывает, как пройти через текст страницы и сделать замену.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("voice over", "voice over new text");

// Загрузите документ в Aspose.Note.
Document oneFile = new Document(dataDir + "Aspose.one");

IList<Page> pageNodes = oneFile.GetChildNodes<Page>();

// Получить все узлы RichText
IList<RichText> textNodes = pageNodes[0].GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // Заменяем текст фигуры
        richText.Replace(kvp.Key, kvp.Value);
    }
}

// Сохраняем в любой поддерживаемый формат файла
dataDir = dataDir + "ReplaceTextOnParticularPage_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

Показывает, как создать новый документ, заменив специальные фрагменты текста в шаблоне.

```csharp
string dataDir = RunExamples.GetDataDir_Text();

var D = new Dictionary<string, string>
            {
                { "Company", "Atlas Shrugged Ltd" },
                { "CandidateName", "John Galt" },
                { "JobTitle", "Chief Entrepreneur Officer" },
                { "Department", "Sales" },
                { "Salary", "123456 USD" },
                { "Vacation", "30" },
                { "StartDate", "29 Feb 2024" },
                { "YourName", "Ayn Rand" }
            };

// Загрузите шаблон документа в Aspose.Note.
var d = new Document(Path.Combine(dataDir, "JobOffer.one"));

// Заменим все слова шаблона
foreach (var e in d.GetChildNodes<RichText>())
{
    foreach (var replace in D)
    {
        e.Replace($"${{{replace.Key}}}", replace.Value);
    }
}

d.Save(Path.Combine(dataDir, "JobOffer_out.one"));
```

### Смотрите также

* class [RichText](../)
* пространство имен [Aspose.Note](../../richtext/)
* сборка [Aspose.Note](../../../)

---

## Replace(string, string, TextStyle) {#replace_2}

Заменяет все вхождения указанной строки в текущем экземпляре другой указанной строкой в указанном стиле.

```csharp
public RichText Replace(string oldValue, string newValue, TextStyle style)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| oldValue | String | Старое значение. |
| newValue | String | Новое значение. |
| style | TextStyle | Стиль нового значения. |

### Возвращаемое значение

[`RichText`](../) .

### Исключения

| исключение | условие |
| --- | --- |
| ArgumentNullException |  |
| ArgumentException |  |

### Смотрите также

* class [TextStyle](../../textstyle/)
* class [RichText](../)
* пространство имен [Aspose.Note](../../richtext/)
* сборка [Aspose.Note](../../../)


