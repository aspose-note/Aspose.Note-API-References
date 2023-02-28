---
title: Document.IsEncrypted
second_title: Справочник по API Aspose.Note для .NET
description: Document метод. Проверяет зашифрован ли документ из потока. Для проверки нам нужно полностью загрузить этот документ. Таким образом этот метод может привести к снижению производительности.
type: docs
weight: 150
url: /ru/net/aspose.note/document/isencrypted/
---
## IsEncrypted(Stream, LoadOptions, out Document) {#isencrypted_1}

Проверяет, зашифрован ли документ из потока. Для проверки нам нужно полностью загрузить этот документ. Таким образом, этот метод может привести к снижению производительности.

```csharp
public static bool IsEncrypted(Stream stream, LoadOptions options, out Document document)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | Stream | Поток. |
| options | LoadOptions | Параметры загрузки. |
| document | Document& | Загруженный документ. |

### Возвращаемое значение

Возвращает true, если документ зашифрован, иначе false.

### Примеры

Показывает, как проверить, защищен ли документ паролем.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (!Document.IsEncrypted(fileName, out document))
{
    Console.WriteLine("The document is loaded and ready to be processed.");
}
else
{
    Console.WriteLine("The document is encrypted. Provide a password.");
}
```

Показывает, как проверить, защищен ли документ определенным паролем.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (Document.IsEncrypted(fileName, "VerySecretPassword", out document))
{
    if (document != null)
    {
        Console.WriteLine("The document is decrypted. It is loaded and ready to be processed.");
    }
    else
    {
        Console.WriteLine("The document is encrypted. Invalid password was provided.");
    }
}
else
{
    Console.WriteLine("The document is NOT encrypted. It is loaded and ready to be processed.");
}
```

### Смотрите также

* class [LoadOptions](../../loadoptions/)
* class [Document](../)
* пространство имен [Aspose.Note](../../document/)
* сборка [Aspose.Note](../../../)

---

## IsEncrypted(Stream, string, out Document) {#isencrypted_2}

Проверяет, зашифрован ли документ из потока. Для проверки нам нужно полностью загрузить этот документ. Таким образом, этот метод может привести к снижению производительности.

```csharp
public static bool IsEncrypted(Stream stream, string password, out Document document)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | Stream | Поток. |
| password | String | Пароль для расшифровки документа. |
| document | Document& | Загруженный документ. |

### Возвращаемое значение

Возвращает true, если документ зашифрован, иначе false.

### Примеры

Показывает, как проверить, защищен ли документ паролем.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (!Document.IsEncrypted(fileName, out document))
{
    Console.WriteLine("The document is loaded and ready to be processed.");
}
else
{
    Console.WriteLine("The document is encrypted. Provide a password.");
}
```

Показывает, как проверить, защищен ли документ определенным паролем.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (Document.IsEncrypted(fileName, "VerySecretPassword", out document))
{
    if (document != null)
    {
        Console.WriteLine("The document is decrypted. It is loaded and ready to be processed.");
    }
    else
    {
        Console.WriteLine("The document is encrypted. Invalid password was provided.");
    }
}
else
{
    Console.WriteLine("The document is NOT encrypted. It is loaded and ready to be processed.");
}
```

### Смотрите также

* class [Document](../)
* пространство имен [Aspose.Note](../../document/)
* сборка [Aspose.Note](../../../)

---

## IsEncrypted(Stream, out Document) {#isencrypted}

Проверяет, зашифрован ли документ из потока. Для проверки нам нужно полностью загрузить этот документ. Таким образом, этот метод может привести к снижению производительности.

```csharp
public static bool IsEncrypted(Stream stream, out Document document)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| stream | Stream | Поток. |
| document | Document& | Загруженный документ. |

### Возвращаемое значение

Возвращает true, если документ зашифрован, иначе false.

### Примеры

Показывает, как проверить, защищен ли документ паролем.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (!Document.IsEncrypted(fileName, out document))
{
    Console.WriteLine("The document is loaded and ready to be processed.");
}
else
{
    Console.WriteLine("The document is encrypted. Provide a password.");
}
```

Показывает, как проверить, защищен ли документ определенным паролем.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (Document.IsEncrypted(fileName, "VerySecretPassword", out document))
{
    if (document != null)
    {
        Console.WriteLine("The document is decrypted. It is loaded and ready to be processed.");
    }
    else
    {
        Console.WriteLine("The document is encrypted. Invalid password was provided.");
    }
}
else
{
    Console.WriteLine("The document is NOT encrypted. It is loaded and ready to be processed.");
}
```

### Смотрите также

* class [Document](../)
* пространство имен [Aspose.Note](../../document/)
* сборка [Aspose.Note](../../../)

---

## IsEncrypted(string, LoadOptions, out Document) {#isencrypted_4}

Проверяет, зашифрован ли документ из файла. Для проверки нам нужно полностью загрузить этот документ. Таким образом, этот метод может привести к снижению производительности.

```csharp
public static bool IsEncrypted(string filePath, LoadOptions options, out Document document)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| filePath | String | Путь к файлу. |
| options | LoadOptions | Параметры загрузки. |
| document | Document& | Загруженный документ. |

### Возвращаемое значение

Возвращает true, если документ зашифрован, иначе false.

### Примеры

Показывает, как проверить, защищен ли документ паролем.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (!Document.IsEncrypted(fileName, out document))
{
    Console.WriteLine("The document is loaded and ready to be processed.");
}
else
{
    Console.WriteLine("The document is encrypted. Provide a password.");
}
```

Показывает, как проверить, защищен ли документ определенным паролем.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (Document.IsEncrypted(fileName, "VerySecretPassword", out document))
{
    if (document != null)
    {
        Console.WriteLine("The document is decrypted. It is loaded and ready to be processed.");
    }
    else
    {
        Console.WriteLine("The document is encrypted. Invalid password was provided.");
    }
}
else
{
    Console.WriteLine("The document is NOT encrypted. It is loaded and ready to be processed.");
}
```

### Смотрите также

* class [LoadOptions](../../loadoptions/)
* class [Document](../)
* пространство имен [Aspose.Note](../../document/)
* сборка [Aspose.Note](../../../)

---

## IsEncrypted(string, out Document) {#isencrypted_3}

Проверяет, зашифрован ли документ из файла. Для проверки нам нужно полностью загрузить этот документ. Таким образом, этот метод может привести к снижению производительности.

```csharp
public static bool IsEncrypted(string filePath, out Document document)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| filePath | String | Путь к файлу. |
| document | Document& | Загруженный документ. |

### Возвращаемое значение

Возвращает true, если документ зашифрован, иначе false.

### Примеры

Показывает, как проверить, защищен ли документ паролем.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (!Document.IsEncrypted(fileName, out document))
{
    Console.WriteLine("The document is loaded and ready to be processed.");
}
else
{
    Console.WriteLine("The document is encrypted. Provide a password.");
}
```

Показывает, как проверить, защищен ли документ определенным паролем.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (Document.IsEncrypted(fileName, "VerySecretPassword", out document))
{
    if (document != null)
    {
        Console.WriteLine("The document is decrypted. It is loaded and ready to be processed.");
    }
    else
    {
        Console.WriteLine("The document is encrypted. Invalid password was provided.");
    }
}
else
{
    Console.WriteLine("The document is NOT encrypted. It is loaded and ready to be processed.");
}
```

### Смотрите также

* class [Document](../)
* пространство имен [Aspose.Note](../../document/)
* сборка [Aspose.Note](../../../)

---

## IsEncrypted(string, string, out Document) {#isencrypted_5}

Проверяет, зашифрован ли документ из файла. Для проверки нам нужно полностью загрузить этот документ. Таким образом, этот метод может привести к снижению производительности.

```csharp
public static bool IsEncrypted(string filePath, string password, out Document document)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| filePath | String | Путь к файлу. |
| password | String | Пароль для расшифровки документа. |
| document | Document& | Загруженный документ. |

### Возвращаемое значение

Возвращает true, если документ зашифрован, иначе false.

### Примеры

Показывает, как проверить, защищен ли документ паролем.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (!Document.IsEncrypted(fileName, out document))
{
    Console.WriteLine("The document is loaded and ready to be processed.");
}
else
{
    Console.WriteLine("The document is encrypted. Provide a password.");
}
```

Показывает, как проверить, защищен ли документ определенным паролем.

```csharp
// Путь к каталогу документов.
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string fileName = Path.Combine(dataDir, "Aspose.one");

Document document;
if (Document.IsEncrypted(fileName, "VerySecretPassword", out document))
{
    if (document != null)
    {
        Console.WriteLine("The document is decrypted. It is loaded and ready to be processed.");
    }
    else
    {
        Console.WriteLine("The document is encrypted. Invalid password was provided.");
    }
}
else
{
    Console.WriteLine("The document is NOT encrypted. It is loaded and ready to be processed.");
}
```

### Смотрите также

* class [Document](../)
* пространство имен [Aspose.Note](../../document/)
* сборка [Aspose.Note](../../../)


