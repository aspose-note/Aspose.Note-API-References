---
title: "Document"
second_title: "Справочник API Aspose.Note for Java"
description: "Представляет документ Aspose.Note."
type: docs
weight: 20
url: /ru/java/com.aspose.note/document/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode

**All Implemented Interfaces:**
[com.aspose.note.INotebookChildNode](../../com.aspose.note/inotebookchildnode)
```
public class Document extends CompositeNode<Page> implements INotebookChildNode
```

Представляет документ Aspose.Note.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [Document()](#Document--) | Инициализирует новый экземпляр класса `Document`. |
| [Document(String filePath)](#Document-java.lang.String-) | Инициализирует новый экземпляр класса `Document`. |
| [Document(String filePath, LoadOptions loadOptions)](#Document-java.lang.String-com.aspose.note.LoadOptions-) | Инициализирует новый экземпляр класса `Document`. |
| [Document(InputStream inStream)](#Document-java.io.InputStream-) | Инициализирует новый экземпляр класса `Document`. |
| [Document(InputStream inStream, LoadOptions loadOptions)](#Document-java.io.InputStream-com.aspose.note.LoadOptions-) | Инициализирует новый экземпляр класса `Document`. |
## Методы

| Метод | Описание |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Принимает посетителя узла. |
| [detectLayoutChanges()](#detectLayoutChanges--) | Обнаруживает все изменения, внесенные в макет документа с момента предыдущего вызова `DetectLayoutChanges`. |
| [getAutomaticLayoutChangesDetectionEnabled()](#getAutomaticLayoutChangesDetectionEnabled--) | Получает значение, указывающее, выполняет ли Aspose.Note автоматическое обнаружение изменений макета. |
| [getColor()](#getColor--) | Получает цвет. |
| [getCreationTime()](#getCreationTime--) | Получает время создания. |
| [getDisplayName()](#getDisplayName--) | Получает отображаемое имя. |
| [getFileFormat()](#getFileFormat--) | Получает формат файла (OneNote 2010, OneNote Online). |
| [getGuid()](#getGuid--) | Получает глобальный уникальный идентификатор объекта. |
| [getGuidInternal()](#getGuidInternal--) |  |
| [getPageHistory(Page page)](#getPageHistory-com.aspose.note.Page-) | Получает `PageHistory`, который содержит полную историю каждой страницы, представленной в документе (самая ранняя имеет индекс 0). |
| [isEncrypted(InputStream stream, Document[] document)](#isEncrypted-java.io.InputStream-com.aspose.note.Document---) | Проверяет, зашифрован ли документ из потока. |
| [isEncrypted(InputStream stream, LoadOptions options, Document[] document)](#isEncrypted-java.io.InputStream-com.aspose.note.LoadOptions-com.aspose.note.Document---) | Проверяет, зашифрован ли документ из потока. |
| [isEncrypted(InputStream stream, String password, Document[] document)](#isEncrypted-java.io.InputStream-java.lang.String-com.aspose.note.Document---) | Проверяет, зашифрован ли документ из потока. |
| [isEncrypted(String filePath, Document[] document)](#isEncrypted-java.lang.String-com.aspose.note.Document---) | Проверяет, зашифрован ли документ из файла. |
| [isEncrypted(String filePath, LoadOptions options, Document[] document)](#isEncrypted-java.lang.String-com.aspose.note.LoadOptions-com.aspose.note.Document---) | Проверяет, зашифрован ли документ из файла. |
| [isEncrypted(String filePath, String password, Document[] document)](#isEncrypted-java.lang.String-java.lang.String-com.aspose.note.Document---) | Проверяет, зашифрован ли документ из файла. |
| [print()](#print--) | Печатает документ с использованием принтера по умолчанию. |
| [print(PrintOptions options)](#print-com.aspose.note.PrintOptions-) | Печатает документ с использованием принтера по умолчанию. |
| [print(String printerName)](#print-java.lang.String-) | Печатает документ с использованием принтера по умолчанию. |
| [print(AttributeSet printSettings)](#print-javax.print.attribute.AttributeSet-) | Печатает документ с использованием принтера по умолчанию. |
| [save(OutputStream stream)](#save-java.io.OutputStream-) | Сохраняет документ OneNote в поток. |
| [save(OutputStream stream, SaveOptions options)](#save-java.io.OutputStream-com.aspose.note.SaveOptions-) | Сохраняет документ OneNote в поток, используя указанные параметры сохранения. |
| [save(OutputStream stream, int format)](#save-java.io.OutputStream-int-) | Сохраняет документ OneNote в поток в указанном формате. |
| [save(String fileName)](#save-java.lang.String-) | Сохраняет документ OneNote в файл. |
| [save(String fileName, SaveOptions options)](#save-java.lang.String-com.aspose.note.SaveOptions-) | Сохраняет документ OneNote в файл, используя указанные параметры сохранения. |
| [save(String fileName, int format)](#save-java.lang.String-int-) | Сохраняет документ OneNote в файл в указанном формате. |
| [setAutomaticLayoutChangesDetectionEnabled(boolean value)](#setAutomaticLayoutChangesDetectionEnabled-boolean-) | Устанавливает значение, указывающее, будет ли Aspose.Note автоматически выполнять обнаружение изменений макета. |
| [setColor(Color value)](#setColor-java.awt.Color-) | Устанавливает цвет. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Устанавливает время создания. |
| [setDisplayName(String value)](#setDisplayName-java.lang.String-) | Устанавливает отображаемое имя. |
### Document() {#Document--}
```
public Document()
```


Инициализирует новый экземпляр класса `Document`. Создаёт пустой документ OneNote.

### Document(String filePath) {#Document-java.lang.String-}
```
public Document(String filePath)
```


Инициализирует новый экземпляр класса `Document`. Открывает существующий документ OneNote из файла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| filePath | java.lang.String | Путь к файлу. |

### Document(String filePath, LoadOptions loadOptions) {#Document-java.lang.String-com.aspose.note.LoadOptions-}
```
public Document(String filePath, LoadOptions loadOptions)
```


Инициализирует новый экземпляр класса `Document`. Открывает существующий документ OneNote из файла. Позволяет указать дополнительные параметры, такие как пароль шифрования.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| filePath | java.lang.String | Путь к файлу. |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | Параметры, используемые для загрузки документа. Может быть null. |

### Document(InputStream inStream) {#Document-java.io.InputStream-}
```
public Document(InputStream inStream)
```


Инициализирует новый экземпляр класса `Document`. Открывает существующий документ OneNote из потока.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| inStream | java.io.InputStream | Поток. |

### Document(InputStream inStream, LoadOptions loadOptions) {#Document-java.io.InputStream-com.aspose.note.LoadOptions-}
```
public Document(InputStream inStream, LoadOptions loadOptions)
```


Инициализирует новый экземпляр класса `Document`. Открывает существующий документ OneNote из потока. Позволяет указать дополнительные параметры, такие как пароль шифрования.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| inStream | java.io.InputStream | Поток. |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | Параметры, используемые для загрузки документа. Может быть null. |

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Принимает посетителя узла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | Объект класса, производного от `DocumentVisitor`. |

### detectLayoutChanges() {#detectLayoutChanges--}
```
public void detectLayoutChanges()
```


Обнаруживает все изменения, внесённые в макет документа с момента предыдущего вызова `DetectLayoutChanges`. Если `AutomaticLayoutChangesDetectionEnabled` установлен в true, используется автоматически в начале экспорта документа.

### getAutomaticLayoutChangesDetectionEnabled() {#getAutomaticLayoutChangesDetectionEnabled--}
```
public boolean getAutomaticLayoutChangesDetectionEnabled()
```


Получает значение, указывающее, будет ли Aspose.Note автоматически выполнять обнаружение изменений макета. Значение по умолчанию — `true`.

**Returns:**
boolean
### getColor() {#getColor--}
```
public Color getColor()
```


Получает цвет.

**Returns:**
java.awt.Color
### getCreationTime() {#getCreationTime--}
```
public Date getCreationTime()
```


Получает время создания.

**Returns:**
java.util.Date
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


Получает отображаемое имя.

**Returns:**
java.lang.String
### getFileFormat() {#getFileFormat--}
```
public int getFileFormat()
```


Получает формат файла (OneNote 2010, OneNote Online).

**Returns:**
int
### getGuid() {#getGuid--}
```
public UUID getGuid()
```


Получает глобальный уникальный идентификатор объекта.

**Returns:**
java.util.UUID
### getGuidInternal() {#getGuidInternal--}
```
public System.Guid getGuidInternal()
```




**Returns:**
com.aspose.ms.System.Guid
### getPageHistory(Page page) {#getPageHistory-com.aspose.note.Page-}
```
public PageHistory getPageHistory(Page page)
```


Получает `PageHistory`, который содержит полную историю каждой страницы, представленной в документе (самая ранняя имеет индекс 0). Текущая версия страницы доступна как `PageHistory.current` и хранится отдельно от коллекции исторических версий.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | Текущая версия страницы. |

**Returns:**
[PageHistory](../../com.aspose.note/pagehistory) - The `PageHistory`.
### isEncrypted(InputStream stream, Document[] document) {#isEncrypted-java.io.InputStream-com.aspose.note.Document---}
```
public static boolean isEncrypted(InputStream stream, Document[] document)
```


Проверяет, зашифрован ли документ из потока. Для проверки необходимо полностью загрузить документ. Поэтому этот метод может привести к потере производительности.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | java.io.InputStream | Поток. |
| document | [Document\[\]](../../com.aspose.note/document) | Загруженный документ. |

**Returns:**
boolean — Возвращает true, если документ зашифрован, иначе false.
### isEncrypted(InputStream stream, LoadOptions options, Document[] document) {#isEncrypted-java.io.InputStream-com.aspose.note.LoadOptions-com.aspose.note.Document---}
```
public static boolean isEncrypted(InputStream stream, LoadOptions options, Document[] document)
```


Проверяет, зашифрован ли документ из потока. Для проверки необходимо полностью загрузить документ. Поэтому этот метод может привести к потере производительности.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | java.io.InputStream | Поток. |
| options | [LoadOptions](../../com.aspose.note/loadoptions) | Параметры загрузки. |
| document | [Document\[\]](../../com.aspose.note/document) | Загруженный документ. |

**Returns:**
boolean — Возвращает true, если документ зашифрован, иначе false.
### isEncrypted(InputStream stream, String password, Document[] document) {#isEncrypted-java.io.InputStream-java.lang.String-com.aspose.note.Document---}
```
public static boolean isEncrypted(InputStream stream, String password, Document[] document)
```


Проверяет, зашифрован ли документ из потока. Для проверки необходимо полностью загрузить документ. Поэтому этот метод может привести к потере производительности.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | java.io.InputStream | Поток. |
| password | java.lang.String | Пароль для расшифровки документа. |
| document | [Document\[\]](../../com.aspose.note/document) | Загруженный документ. |

**Returns:**
boolean — Возвращает true, если документ зашифрован, иначе false.
### isEncrypted(String filePath, Document[] document) {#isEncrypted-java.lang.String-com.aspose.note.Document---}
```
public static boolean isEncrypted(String filePath, Document[] document)
```


Проверяет, зашифрован ли документ из файла. Для проверки необходимо полностью загрузить документ. Поэтому этот метод может привести к потере производительности.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| filePath | java.lang.String | Путь к файлу. |
| document | [Document\[\]](../../com.aspose.note/document) | Загруженный документ. |

**Returns:**
boolean — Возвращает true, если документ зашифрован, иначе false.
### isEncrypted(String filePath, LoadOptions options, Document[] document) {#isEncrypted-java.lang.String-com.aspose.note.LoadOptions-com.aspose.note.Document---}
```
public static boolean isEncrypted(String filePath, LoadOptions options, Document[] document)
```


Проверяет, зашифрован ли документ из файла. Для проверки необходимо полностью загрузить документ. Поэтому этот метод может привести к потере производительности.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| filePath | java.lang.String | Путь к файлу. |
| options | [LoadOptions](../../com.aspose.note/loadoptions) | Параметры загрузки. |
| document | [Document\[\]](../../com.aspose.note/document) | Загруженный документ. |

**Returns:**
boolean — Возвращает true, если документ зашифрован, иначе false.
### isEncrypted(String filePath, String password, Document[] document) {#isEncrypted-java.lang.String-java.lang.String-com.aspose.note.Document---}
```
public static boolean isEncrypted(String filePath, String password, Document[] document)
```


Проверяет, зашифрован ли документ из файла. Для проверки необходимо полностью загрузить документ. Поэтому этот метод может привести к потере производительности.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| filePath | java.lang.String | Путь к файлу. |
| password | java.lang.String | Пароль для расшифровки документа. |
| document | [Document\[\]](../../com.aspose.note/document) | Загруженный документ. |

**Returns:**
boolean — Возвращает true, если документ зашифрован, иначе false.
### print() {#print--}
```
public void print()
```


Печатает документ с использованием принтера по умолчанию.

### print(PrintOptions options) {#print-com.aspose.note.PrintOptions-}
```
public void print(PrintOptions options)
```


Печатает документ с использованием принтера по умолчанию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| options | [PrintOptions](../../com.aspose.note/printoptions) | Параметры, используемые для печати документа. Может быть null. |

### print(String printerName) {#print-java.lang.String-}
```
public void print(String printerName)
```


Печатает документ с использованием принтера по умолчанию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| printerName | java.lang.String |  |

### print(AttributeSet printSettings) {#print-javax.print.attribute.AttributeSet-}
```
public void print(AttributeSet printSettings)
```


Печатает документ с использованием принтера по умолчанию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| printSettings | javax.print.attribute.AttributeSet |  |

### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public void save(OutputStream stream)
```


Сохраняет документ OneNote в поток.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | java.io.OutputStream | Поток System.iO.stream, в котором будет сохранён документ. |

### save(OutputStream stream, SaveOptions options) {#save-java.io.OutputStream-com.aspose.note.SaveOptions-}
```
public void save(OutputStream stream, SaveOptions options)
```


Сохраняет документ OneNote в поток, используя указанные параметры сохранения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | java.io.OutputStream | Поток System.iO.stream, в котором будет сохранён документ. |
| options | [SaveOptions](../../com.aspose.note/saveoptions) | Указывает параметры, как документ сохраняется в поток. |

### save(OutputStream stream, int format) {#save-java.io.OutputStream-int-}
```
public void save(OutputStream stream, int format)
```


Сохраняет документ OneNote в поток в указанном формате.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| поток | java.io.OutputStream | Поток System.iO.stream, в котором будет сохранён документ. |
| format | int | Формат, в котором сохраняется документ. |

### save(String fileName) {#save-java.lang.String-}
```
public void save(String fileName)
```


Сохраняет документ OneNote в файл.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | java.lang.String | Полное имя файла. Если файл с указанным полным именем уже существует, существующий файл будет перезаписан. |

### save(String fileName, SaveOptions options) {#save-java.lang.String-com.aspose.note.SaveOptions-}
```
public void save(String fileName, SaveOptions options)
```


Сохраняет документ OneNote в файл, используя указанные параметры сохранения.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | java.lang.String | Полное имя файла. Если файл с указанным полным именем уже существует, существующий файл будет перезаписан. |
| options | [SaveOptions](../../com.aspose.note/saveoptions) | Указывает параметры, как документ сохраняется в файл. |

### save(String fileName, int format) {#save-java.lang.String-int-}
```
public void save(String fileName, int format)
```


Сохраняет документ OneNote в файл в указанном формате.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fileName | java.lang.String | Полное имя файла. Если файл с указанным полным именем уже существует, существующий файл будет перезаписан. |
| format | int | Формат, в котором сохраняется документ. |

### setAutomaticLayoutChangesDetectionEnabled(boolean value) {#setAutomaticLayoutChangesDetectionEnabled-boolean-}
```
public void setAutomaticLayoutChangesDetectionEnabled(boolean value)
```


Устанавливает значение, указывающее, будет ли Aspose.Note автоматически выполнять обнаружение изменений макета.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | boolean | Новое значение. Может быть null. |

### setColor(Color value) {#setColor-java.awt.Color-}
```
public void setColor(Color value)
```


Устанавливает цвет.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.awt.Color | Значение цвета. |

### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public void setCreationTime(Date value)
```


Устанавливает время создания.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.util.Date | Значение DateTime. |

### setDisplayName(String value) {#setDisplayName-java.lang.String-}
```
public void setDisplayName(String value)
```


Устанавливает отображаемое имя.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.lang.String | Значение DateTime. |

