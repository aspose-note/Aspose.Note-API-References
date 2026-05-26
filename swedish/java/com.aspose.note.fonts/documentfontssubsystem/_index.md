---
title: "DocumentFontsSubsystem"
second_title: "Aspose.Note for Java API-referens"
description: "Enkel implementation av Aspose.Note.Fonts.FontsSubsystem."
type: docs
weight: 10
url: /sv/java/com.aspose.note.fonts/documentfontssubsystem/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.fonts.FontsSubsystem](../../com.aspose.note.fonts/fontssubsystem)
```
public class DocumentFontsSubsystem extends FontsSubsystem
```

Enkel implementation av Aspose.Note.Fonts.FontsSubsystem. Hämtar FontFamily-objekt från OS.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [DocumentFontsSubsystem(InputStream defaultFontStream, Map&lt;String,String&gt; fontsSubstitutions)](#DocumentFontsSubsystem-java.io.InputStream-java.util.Map-java.lang.String-java.lang.String--) | Initierar en ny instans av klassen [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem). |
| [DocumentFontsSubsystem(InputStream defaultFontStream)](#DocumentFontsSubsystem-java.io.InputStream-) | Initierar en ny instans av klassen [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem). |
| [DocumentFontsSubsystem(String defaultFontFile, Map&lt;String,String&gt; fontsSubstitutions)](#DocumentFontsSubsystem-java.lang.String-java.util.Map-java.lang.String-java.lang.String--) | Initierar en ny instans av klassen [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem). |
| [DocumentFontsSubsystem(String defaultFontFile)](#DocumentFontsSubsystem-java.lang.String-) | Initierar en ny instans av klassen [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem). |
| [DocumentFontsSubsystem(Map&lt;String,String&gt; fontsSubstitutions)](#DocumentFontsSubsystem-java.util.Map-java.lang.String-java.lang.String--) | Initierar en ny instans av klassen [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem). |
| [DocumentFontsSubsystem()](#DocumentFontsSubsystem--) | Initierar en ny instans av klassen [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem). |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getDefault()](#getDefault--) | Hämtar eller anger den statiska standardinstansen. |
| [setDefault(DocumentFontsSubsystem value)](#setDefault-com.aspose.note.fonts.DocumentFontsSubsystem-) | Hämtar eller anger den statiska standardinstansen. |
| [usingDefaultFont(String defaultFontName)](#usingDefaultFont-java.lang.String-) | Skapa en ny DocumentFontsSubsystem-instans med angivet standardfontnamn. |
| [usingDefaultFont(String defaultFontName, Map&lt;String,String&gt; fontsSubstitutions)](#usingDefaultFont-java.lang.String-java.util.Map-java.lang.String-java.lang.String--) | Skapa en ny DocumentFontsSubsystem-instans med angivet standardfontnamn. |
| [usingDefaultFontFromFile(String filePath)](#usingDefaultFontFromFile-java.lang.String-) | Skapa en ny DocumentFontsSubsystem-instans med angivet standardfontnamn. |
| [usingDefaultFontFromFile(String filePath, Map&lt;String,String&gt; fontsSubstitutions)](#usingDefaultFontFromFile-java.lang.String-java.util.Map-java.lang.String-java.lang.String--) | Skapa en ny DocumentFontsSubsystem-instans med ett font från angiven fil som standard. |
| [usingDefaultFontFromStream(InputStream defaultFontStream)](#usingDefaultFontFromStream-java.io.InputStream-) | Skapa en ny DocumentFontsSubsystem-instans med ett font från angiven ström som standard. |
| [usingDefaultFontFromStream(InputStream defaultFontStream, Map&lt;String,String&gt; fontsSubstitutions)](#usingDefaultFontFromStream-java.io.InputStream-java.util.Map-java.lang.String-java.lang.String--) | Skapa en ny DocumentFontsSubsystem-instans med ett font från angiven ström som standard. |
### DocumentFontsSubsystem(InputStream defaultFontStream, Map&lt;String,String&gt; fontsSubstitutions) {#DocumentFontsSubsystem-java.io.InputStream-java.util.Map-java.lang.String-java.lang.String--}
```
public DocumentFontsSubsystem(InputStream defaultFontStream, Map<String,String> fontsSubstitutions)
```


Initierar en ny instans av klassen [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| defaultFontStream | java.io.InputStream | Strömmen som innehåller standard Font. |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | Fontsubstitutionerna. |

### DocumentFontsSubsystem(InputStream defaultFontStream) {#DocumentFontsSubsystem-java.io.InputStream-}
```
public DocumentFontsSubsystem(InputStream defaultFontStream)
```


Initierar en ny instans av klassen [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| defaultFontStream | java.io.InputStream | Strömmen som innehåller standard Font. |

### DocumentFontsSubsystem(String defaultFontFile, Map&lt;String,String&gt; fontsSubstitutions) {#DocumentFontsSubsystem-java.lang.String-java.util.Map-java.lang.String-java.lang.String--}
```
public DocumentFontsSubsystem(String defaultFontFile, Map<String,String> fontsSubstitutions)
```


Initierar en ny instans av klassen [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| defaultFontFile | java.lang.String | Sökvägen till filen som innehåller standard Font. |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | Fontsubstitutionerna. |

### DocumentFontsSubsystem(String defaultFontFile) {#DocumentFontsSubsystem-java.lang.String-}
```
public DocumentFontsSubsystem(String defaultFontFile)
```


Initierar en ny instans av klassen [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| defaultFontFile | java.lang.String | Sökvägen till filen som innehåller standard Font. |

### DocumentFontsSubsystem(Map&lt;String,String&gt; fontsSubstitutions) {#DocumentFontsSubsystem-java.util.Map-java.lang.String-java.lang.String--}
```
public DocumentFontsSubsystem(Map<String,String> fontsSubstitutions)
```


Initierar en ny instans av klassen [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | Fontsubstitutionerna. |

### DocumentFontsSubsystem() {#DocumentFontsSubsystem--}
```
public DocumentFontsSubsystem()
```


Initierar en ny instans av klassen [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).

### getDefault() {#getDefault--}
```
public static DocumentFontsSubsystem getDefault()
```


Hämtar eller anger den statiska standardinstansen.

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem)
### setDefault(DocumentFontsSubsystem value) {#setDefault-com.aspose.note.fonts.DocumentFontsSubsystem-}
```
public static void setDefault(DocumentFontsSubsystem value)
```


Hämtar eller anger den statiska standardinstansen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) |  |

### usingDefaultFont(String defaultFontName) {#usingDefaultFont-java.lang.String-}
```
public static DocumentFontsSubsystem usingDefaultFont(String defaultFontName)
```


Skapa en ny DocumentFontsSubsystem-instans med angivet standardfontnamn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| defaultFontName | java.lang.String | Standardfontnamnet. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFont(String defaultFontName, Map&lt;String,String&gt; fontsSubstitutions) {#usingDefaultFont-java.lang.String-java.util.Map-java.lang.String-java.lang.String--}
```
public static DocumentFontsSubsystem usingDefaultFont(String defaultFontName, Map<String,String> fontsSubstitutions)
```


Skapa en ny DocumentFontsSubsystem-instans med angivet standardfontnamn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| defaultFontName | java.lang.String | Standardfontnamnet. |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | Fontsubstitutionerna. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFontFromFile(String filePath) {#usingDefaultFontFromFile-java.lang.String-}
```
public static DocumentFontsSubsystem usingDefaultFontFromFile(String filePath)
```


Skapa en ny DocumentFontsSubsystem-instans med angivet standardfontnamn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filePath | java.lang.String | Filen som innehåller standardfontnamnet. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFontFromFile(String filePath, Map&lt;String,String&gt; fontsSubstitutions) {#usingDefaultFontFromFile-java.lang.String-java.util.Map-java.lang.String-java.lang.String--}
```
public static DocumentFontsSubsystem usingDefaultFontFromFile(String filePath, Map<String,String> fontsSubstitutions)
```


Skapa en ny DocumentFontsSubsystem-instans med ett font från angiven fil som standard.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| filePath | java.lang.String | Filen som innehåller standardfontnamnet. |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | Fontsubstitutionerna. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFontFromStream(InputStream defaultFontStream) {#usingDefaultFontFromStream-java.io.InputStream-}
```
public static DocumentFontsSubsystem usingDefaultFontFromStream(InputStream defaultFontStream)
```


Skapa en ny DocumentFontsSubsystem-instans med ett font från angiven ström som standard.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| defaultFontStream | java.io.InputStream | Strömmen som innehåller standardfontnamnet. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFontFromStream(InputStream defaultFontStream, Map&lt;String,String&gt; fontsSubstitutions) {#usingDefaultFontFromStream-java.io.InputStream-java.util.Map-java.lang.String-java.lang.String--}
```
public static DocumentFontsSubsystem usingDefaultFontFromStream(InputStream defaultFontStream, Map<String,String> fontsSubstitutions)
```


Skapa en ny DocumentFontsSubsystem-instans med ett font från angiven ström som standard.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| defaultFontStream | java.io.InputStream | Strömmen som innehåller standardfontnamnet. |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | Fontsubstitutionerna. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
