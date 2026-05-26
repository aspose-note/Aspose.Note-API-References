---
title: "DocumentFontsSubsystem"
second_title: "Справочник API Aspose.Note for Java"
description: "Простая реализация Aspose.Note.Fonts.FontsSubsystem."
type: docs
weight: 10
url: /ru/java/com.aspose.note.fonts/documentfontssubsystem/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.fonts.FontsSubsystem](../../com.aspose.note.fonts/fontssubsystem)
```
public class DocumentFontsSubsystem extends FontsSubsystem
```

Простая реализация Aspose.Note.Fonts.FontsSubsystem. Получает объект FontFamily из ОС.
## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [DocumentFontsSubsystem(InputStream defaultFontStream, Map&lt;String,String&gt; fontsSubstitutions)](#DocumentFontsSubsystem-java.io.InputStream-java.util.Map-java.lang.String-java.lang.String--) | Инициализирует новый экземпляр класса [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem). |
| [DocumentFontsSubsystem(InputStream defaultFontStream)](#DocumentFontsSubsystem-java.io.InputStream-) | Инициализирует новый экземпляр класса [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem). |
| [DocumentFontsSubsystem(String defaultFontFile, Map&lt;String,String&gt; fontsSubstitutions)](#DocumentFontsSubsystem-java.lang.String-java.util.Map-java.lang.String-java.lang.String--) | Инициализирует новый экземпляр класса [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem). |
| [DocumentFontsSubsystem(String defaultFontFile)](#DocumentFontsSubsystem-java.lang.String-) | Инициализирует новый экземпляр класса [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem). |
| [DocumentFontsSubsystem(Map&lt;String,String&gt; fontsSubstitutions)](#DocumentFontsSubsystem-java.util.Map-java.lang.String-java.lang.String--) | Инициализирует новый экземпляр класса [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem). |
| [DocumentFontsSubsystem()](#DocumentFontsSubsystem--) | Инициализирует новый экземпляр класса [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem). |
## Методы

| Метод | Описание |
| --- | --- |
| [getDefault()](#getDefault--) | Получает или задает статический экземпляр по умолчанию. |
| [setDefault(DocumentFontsSubsystem value)](#setDefault-com.aspose.note.fonts.DocumentFontsSubsystem-) | Получает или задает статический экземпляр по умолчанию. |
| [usingDefaultFont(String defaultFontName)](#usingDefaultFont-java.lang.String-) | Создайте новый экземпляр DocumentFontsSubsystem, используя указанное имя шрифта по умолчанию. |
| [usingDefaultFont(String defaultFontName, Map&lt;String,String&gt; fontsSubstitutions)](#usingDefaultFont-java.lang.String-java.util.Map-java.lang.String-java.lang.String--) | Создайте новый экземпляр DocumentFontsSubsystem, используя указанное имя шрифта по умолчанию. |
| [usingDefaultFontFromFile(String filePath)](#usingDefaultFontFromFile-java.lang.String-) | Создайте новый экземпляр DocumentFontsSubsystem, используя указанное имя шрифта по умолчанию. |
| [usingDefaultFontFromFile(String filePath, Map&lt;String,String&gt; fontsSubstitutions)](#usingDefaultFontFromFile-java.lang.String-java.util.Map-java.lang.String-java.lang.String--) | Создайте новый экземпляр DocumentFontsSubsystem, используя шрифт из указанного файла в качестве шрифта по умолчанию. |
| [usingDefaultFontFromStream(InputStream defaultFontStream)](#usingDefaultFontFromStream-java.io.InputStream-) | Создайте новый экземпляр DocumentFontsSubsystem, используя шрифт из указанного потока в качестве шрифта по умолчанию. |
| [usingDefaultFontFromStream(InputStream defaultFontStream, Map&lt;String,String&gt; fontsSubstitutions)](#usingDefaultFontFromStream-java.io.InputStream-java.util.Map-java.lang.String-java.lang.String--) | Создайте новый экземпляр DocumentFontsSubsystem, используя шрифт из указанного потока в качестве шрифта по умолчанию. |
### DocumentFontsSubsystem(InputStream defaultFontStream, Map&lt;String,String&gt; fontsSubstitutions) {#DocumentFontsSubsystem-java.io.InputStream-java.util.Map-java.lang.String-java.lang.String--}
```
public DocumentFontsSubsystem(InputStream defaultFontStream, Map<String,String> fontsSubstitutions)
```


Инициализирует новый экземпляр класса [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| defaultFontStream | java.io.InputStream | Поток, содержащий шрифт по умолчанию. |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | Замены шрифтов. |

### DocumentFontsSubsystem(InputStream defaultFontStream) {#DocumentFontsSubsystem-java.io.InputStream-}
```
public DocumentFontsSubsystem(InputStream defaultFontStream)
```


Инициализирует новый экземпляр класса [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| defaultFontStream | java.io.InputStream | Поток, содержащий шрифт по умолчанию. |

### DocumentFontsSubsystem(String defaultFontFile, Map&lt;String,String&gt; fontsSubstitutions) {#DocumentFontsSubsystem-java.lang.String-java.util.Map-java.lang.String-java.lang.String--}
```
public DocumentFontsSubsystem(String defaultFontFile, Map<String,String> fontsSubstitutions)
```


Инициализирует новый экземпляр класса [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| defaultFontFile | java.lang.String | Путь к файлу, содержащему шрифт по умолчанию. |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | Замены шрифтов. |

### DocumentFontsSubsystem(String defaultFontFile) {#DocumentFontsSubsystem-java.lang.String-}
```
public DocumentFontsSubsystem(String defaultFontFile)
```


Инициализирует новый экземпляр класса [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| defaultFontFile | java.lang.String | Путь к файлу, содержащему шрифт по умолчанию. |

### DocumentFontsSubsystem(Map&lt;String,String&gt; fontsSubstitutions) {#DocumentFontsSubsystem-java.util.Map-java.lang.String-java.lang.String--}
```
public DocumentFontsSubsystem(Map<String,String> fontsSubstitutions)
```


Инициализирует новый экземпляр класса [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | Замены шрифтов. |

### DocumentFontsSubsystem() {#DocumentFontsSubsystem--}
```
public DocumentFontsSubsystem()
```


Инициализирует новый экземпляр класса [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).

### getDefault() {#getDefault--}
```
public static DocumentFontsSubsystem getDefault()
```


Получает или задает статический экземпляр по умолчанию.

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem)
### setDefault(DocumentFontsSubsystem value) {#setDefault-com.aspose.note.fonts.DocumentFontsSubsystem-}
```
public static void setDefault(DocumentFontsSubsystem value)
```


Получает или задает статический экземпляр по умолчанию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| value | [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) |  |

### usingDefaultFont(String defaultFontName) {#usingDefaultFont-java.lang.String-}
```
public static DocumentFontsSubsystem usingDefaultFont(String defaultFontName)
```


Создайте новый экземпляр DocumentFontsSubsystem, используя указанное имя шрифта по умолчанию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| defaultFontName | java.lang.String | Имя шрифта по умолчанию. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFont(String defaultFontName, Map&lt;String,String&gt; fontsSubstitutions) {#usingDefaultFont-java.lang.String-java.util.Map-java.lang.String-java.lang.String--}
```
public static DocumentFontsSubsystem usingDefaultFont(String defaultFontName, Map<String,String> fontsSubstitutions)
```


Создайте новый экземпляр DocumentFontsSubsystem, используя указанное имя шрифта по умолчанию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| defaultFontName | java.lang.String | Имя шрифта по умолчанию. |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | Замены шрифтов. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFontFromFile(String filePath) {#usingDefaultFontFromFile-java.lang.String-}
```
public static DocumentFontsSubsystem usingDefaultFontFromFile(String filePath)
```


Создайте новый экземпляр DocumentFontsSubsystem, используя указанное имя шрифта по умолчанию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| filePath | java.lang.String | Файл, содержащий имя шрифта по умолчанию. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFontFromFile(String filePath, Map&lt;String,String&gt; fontsSubstitutions) {#usingDefaultFontFromFile-java.lang.String-java.util.Map-java.lang.String-java.lang.String--}
```
public static DocumentFontsSubsystem usingDefaultFontFromFile(String filePath, Map<String,String> fontsSubstitutions)
```


Создайте новый экземпляр DocumentFontsSubsystem, используя шрифт из указанного файла в качестве шрифта по умолчанию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| filePath | java.lang.String | Файл, содержащий имя шрифта по умолчанию. |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | Замены шрифтов. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFontFromStream(InputStream defaultFontStream) {#usingDefaultFontFromStream-java.io.InputStream-}
```
public static DocumentFontsSubsystem usingDefaultFontFromStream(InputStream defaultFontStream)
```


Создайте новый экземпляр DocumentFontsSubsystem, используя шрифт из указанного потока в качестве шрифта по умолчанию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| defaultFontStream | java.io.InputStream | Поток, содержащий имя шрифта по умолчанию. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFontFromStream(InputStream defaultFontStream, Map&lt;String,String&gt; fontsSubstitutions) {#usingDefaultFontFromStream-java.io.InputStream-java.util.Map-java.lang.String-java.lang.String--}
```
public static DocumentFontsSubsystem usingDefaultFontFromStream(InputStream defaultFontStream, Map<String,String> fontsSubstitutions)
```


Создайте новый экземпляр DocumentFontsSubsystem, используя шрифт из указанного потока в качестве шрифта по умолчанию.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| defaultFontStream | java.io.InputStream | Поток, содержащий имя шрифта по умолчанию. |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | Замены шрифтов. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
