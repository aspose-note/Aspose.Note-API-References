---
title: DocumentFontsSubsystem
second_title: Aspose.Note for Java API Reference
description: Simple implementation of Aspose.Note.Fonts.FontsSubsystem.
type: docs
weight: 10
url: /java/com.aspose.note.fonts/documentfontssubsystem/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.fonts.FontsSubsystem](../../com.aspose.note.fonts/fontssubsystem)
```
public class DocumentFontsSubsystem extends FontsSubsystem
```

Simple implementation of Aspose.Note.Fonts.FontsSubsystem. Retrieves FontFamily object from OS.
## Constructors

| Constructor | Description |
| --- | --- |
| [DocumentFontsSubsystem(InputStream defaultFontStream, Map<String,String> fontsSubstitutions)](#DocumentFontsSubsystem-java.io.InputStream-java.util.Map-java.lang.String-java.lang.String--) | Initializes a new instance of the [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) class. |
| [DocumentFontsSubsystem(InputStream defaultFontStream)](#DocumentFontsSubsystem-java.io.InputStream-) | Initializes a new instance of the [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) class. |
| [DocumentFontsSubsystem(String defaultFontFile, Map<String,String> fontsSubstitutions)](#DocumentFontsSubsystem-java.lang.String-java.util.Map-java.lang.String-java.lang.String--) | Initializes a new instance of the [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) class. |
| [DocumentFontsSubsystem(String defaultFontFile)](#DocumentFontsSubsystem-java.lang.String-) | Initializes a new instance of the [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) class. |
| [DocumentFontsSubsystem(Map<String,String> fontsSubstitutions)](#DocumentFontsSubsystem-java.util.Map-java.lang.String-java.lang.String--) | Initializes a new instance of the [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) class. |
| [DocumentFontsSubsystem()](#DocumentFontsSubsystem--) | Initializes a new instance of the [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) class. |
## Methods

| Method | Description |
| --- | --- |
| [usingDefaultFont(String defaultFontName, Map<String,String> fontsSubstitutions)](#usingDefaultFont-java.lang.String-java.util.Map-java.lang.String-java.lang.String--) | Create new DocumentFontsSubsystem instance using specified default font name. |
| [usingDefaultFont(String defaultFontName)](#usingDefaultFont-java.lang.String-) | Create new DocumentFontsSubsystem instance using specified default font name. |
| [usingDefaultFontFromFile(String filePath, Map<String,String> fontsSubstitutions)](#usingDefaultFontFromFile-java.lang.String-java.util.Map-java.lang.String-java.lang.String--) | Create new DocumentFontsSubsystem instance using a font from specified file as default. |
| [usingDefaultFontFromFile(String filePath)](#usingDefaultFontFromFile-java.lang.String-) | Create new DocumentFontsSubsystem instance using specified default font name. |
| [usingDefaultFontFromStream(InputStream defaultFontStream, Map<String,String> fontsSubstitutions)](#usingDefaultFontFromStream-java.io.InputStream-java.util.Map-java.lang.String-java.lang.String--) | Create new DocumentFontsSubsystem instance using a font from specified stream as default. |
| [usingDefaultFontFromStream(InputStream defaultFontStream)](#usingDefaultFontFromStream-java.io.InputStream-) | Create new DocumentFontsSubsystem instance using a font from specified stream as default. |
| [getDefault()](#getDefault--) | Gets or sets the static default instance. |
| [setDefault(DocumentFontsSubsystem value)](#setDefault-com.aspose.note.fonts.DocumentFontsSubsystem-) | Gets or sets the static default instance. |
### DocumentFontsSubsystem(InputStream defaultFontStream, Map<String,String> fontsSubstitutions) {#DocumentFontsSubsystem-java.io.InputStream-java.util.Map-java.lang.String-java.lang.String--}
```
public DocumentFontsSubsystem(InputStream defaultFontStream, Map<String,String> fontsSubstitutions)
```


Initializes a new instance of the [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| defaultFontStream | java.io.InputStream | The stream containing default Font. |
| fontsSubstitutions | java.util.Map<java.lang.String,java.lang.String> | The fonts substitutions. |

### DocumentFontsSubsystem(InputStream defaultFontStream) {#DocumentFontsSubsystem-java.io.InputStream-}
```
public DocumentFontsSubsystem(InputStream defaultFontStream)
```


Initializes a new instance of the [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| defaultFontStream | java.io.InputStream | The stream containing default Font. |

### DocumentFontsSubsystem(String defaultFontFile, Map<String,String> fontsSubstitutions) {#DocumentFontsSubsystem-java.lang.String-java.util.Map-java.lang.String-java.lang.String--}
```
public DocumentFontsSubsystem(String defaultFontFile, Map<String,String> fontsSubstitutions)
```


Initializes a new instance of the [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| defaultFontFile | java.lang.String | The path to the file containing default Font. |
| fontsSubstitutions | java.util.Map<java.lang.String,java.lang.String> | The fonts substitutions. |

### DocumentFontsSubsystem(String defaultFontFile) {#DocumentFontsSubsystem-java.lang.String-}
```
public DocumentFontsSubsystem(String defaultFontFile)
```


Initializes a new instance of the [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| defaultFontFile | java.lang.String | The path to the file containing default Font. |

### DocumentFontsSubsystem(Map<String,String> fontsSubstitutions) {#DocumentFontsSubsystem-java.util.Map-java.lang.String-java.lang.String--}
```
public DocumentFontsSubsystem(Map<String,String> fontsSubstitutions)
```


Initializes a new instance of the [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fontsSubstitutions | java.util.Map<java.lang.String,java.lang.String> | The fonts substitutions. |

### DocumentFontsSubsystem() {#DocumentFontsSubsystem--}
```
public DocumentFontsSubsystem()
```


Initializes a new instance of the [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) class.

### usingDefaultFont(String defaultFontName, Map<String,String> fontsSubstitutions) {#usingDefaultFont-java.lang.String-java.util.Map-java.lang.String-java.lang.String--}
```
public static DocumentFontsSubsystem usingDefaultFont(String defaultFontName, Map<String,String> fontsSubstitutions)
```


Create new DocumentFontsSubsystem instance using specified default font name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| defaultFontName | java.lang.String | The default font name. |
| fontsSubstitutions | java.util.Map<java.lang.String,java.lang.String> | The fonts substitutions. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFont(String defaultFontName) {#usingDefaultFont-java.lang.String-}
```
public static DocumentFontsSubsystem usingDefaultFont(String defaultFontName)
```


Create new DocumentFontsSubsystem instance using specified default font name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| defaultFontName | java.lang.String | The default font name. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFontFromFile(String filePath, Map<String,String> fontsSubstitutions) {#usingDefaultFontFromFile-java.lang.String-java.util.Map-java.lang.String-java.lang.String--}
```
public static DocumentFontsSubsystem usingDefaultFontFromFile(String filePath, Map<String,String> fontsSubstitutions)
```


Create new DocumentFontsSubsystem instance using a font from specified file as default.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | The file containing default font name. |
| fontsSubstitutions | java.util.Map<java.lang.String,java.lang.String> | The fonts substitutions. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFontFromFile(String filePath) {#usingDefaultFontFromFile-java.lang.String-}
```
public static DocumentFontsSubsystem usingDefaultFontFromFile(String filePath)
```


Create new DocumentFontsSubsystem instance using specified default font name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | The file containing default font name. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFontFromStream(InputStream defaultFontStream, Map<String,String> fontsSubstitutions) {#usingDefaultFontFromStream-java.io.InputStream-java.util.Map-java.lang.String-java.lang.String--}
```
public static DocumentFontsSubsystem usingDefaultFontFromStream(InputStream defaultFontStream, Map<String,String> fontsSubstitutions)
```


Create new DocumentFontsSubsystem instance using a font from specified stream as default.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| defaultFontStream | java.io.InputStream | The stream containing the default font name. |
| fontsSubstitutions | java.util.Map<java.lang.String,java.lang.String> | The fonts substitutions. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFontFromStream(InputStream defaultFontStream) {#usingDefaultFontFromStream-java.io.InputStream-}
```
public static DocumentFontsSubsystem usingDefaultFontFromStream(InputStream defaultFontStream)
```


Create new DocumentFontsSubsystem instance using a font from specified stream as default.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| defaultFontStream | java.io.InputStream | The stream containing the default font name. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### getDefault() {#getDefault--}
```
public static DocumentFontsSubsystem getDefault()
```


Gets or sets the static default instance.

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem)
### setDefault(DocumentFontsSubsystem value) {#setDefault-com.aspose.note.fonts.DocumentFontsSubsystem-}
```
public static void setDefault(DocumentFontsSubsystem value)
```


Gets or sets the static default instance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) |  |

