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
| [addFont(InputStream stream)](#addFont-java.io.InputStream-) | Adds the font. |
| [addFont(String file)](#addFont-java.lang.String-) | Adds the font. |
| [addFontSubstitution(String substituted, String substitution)](#addFontSubstitution-java.lang.String-java.lang.String-) | Adds font substitution. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDefault()](#getDefault--) | Gets or sets the static default instance. |
| [getDefaultFont()](#getDefaultFont--) | Gets default font. |
| [getFontFamily(String fontName)](#getFontFamily-java.lang.String-) | Gets font. |
| [hashCode()](#hashCode--) |  |
| [loadFontsFromFolder(String folder)](#loadFontsFromFolder-java.lang.String-) | Loads all TrueType fonts from specified folder to internal collection. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setDefault(DocumentFontsSubsystem value)](#setDefault-com.aspose.note.fonts.DocumentFontsSubsystem-) | Gets or sets the static default instance. |
| [toString()](#toString--) |  |
| [usingDefaultFont(String defaultFontName)](#usingDefaultFont-java.lang.String-) | Create new DocumentFontsSubsystem instance using specified default font name. |
| [usingDefaultFont(String defaultFontName, Map<String,String> fontsSubstitutions)](#usingDefaultFont-java.lang.String-java.util.Map-java.lang.String-java.lang.String--) | Create new DocumentFontsSubsystem instance using specified default font name. |
| [usingDefaultFontFromFile(String filePath)](#usingDefaultFontFromFile-java.lang.String-) | Create new DocumentFontsSubsystem instance using specified default font name. |
| [usingDefaultFontFromFile(String filePath, Map<String,String> fontsSubstitutions)](#usingDefaultFontFromFile-java.lang.String-java.util.Map-java.lang.String-java.lang.String--) | Create new DocumentFontsSubsystem instance using a font from specified file as default. |
| [usingDefaultFontFromStream(InputStream defaultFontStream)](#usingDefaultFontFromStream-java.io.InputStream-) | Create new DocumentFontsSubsystem instance using a font from specified stream as default. |
| [usingDefaultFontFromStream(InputStream defaultFontStream, Map<String,String> fontsSubstitutions)](#usingDefaultFontFromStream-java.io.InputStream-java.util.Map-java.lang.String-java.lang.String--) | Create new DocumentFontsSubsystem instance using a font from specified stream as default. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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

### addFont(InputStream stream) {#addFont-java.io.InputStream-}
```
public final void addFont(InputStream stream)
```


Adds the font.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | The stream containing the font. |

### addFont(String file) {#addFont-java.lang.String-}
```
public final void addFont(String file)
```


Adds the font.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| file | java.lang.String | The path to the file containing the font. |

### addFontSubstitution(String substituted, String substitution) {#addFontSubstitution-java.lang.String-java.lang.String-}
```
public final void addFontSubstitution(String substituted, String substitution)
```


Adds font substitution.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| substituted | java.lang.String | The substituted font name. |
| substitution | java.lang.String | The substitution font name. |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDefault() {#getDefault--}
```
public static DocumentFontsSubsystem getDefault()
```


Gets or sets the static default instance.

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem)
### getDefaultFont() {#getDefaultFont--}
```
public Font getDefaultFont()
```


Gets default font.

**Returns:**
java.awt.Font
### getFontFamily(String fontName) {#getFontFamily-java.lang.String-}
```
public Font getFontFamily(String fontName)
```


Gets font.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fontName | java.lang.String | The font name. |

**Returns:**
java.awt.Font - The Font.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### loadFontsFromFolder(String folder) {#loadFontsFromFolder-java.lang.String-}
```
public final void loadFontsFromFolder(String folder)
```


Loads all TrueType fonts from specified folder to internal collection.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| folder | java.lang.String | The folder containing fonts. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setDefault(DocumentFontsSubsystem value) {#setDefault-com.aspose.note.fonts.DocumentFontsSubsystem-}
```
public static void setDefault(DocumentFontsSubsystem value)
```


Gets or sets the static default instance.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
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
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final void wait(long arg0)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

