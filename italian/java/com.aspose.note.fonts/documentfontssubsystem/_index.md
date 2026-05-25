---
title: "DocumentFontsSubsystem"
second_title: "Riferimento API di Aspose.Note per Java"
description: "Implementazione semplice di Aspose.Note.Fonts.FontsSubsystem."
type: docs
weight: 10
url: /it/java/com.aspose.note.fonts/documentfontssubsystem/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.fonts.FontsSubsystem](../../com.aspose.note.fonts/fontssubsystem)
```
public class DocumentFontsSubsystem extends FontsSubsystem
```

Implementazione semplice di Aspose.Note.Fonts.FontsSubsystem. Recupera l'oggetto FontFamily dal sistema operativo.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [DocumentFontsSubsystem(InputStream defaultFontStream, Map&lt;String,String&gt; fontsSubstitutions)](#DocumentFontsSubsystem-java.io.InputStream-java.util.Map-java.lang.String-java.lang.String--) | Inizializza una nuova istanza della classe [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem). |
| [DocumentFontsSubsystem(InputStream defaultFontStream)](#DocumentFontsSubsystem-java.io.InputStream-) | Inizializza una nuova istanza della classe [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem). |
| [DocumentFontsSubsystem(String defaultFontFile, Map&lt;String,String&gt; fontsSubstitutions)](#DocumentFontsSubsystem-java.lang.String-java.util.Map-java.lang.String-java.lang.String--) | Inizializza una nuova istanza della classe [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem). |
| [DocumentFontsSubsystem(String defaultFontFile)](#DocumentFontsSubsystem-java.lang.String-) | Inizializza una nuova istanza della classe [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem). |
| [DocumentFontsSubsystem(Map&lt;String,String&gt; fontsSubstitutions)](#DocumentFontsSubsystem-java.util.Map-java.lang.String-java.lang.String--) | Inizializza una nuova istanza della classe [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem). |
| [DocumentFontsSubsystem()](#DocumentFontsSubsystem--) | Inizializza una nuova istanza della classe [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem). |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getDefault()](#getDefault--) | Ottiene o imposta l'istanza predefinita statica. |
| [setDefault(DocumentFontsSubsystem value)](#setDefault-com.aspose.note.fonts.DocumentFontsSubsystem-) | Ottiene o imposta l'istanza predefinita statica. |
| [usingDefaultFont(String defaultFontName)](#usingDefaultFont-java.lang.String-) | Crea una nuova istanza di DocumentFontsSubsystem utilizzando il nome del carattere predefinito specificato. |
| [usingDefaultFont(String defaultFontName, Map&lt;String,String&gt; fontsSubstitutions)](#usingDefaultFont-java.lang.String-java.util.Map-java.lang.String-java.lang.String--) | Crea una nuova istanza di DocumentFontsSubsystem utilizzando il nome del carattere predefinito specificato. |
| [usingDefaultFontFromFile(String filePath)](#usingDefaultFontFromFile-java.lang.String-) | Crea una nuova istanza di DocumentFontsSubsystem utilizzando il nome del carattere predefinito specificato. |
| [usingDefaultFontFromFile(String filePath, Map&lt;String,String&gt; fontsSubstitutions)](#usingDefaultFontFromFile-java.lang.String-java.util.Map-java.lang.String-java.lang.String--) | Crea una nuova istanza di DocumentFontsSubsystem utilizzando un carattere dal file specificato come predefinito. |
| [usingDefaultFontFromStream(InputStream defaultFontStream)](#usingDefaultFontFromStream-java.io.InputStream-) | Crea una nuova istanza di DocumentFontsSubsystem utilizzando un carattere dallo stream specificato come predefinito. |
| [usingDefaultFontFromStream(InputStream defaultFontStream, Map&lt;String,String&gt; fontsSubstitutions)](#usingDefaultFontFromStream-java.io.InputStream-java.util.Map-java.lang.String-java.lang.String--) | Crea una nuova istanza di DocumentFontsSubsystem utilizzando un carattere dallo stream specificato come predefinito. |
### DocumentFontsSubsystem(InputStream defaultFontStream, Map&lt;String,String&gt; fontsSubstitutions) {#DocumentFontsSubsystem-java.io.InputStream-java.util.Map-java.lang.String-java.lang.String--}
```
public DocumentFontsSubsystem(InputStream defaultFontStream, Map<String,String> fontsSubstitutions)
```


Inizializza una nuova istanza della classe [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| defaultFontStream | java.io.InputStream | Lo stream contenente il Font predefinito. |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | Le sostituzioni dei caratteri. |

### DocumentFontsSubsystem(InputStream defaultFontStream) {#DocumentFontsSubsystem-java.io.InputStream-}
```
public DocumentFontsSubsystem(InputStream defaultFontStream)
```


Inizializza una nuova istanza della classe [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| defaultFontStream | java.io.InputStream | Lo stream contenente il Font predefinito. |

### DocumentFontsSubsystem(String defaultFontFile, Map&lt;String,String&gt; fontsSubstitutions) {#DocumentFontsSubsystem-java.lang.String-java.util.Map-java.lang.String-java.lang.String--}
```
public DocumentFontsSubsystem(String defaultFontFile, Map<String,String> fontsSubstitutions)
```


Inizializza una nuova istanza della classe [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| defaultFontFile | java.lang.String | Il percorso al file che contiene il Font predefinito. |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | Le sostituzioni dei caratteri. |

### DocumentFontsSubsystem(String defaultFontFile) {#DocumentFontsSubsystem-java.lang.String-}
```
public DocumentFontsSubsystem(String defaultFontFile)
```


Inizializza una nuova istanza della classe [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| defaultFontFile | java.lang.String | Il percorso al file che contiene il Font predefinito. |

### DocumentFontsSubsystem(Map&lt;String,String&gt; fontsSubstitutions) {#DocumentFontsSubsystem-java.util.Map-java.lang.String-java.lang.String--}
```
public DocumentFontsSubsystem(Map<String,String> fontsSubstitutions)
```


Inizializza una nuova istanza della classe [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | Le sostituzioni dei caratteri. |

### DocumentFontsSubsystem() {#DocumentFontsSubsystem--}
```
public DocumentFontsSubsystem()
```


Inizializza una nuova istanza della classe [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).

### getDefault() {#getDefault--}
```
public static DocumentFontsSubsystem getDefault()
```


Ottiene o imposta l'istanza predefinita statica.

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem)
### setDefault(DocumentFontsSubsystem value) {#setDefault-com.aspose.note.fonts.DocumentFontsSubsystem-}
```
public static void setDefault(DocumentFontsSubsystem value)
```


Ottiene o imposta l'istanza predefinita statica.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) |  |

### usingDefaultFont(String defaultFontName) {#usingDefaultFont-java.lang.String-}
```
public static DocumentFontsSubsystem usingDefaultFont(String defaultFontName)
```


Crea una nuova istanza di DocumentFontsSubsystem utilizzando il nome del carattere predefinito specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| defaultFontName | java.lang.String | Il nome del carattere predefinito. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFont(String defaultFontName, Map&lt;String,String&gt; fontsSubstitutions) {#usingDefaultFont-java.lang.String-java.util.Map-java.lang.String-java.lang.String--}
```
public static DocumentFontsSubsystem usingDefaultFont(String defaultFontName, Map<String,String> fontsSubstitutions)
```


Crea una nuova istanza di DocumentFontsSubsystem utilizzando il nome del carattere predefinito specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| defaultFontName | java.lang.String | Il nome del carattere predefinito. |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | Le sostituzioni dei caratteri. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFontFromFile(String filePath) {#usingDefaultFontFromFile-java.lang.String-}
```
public static DocumentFontsSubsystem usingDefaultFontFromFile(String filePath)
```


Crea una nuova istanza di DocumentFontsSubsystem utilizzando il nome del carattere predefinito specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| filePath | java.lang.String | Il file che contiene il nome del carattere predefinito. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFontFromFile(String filePath, Map&lt;String,String&gt; fontsSubstitutions) {#usingDefaultFontFromFile-java.lang.String-java.util.Map-java.lang.String-java.lang.String--}
```
public static DocumentFontsSubsystem usingDefaultFontFromFile(String filePath, Map<String,String> fontsSubstitutions)
```


Crea una nuova istanza di DocumentFontsSubsystem utilizzando un carattere dal file specificato come predefinito.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| filePath | java.lang.String | Il file che contiene il nome del carattere predefinito. |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | Le sostituzioni dei caratteri. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFontFromStream(InputStream defaultFontStream) {#usingDefaultFontFromStream-java.io.InputStream-}
```
public static DocumentFontsSubsystem usingDefaultFontFromStream(InputStream defaultFontStream)
```


Crea una nuova istanza di DocumentFontsSubsystem utilizzando un carattere dallo stream specificato come predefinito.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| defaultFontStream | java.io.InputStream | Lo stream che contiene il nome del carattere predefinito. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFontFromStream(InputStream defaultFontStream, Map&lt;String,String&gt; fontsSubstitutions) {#usingDefaultFontFromStream-java.io.InputStream-java.util.Map-java.lang.String-java.lang.String--}
```
public static DocumentFontsSubsystem usingDefaultFontFromStream(InputStream defaultFontStream, Map<String,String> fontsSubstitutions)
```


Crea una nuova istanza di DocumentFontsSubsystem utilizzando un carattere dallo stream specificato come predefinito.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| defaultFontStream | java.io.InputStream | Lo stream che contiene il nome del carattere predefinito. |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | Le sostituzioni dei caratteri. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
