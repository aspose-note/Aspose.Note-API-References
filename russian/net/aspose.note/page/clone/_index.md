---
title: Page.Clone
second_title: Справочник по API Aspose.Note для .NET
description: Page метод. Клонирует страницу.
type: docs
weight: 140
url: /ru/net/aspose.note/page/clone/
---
## Page.Clone method

Клонирует страницу.

```csharp
public Page Clone(bool cloneHistory = false)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| cloneHistory | Boolean | Указывает, следует ли клонировать историю страницы.. |

### Возвращаемое значение

Клон страницы.

### Примеры

Показывает, как отправить текущую версию страницы в историю.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_Pages();

// Загрузить документ OneNote и получить первый дочерний элемент           
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

var pageHistory = document.GetPageHistory(page);

pageHistory.Add(page.Clone());

document.Save(dataDir + "PushCurrentPageVersion_out.one");
```

Показывает, как клонировать страницу.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_Pages();

// Загрузить документ OneNote
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// Клонировать в новый документ без истории
var cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone());

// Клонируем в новый документ с историей
cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone(true));
```

### Смотрите также

* class [Page](../)
* пространство имен [Aspose.Note](../../page/)
* сборка [Aspose.Note](../../../)


