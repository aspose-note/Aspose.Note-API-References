---
title: "DocumentFontsSubsystem"
second_title: "Référence d'API Aspose.Note pour Java"
description: "Implémentation simple de Aspose.Note.Fonts.FontsSubsystem."
type: docs
weight: 10
url: /fr/java/com.aspose.note.fonts/documentfontssubsystem/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.fonts.FontsSubsystem](../../com.aspose.note.fonts/fontssubsystem)
```
public class DocumentFontsSubsystem extends FontsSubsystem
```

Implémentation simple de Aspose.Note.Fonts.FontsSubsystem. Récupère l'objet FontFamily depuis le système d'exploitation.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [DocumentFontsSubsystem(InputStream defaultFontStream, Map&lt;String,String&gt; fontsSubstitutions)](#DocumentFontsSubsystem-java.io.InputStream-java.util.Map-java.lang.String-java.lang.String--) | Initialise une nouvelle instance de la classe [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem). |
| [DocumentFontsSubsystem(InputStream defaultFontStream)](#DocumentFontsSubsystem-java.io.InputStream-) | Initialise une nouvelle instance de la classe [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem). |
| [DocumentFontsSubsystem(String defaultFontFile, Map&lt;String,String&gt; fontsSubstitutions)](#DocumentFontsSubsystem-java.lang.String-java.util.Map-java.lang.String-java.lang.String--) | Initialise une nouvelle instance de la classe [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem). |
| [DocumentFontsSubsystem(String defaultFontFile)](#DocumentFontsSubsystem-java.lang.String-) | Initialise une nouvelle instance de la classe [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem). |
| [DocumentFontsSubsystem(Map&lt;String,String&gt; fontsSubstitutions)](#DocumentFontsSubsystem-java.util.Map-java.lang.String-java.lang.String--) | Initialise une nouvelle instance de la classe [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem). |
| [DocumentFontsSubsystem()](#DocumentFontsSubsystem--) | Initialise une nouvelle instance de la classe [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem). |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getDefault()](#getDefault--) | Obtient ou définit l'instance statique par défaut. |
| [setDefault(DocumentFontsSubsystem value)](#setDefault-com.aspose.note.fonts.DocumentFontsSubsystem-) | Obtient ou définit l'instance statique par défaut. |
| [usingDefaultFont(String defaultFontName)](#usingDefaultFont-java.lang.String-) | Crée une nouvelle instance de DocumentFontsSubsystem en utilisant le nom de police par défaut spécifié. |
| [usingDefaultFont(String defaultFontName, Map&lt;String,String&gt; fontsSubstitutions)](#usingDefaultFont-java.lang.String-java.util.Map-java.lang.String-java.lang.String--) | Crée une nouvelle instance de DocumentFontsSubsystem en utilisant le nom de police par défaut spécifié. |
| [usingDefaultFontFromFile(String filePath)](#usingDefaultFontFromFile-java.lang.String-) | Crée une nouvelle instance de DocumentFontsSubsystem en utilisant le nom de police par défaut spécifié. |
| [usingDefaultFontFromFile(String filePath, Map&lt;String,String&gt; fontsSubstitutions)](#usingDefaultFontFromFile-java.lang.String-java.util.Map-java.lang.String-java.lang.String--) | Crée une nouvelle instance de DocumentFontsSubsystem en utilisant une police du fichier spécifié comme police par défaut. |
| [usingDefaultFontFromStream(InputStream defaultFontStream)](#usingDefaultFontFromStream-java.io.InputStream-) | Crée une nouvelle instance de DocumentFontsSubsystem en utilisant une police du flux spécifié comme police par défaut. |
| [usingDefaultFontFromStream(InputStream defaultFontStream, Map&lt;String,String&gt; fontsSubstitutions)](#usingDefaultFontFromStream-java.io.InputStream-java.util.Map-java.lang.String-java.lang.String--) | Crée une nouvelle instance de DocumentFontsSubsystem en utilisant une police du flux spécifié comme police par défaut. |
### DocumentFontsSubsystem(InputStream defaultFontStream, Map&lt;String,String&gt; fontsSubstitutions) {#DocumentFontsSubsystem-java.io.InputStream-java.util.Map-java.lang.String-java.lang.String--}
```
public DocumentFontsSubsystem(InputStream defaultFontStream, Map<String,String> fontsSubstitutions)
```


Initialise une nouvelle instance de la classe [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| defaultFontStream | java.io.InputStream | Le flux contenant la police par défaut. |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | Les substitutions de polices. |

### DocumentFontsSubsystem(InputStream defaultFontStream) {#DocumentFontsSubsystem-java.io.InputStream-}
```
public DocumentFontsSubsystem(InputStream defaultFontStream)
```


Initialise une nouvelle instance de la classe [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| defaultFontStream | java.io.InputStream | Le flux contenant la police par défaut. |

### DocumentFontsSubsystem(String defaultFontFile, Map&lt;String,String&gt; fontsSubstitutions) {#DocumentFontsSubsystem-java.lang.String-java.util.Map-java.lang.String-java.lang.String--}
```
public DocumentFontsSubsystem(String defaultFontFile, Map<String,String> fontsSubstitutions)
```


Initialise une nouvelle instance de la classe [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| defaultFontFile | java.lang.String | Le chemin du fichier contenant la police par défaut. |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | Les substitutions de polices. |

### DocumentFontsSubsystem(String defaultFontFile) {#DocumentFontsSubsystem-java.lang.String-}
```
public DocumentFontsSubsystem(String defaultFontFile)
```


Initialise une nouvelle instance de la classe [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| defaultFontFile | java.lang.String | Le chemin du fichier contenant la police par défaut. |

### DocumentFontsSubsystem(Map&lt;String,String&gt; fontsSubstitutions) {#DocumentFontsSubsystem-java.util.Map-java.lang.String-java.lang.String--}
```
public DocumentFontsSubsystem(Map<String,String> fontsSubstitutions)
```


Initialise une nouvelle instance de la classe [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | Les substitutions de polices. |

### DocumentFontsSubsystem() {#DocumentFontsSubsystem--}
```
public DocumentFontsSubsystem()
```


Initialise une nouvelle instance de la classe [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).

### getDefault() {#getDefault--}
```
public static DocumentFontsSubsystem getDefault()
```


Obtient ou définit l'instance statique par défaut.

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem)
### setDefault(DocumentFontsSubsystem value) {#setDefault-com.aspose.note.fonts.DocumentFontsSubsystem-}
```
public static void setDefault(DocumentFontsSubsystem value)
```


Obtient ou définit l'instance statique par défaut.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) |  |

### usingDefaultFont(String defaultFontName) {#usingDefaultFont-java.lang.String-}
```
public static DocumentFontsSubsystem usingDefaultFont(String defaultFontName)
```


Crée une nouvelle instance de DocumentFontsSubsystem en utilisant le nom de police par défaut spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| defaultFontName | java.lang.String | Le nom de police par défaut. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFont(String defaultFontName, Map&lt;String,String&gt; fontsSubstitutions) {#usingDefaultFont-java.lang.String-java.util.Map-java.lang.String-java.lang.String--}
```
public static DocumentFontsSubsystem usingDefaultFont(String defaultFontName, Map<String,String> fontsSubstitutions)
```


Crée une nouvelle instance de DocumentFontsSubsystem en utilisant le nom de police par défaut spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| defaultFontName | java.lang.String | Le nom de police par défaut. |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | Les substitutions de polices. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFontFromFile(String filePath) {#usingDefaultFontFromFile-java.lang.String-}
```
public static DocumentFontsSubsystem usingDefaultFontFromFile(String filePath)
```


Crée une nouvelle instance de DocumentFontsSubsystem en utilisant le nom de police par défaut spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | Le fichier contenant le nom de police par défaut. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFontFromFile(String filePath, Map&lt;String,String&gt; fontsSubstitutions) {#usingDefaultFontFromFile-java.lang.String-java.util.Map-java.lang.String-java.lang.String--}
```
public static DocumentFontsSubsystem usingDefaultFontFromFile(String filePath, Map<String,String> fontsSubstitutions)
```


Crée une nouvelle instance de DocumentFontsSubsystem en utilisant une police du fichier spécifié comme police par défaut.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | Le fichier contenant le nom de police par défaut. |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | Les substitutions de polices. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFontFromStream(InputStream defaultFontStream) {#usingDefaultFontFromStream-java.io.InputStream-}
```
public static DocumentFontsSubsystem usingDefaultFontFromStream(InputStream defaultFontStream)
```


Crée une nouvelle instance de DocumentFontsSubsystem en utilisant une police du flux spécifié comme police par défaut.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| defaultFontStream | java.io.InputStream | Le flux contenant le nom de police par défaut. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFontFromStream(InputStream defaultFontStream, Map&lt;String,String&gt; fontsSubstitutions) {#usingDefaultFontFromStream-java.io.InputStream-java.util.Map-java.lang.String-java.lang.String--}
```
public static DocumentFontsSubsystem usingDefaultFontFromStream(InputStream defaultFontStream, Map<String,String> fontsSubstitutions)
```


Crée une nouvelle instance de DocumentFontsSubsystem en utilisant une police du flux spécifié comme police par défaut.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| defaultFontStream | java.io.InputStream | Le flux contenant le nom de police par défaut. |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | Les substitutions de polices. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
