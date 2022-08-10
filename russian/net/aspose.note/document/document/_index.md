---
title: Document
second_title: Справочник по API Aspose.Note для .NET
description: Инициализирует новый экземплярDocumentaspose.note/document class. Создает пустой документ OneNote.
type: docs
weight: 10
url: /ru/net/aspose.note/document/document/
---
## Document() {#constructor}

Инициализирует новый экземпляр[`Document`](../../document) class. Создает пустой документ OneNote.

```csharp
public Document()
```

### Смотрите также

* class [Document](../../document)
* пространство имен [Aspose.Note](../../document)
* сборка [Aspose.Note](../../../)

---

## Document(string) {#constructor_3}

Инициализирует новый экземпляр[`Document`](../../document) class. Открывает существующий документ OneNote из файла.

```csharp
public Document(string filePath)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| filePath | String | Путь к файлу. |

### Исключения

| исключение | условие |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception) | Формат документа не распознан или не поддерживается. |
| [FileCorruptedException](../../filecorruptedexception) | Документ поврежден и не может быть загружен. |
| [IncorrectPasswordException](../../incorrectpasswordexception) | Документ зашифрован, и для его открытия требуется пароль, но вы указали неверный пароль. |
| InvalidOperationException | Возникла проблема с документом, о ней следует сообщить разработчикам Aspose.Note. |
| IOException | Существует исключение ввода/вывода. |

### Смотрите также

* class [Document](../../document)
* пространство имен [Aspose.Note](../../document)
* сборка [Aspose.Note](../../../)

---

## Document(string, LoadOptions) {#constructor_4}

Инициализирует новый экземпляр[`Document`](../../document) class. Открывает существующий документ OneNote из файла. Позволяет указать дополнительные параметры, такие как пароль шифрования.

```csharp
public Document(string filePath, LoadOptions loadOptions)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| filePath | String | Путь к файлу. |
| loadOptions | LoadOptions | Параметры, используемые для загрузки документа. Может быть нулевым. |

### Исключения

| исключение | условие |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception) | Формат документа не распознан или не поддерживается. |
| [FileCorruptedException](../../filecorruptedexception) | Документ поврежден и не может быть загружен. |
| [IncorrectPasswordException](../../incorrectpasswordexception) | Документ зашифрован, и для его открытия требуется пароль, но вы указали неверный пароль. |
| InvalidOperationException | Возникла проблема с документом, о ней следует сообщить разработчикам Aspose.Note. |
| IOException | Существует исключение ввода/вывода. |

### Смотрите также

* class [LoadOptions](../../loadoptions)
* class [Document](../../document)
* пространство имен [Aspose.Note](../../document)
* сборка [Aspose.Note](../../../)

---

## Document(Stream) {#constructor_1}

Инициализирует новый экземпляр[`Document`](../../document) class. Открывает существующий документ OneNote из потока.

```csharp
public Document(Stream inStream)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| inStream | Stream | Поток. |

### Исключения

| исключение | условие |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception) | Формат документа не распознан или не поддерживается. |
| [FileCorruptedException](../../filecorruptedexception) | Документ поврежден и не может быть загружен. |
| [IncorrectPasswordException](../../incorrectpasswordexception) | Документ зашифрован, и для его открытия требуется пароль, но вы указали неверный пароль. |
| InvalidOperationException | Возникла проблема с документом, о ней следует сообщить разработчикам Aspose.Note. |
| IOException | Существует исключение ввода/вывода. |
| ArgumentException | Поток не поддерживает чтение, имеет значение null или уже закрыт. |

### Смотрите также

* class [Document](../../document)
* пространство имен [Aspose.Note](../../document)
* сборка [Aspose.Note](../../../)

---

## Document(Stream, LoadOptions) {#constructor_2}

Инициализирует новый экземпляр[`Document`](../../document) class. Открывает существующий документ OneNote из потока. Позволяет указать дополнительные параметры, такие как пароль шифрования.

```csharp
public Document(Stream inStream, LoadOptions loadOptions)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| inStream | Stream | Поток. |
| loadOptions | LoadOptions | Параметры, используемые для загрузки документа. Может быть нулевым. |

### Исключения

| исключение | условие |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception) | Формат документа не распознан или не поддерживается. |
| [FileCorruptedException](../../filecorruptedexception) | Документ поврежден и не может быть загружен. |
| [IncorrectPasswordException](../../incorrectpasswordexception) | Документ зашифрован, и для его открытия требуется пароль, но вы указали неверный пароль. |
| InvalidOperationException | Возникла проблема с документом, о ней следует сообщить разработчикам Aspose.Note. |
| IOException | Существует исключение ввода/вывода. |
| ArgumentException | Поток не поддерживает чтение, имеет значение null или уже закрыт. |

### Смотрите также

* class [LoadOptions](../../loadoptions)
* class [Document](../../document)
* пространство имен [Aspose.Note](../../document)
* сборка [Aspose.Note](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
