---
title: "DocumentFontsSubsystem"
second_title: "Referencia de API de Aspose.Note para Java"
description: "Implementación simple de Aspose.Note.Fonts.FontsSubsystem."
type: docs
weight: 10
url: /es/java/com.aspose.note.fonts/documentfontssubsystem/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.fonts.FontsSubsystem](../../com.aspose.note.fonts/fontssubsystem)
```
public class DocumentFontsSubsystem extends FontsSubsystem
```

Implementación simple de Aspose.Note.Fonts.FontsSubsystem. Recupera el objeto FontFamily del SO.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [DocumentFontsSubsystem(InputStream defaultFontStream, Map&lt;String,String&gt; fontsSubstitutions)](#DocumentFontsSubsystem-java.io.InputStream-java.util.Map-java.lang.String-java.lang.String--) | Inicializa una nueva instancia de la clase [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem). |
| [DocumentFontsSubsystem(InputStream defaultFontStream)](#DocumentFontsSubsystem-java.io.InputStream-) | Inicializa una nueva instancia de la clase [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem). |
| [DocumentFontsSubsystem(String defaultFontFile, Map&lt;String,String&gt; fontsSubstitutions)](#DocumentFontsSubsystem-java.lang.String-java.util.Map-java.lang.String-java.lang.String--) | Inicializa una nueva instancia de la clase [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem). |
| [DocumentFontsSubsystem(String defaultFontFile)](#DocumentFontsSubsystem-java.lang.String-) | Inicializa una nueva instancia de la clase [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem). |
| [DocumentFontsSubsystem(Map&lt;String,String&gt; fontsSubstitutions)](#DocumentFontsSubsystem-java.util.Map-java.lang.String-java.lang.String--) | Inicializa una nueva instancia de la clase [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem). |
| [DocumentFontsSubsystem()](#DocumentFontsSubsystem--) | Inicializa una nueva instancia de la clase [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem). |
## Métodos

| Método | Descripción |
| --- | --- |
| [getDefault()](#getDefault--) | Obtiene o establece la instancia predeterminada estática. |
| [setDefault(DocumentFontsSubsystem value)](#setDefault-com.aspose.note.fonts.DocumentFontsSubsystem-) | Obtiene o establece la instancia predeterminada estática. |
| [usingDefaultFont(String defaultFontName)](#usingDefaultFont-java.lang.String-) | Crea una nueva instancia de DocumentFontsSubsystem usando el nombre de fuente predeterminado especificado. |
| [usingDefaultFont(String defaultFontName, Map&lt;String,String&gt; fontsSubstitutions)](#usingDefaultFont-java.lang.String-java.util.Map-java.lang.String-java.lang.String--) | Crea una nueva instancia de DocumentFontsSubsystem usando el nombre de fuente predeterminado especificado. |
| [usingDefaultFontFromFile(String filePath)](#usingDefaultFontFromFile-java.lang.String-) | Crea una nueva instancia de DocumentFontsSubsystem usando el nombre de fuente predeterminado especificado. |
| [usingDefaultFontFromFile(String filePath, Map&lt;String,String&gt; fontsSubstitutions)](#usingDefaultFontFromFile-java.lang.String-java.util.Map-java.lang.String-java.lang.String--) | Crea una nueva instancia de DocumentFontsSubsystem usando una fuente del archivo especificado como predeterminada. |
| [usingDefaultFontFromStream(InputStream defaultFontStream)](#usingDefaultFontFromStream-java.io.InputStream-) | Crea una nueva instancia de DocumentFontsSubsystem usando una fuente del flujo especificado como predeterminada. |
| [usingDefaultFontFromStream(InputStream defaultFontStream, Map&lt;String,String&gt; fontsSubstitutions)](#usingDefaultFontFromStream-java.io.InputStream-java.util.Map-java.lang.String-java.lang.String--) | Crea una nueva instancia de DocumentFontsSubsystem usando una fuente del flujo especificado como predeterminada. |
### DocumentFontsSubsystem(InputStream defaultFontStream, Map&lt;String,String&gt; fontsSubstitutions) {#DocumentFontsSubsystem-java.io.InputStream-java.util.Map-java.lang.String-java.lang.String--}
```
public DocumentFontsSubsystem(InputStream defaultFontStream, Map<String,String> fontsSubstitutions)
```


Inicializa una nueva instancia de la clase [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| defaultFontStream | java.io.InputStream | El flujo que contiene la Font predeterminada. |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | Las sustituciones de fuentes. |

### DocumentFontsSubsystem(InputStream defaultFontStream) {#DocumentFontsSubsystem-java.io.InputStream-}
```
public DocumentFontsSubsystem(InputStream defaultFontStream)
```


Inicializa una nueva instancia de la clase [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| defaultFontStream | java.io.InputStream | El flujo que contiene la Font predeterminada. |

### DocumentFontsSubsystem(String defaultFontFile, Map&lt;String,String&gt; fontsSubstitutions) {#DocumentFontsSubsystem-java.lang.String-java.util.Map-java.lang.String-java.lang.String--}
```
public DocumentFontsSubsystem(String defaultFontFile, Map<String,String> fontsSubstitutions)
```


Inicializa una nueva instancia de la clase [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| defaultFontFile | java.lang.String | La ruta al archivo que contiene la Font predeterminada. |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | Las sustituciones de fuentes. |

### DocumentFontsSubsystem(String defaultFontFile) {#DocumentFontsSubsystem-java.lang.String-}
```
public DocumentFontsSubsystem(String defaultFontFile)
```


Inicializa una nueva instancia de la clase [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| defaultFontFile | java.lang.String | La ruta al archivo que contiene la Font predeterminada. |

### DocumentFontsSubsystem(Map&lt;String,String&gt; fontsSubstitutions) {#DocumentFontsSubsystem-java.util.Map-java.lang.String-java.lang.String--}
```
public DocumentFontsSubsystem(Map<String,String> fontsSubstitutions)
```


Inicializa una nueva instancia de la clase [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | Las sustituciones de fuentes. |

### DocumentFontsSubsystem() {#DocumentFontsSubsystem--}
```
public DocumentFontsSubsystem()
```


Inicializa una nueva instancia de la clase [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).

### getDefault() {#getDefault--}
```
public static DocumentFontsSubsystem getDefault()
```


Obtiene o establece la instancia predeterminada estática.

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem)
### setDefault(DocumentFontsSubsystem value) {#setDefault-com.aspose.note.fonts.DocumentFontsSubsystem-}
```
public static void setDefault(DocumentFontsSubsystem value)
```


Obtiene o establece la instancia predeterminada estática.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) |  |

### usingDefaultFont(String defaultFontName) {#usingDefaultFont-java.lang.String-}
```
public static DocumentFontsSubsystem usingDefaultFont(String defaultFontName)
```


Crea una nueva instancia de DocumentFontsSubsystem usando el nombre de fuente predeterminado especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| defaultFontName | java.lang.String | El nombre de la fuente predeterminada. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFont(String defaultFontName, Map&lt;String,String&gt; fontsSubstitutions) {#usingDefaultFont-java.lang.String-java.util.Map-java.lang.String-java.lang.String--}
```
public static DocumentFontsSubsystem usingDefaultFont(String defaultFontName, Map<String,String> fontsSubstitutions)
```


Crea una nueva instancia de DocumentFontsSubsystem usando el nombre de fuente predeterminado especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| defaultFontName | java.lang.String | El nombre de la fuente predeterminada. |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | Las sustituciones de fuentes. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFontFromFile(String filePath) {#usingDefaultFontFromFile-java.lang.String-}
```
public static DocumentFontsSubsystem usingDefaultFontFromFile(String filePath)
```


Crea una nueva instancia de DocumentFontsSubsystem usando el nombre de fuente predeterminado especificado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| filePath | java.lang.String | El archivo que contiene el nombre de la fuente predeterminada. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFontFromFile(String filePath, Map&lt;String,String&gt; fontsSubstitutions) {#usingDefaultFontFromFile-java.lang.String-java.util.Map-java.lang.String-java.lang.String--}
```
public static DocumentFontsSubsystem usingDefaultFontFromFile(String filePath, Map<String,String> fontsSubstitutions)
```


Crea una nueva instancia de DocumentFontsSubsystem usando una fuente del archivo especificado como predeterminada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| filePath | java.lang.String | El archivo que contiene el nombre de la fuente predeterminada. |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | Las sustituciones de fuentes. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFontFromStream(InputStream defaultFontStream) {#usingDefaultFontFromStream-java.io.InputStream-}
```
public static DocumentFontsSubsystem usingDefaultFontFromStream(InputStream defaultFontStream)
```


Crea una nueva instancia de DocumentFontsSubsystem usando una fuente del flujo especificado como predeterminada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| defaultFontStream | java.io.InputStream | El flujo que contiene el nombre de la fuente predeterminada. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFontFromStream(InputStream defaultFontStream, Map&lt;String,String&gt; fontsSubstitutions) {#usingDefaultFontFromStream-java.io.InputStream-java.util.Map-java.lang.String-java.lang.String--}
```
public static DocumentFontsSubsystem usingDefaultFontFromStream(InputStream defaultFontStream, Map<String,String> fontsSubstitutions)
```


Crea una nueva instancia de DocumentFontsSubsystem usando una fuente del flujo especificado como predeterminada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| defaultFontStream | java.io.InputStream | El flujo que contiene el nombre de la fuente predeterminada. |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | Las sustituciones de fuentes. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
