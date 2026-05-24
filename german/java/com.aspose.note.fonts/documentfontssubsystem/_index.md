---
title: "DocumentFontsSubsystem"
second_title: "Aspose.Note für Java API-Referenz"
description: "Einfache Implementierung von Aspose.Note.Fonts.FontsSubsystem."
type: docs
weight: 10
url: /de/java/com.aspose.note.fonts/documentfontssubsystem/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.fonts.FontsSubsystem](../../com.aspose.note.fonts/fontssubsystem)
```
public class DocumentFontsSubsystem extends FontsSubsystem
```

Einfache Implementierung von Aspose.Note.Fonts.FontsSubsystem. Ruft das FontFamily-Objekt vom Betriebssystem ab.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [DocumentFontsSubsystem(InputStream defaultFontStream, Map&lt;String,String&gt; fontsSubstitutions)](#DocumentFontsSubsystem-java.io.InputStream-java.util.Map-java.lang.String-java.lang.String--) | Initialisiert eine neue Instanz der Klasse [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem). |
| [DocumentFontsSubsystem(InputStream defaultFontStream)](#DocumentFontsSubsystem-java.io.InputStream-) | Initialisiert eine neue Instanz der Klasse [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem). |
| [DocumentFontsSubsystem(String defaultFontFile, Map&lt;String,String&gt; fontsSubstitutions)](#DocumentFontsSubsystem-java.lang.String-java.util.Map-java.lang.String-java.lang.String--) | Initialisiert eine neue Instanz der Klasse [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem). |
| [DocumentFontsSubsystem(String defaultFontFile)](#DocumentFontsSubsystem-java.lang.String-) | Initialisiert eine neue Instanz der Klasse [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem). |
| [DocumentFontsSubsystem(Map&lt;String,String&gt; fontsSubstitutions)](#DocumentFontsSubsystem-java.util.Map-java.lang.String-java.lang.String--) | Initialisiert eine neue Instanz der Klasse [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem). |
| [DocumentFontsSubsystem()](#DocumentFontsSubsystem--) | Initialisiert eine neue Instanz der Klasse [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem). |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getDefault()](#getDefault--) | Liest oder setzt die statische Standardinstanz. |
| [setDefault(DocumentFontsSubsystem value)](#setDefault-com.aspose.note.fonts.DocumentFontsSubsystem-) | Liest oder setzt die statische Standardinstanz. |
| [usingDefaultFont(String defaultFontName)](#usingDefaultFont-java.lang.String-) | Erstelle eine neue DocumentFontsSubsystem-Instanz mit dem angegebenen Standard‑Schriftartnamen. |
| [usingDefaultFont(String defaultFontName, Map&lt;String,String&gt; fontsSubstitutions)](#usingDefaultFont-java.lang.String-java.util.Map-java.lang.String-java.lang.String--) | Erstelle eine neue DocumentFontsSubsystem-Instanz mit dem angegebenen Standard‑Schriftartnamen. |
| [usingDefaultFontFromFile(String filePath)](#usingDefaultFontFromFile-java.lang.String-) | Erstelle eine neue DocumentFontsSubsystem-Instanz mit dem angegebenen Standard‑Schriftartnamen. |
| [usingDefaultFontFromFile(String filePath, Map&lt;String,String&gt; fontsSubstitutions)](#usingDefaultFontFromFile-java.lang.String-java.util.Map-java.lang.String-java.lang.String--) | Erstelle eine neue DocumentFontsSubsystem-Instanz mit einer Schriftart aus der angegebenen Datei als Standard. |
| [usingDefaultFontFromStream(InputStream defaultFontStream)](#usingDefaultFontFromStream-java.io.InputStream-) | Erstelle eine neue DocumentFontsSubsystem-Instanz mit einer Schriftart aus dem angegebenen Stream als Standard. |
| [usingDefaultFontFromStream(InputStream defaultFontStream, Map&lt;String,String&gt; fontsSubstitutions)](#usingDefaultFontFromStream-java.io.InputStream-java.util.Map-java.lang.String-java.lang.String--) | Erstelle eine neue DocumentFontsSubsystem-Instanz mit einer Schriftart aus dem angegebenen Stream als Standard. |
### DocumentFontsSubsystem(InputStream defaultFontStream, Map&lt;String,String&gt; fontsSubstitutions) {#DocumentFontsSubsystem-java.io.InputStream-java.util.Map-java.lang.String-java.lang.String--}
```
public DocumentFontsSubsystem(InputStream defaultFontStream, Map<String,String> fontsSubstitutions)
```


Initialisiert eine neue Instanz der Klasse [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| defaultFontStream | java.io.InputStream | Der Stream, der die Standard‑Font enthält. |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | Die Schriftarten‑Ersetzungen. |

### DocumentFontsSubsystem(InputStream defaultFontStream) {#DocumentFontsSubsystem-java.io.InputStream-}
```
public DocumentFontsSubsystem(InputStream defaultFontStream)
```


Initialisiert eine neue Instanz der Klasse [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| defaultFontStream | java.io.InputStream | Der Stream, der die Standard‑Font enthält. |

### DocumentFontsSubsystem(String defaultFontFile, Map&lt;String,String&gt; fontsSubstitutions) {#DocumentFontsSubsystem-java.lang.String-java.util.Map-java.lang.String-java.lang.String--}
```
public DocumentFontsSubsystem(String defaultFontFile, Map<String,String> fontsSubstitutions)
```


Initialisiert eine neue Instanz der Klasse [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| defaultFontFile | java.lang.String | Der Pfad zur Datei, die die Standard‑Font enthält. |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | Die Schriftarten‑Ersetzungen. |

### DocumentFontsSubsystem(String defaultFontFile) {#DocumentFontsSubsystem-java.lang.String-}
```
public DocumentFontsSubsystem(String defaultFontFile)
```


Initialisiert eine neue Instanz der Klasse [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| defaultFontFile | java.lang.String | Der Pfad zur Datei, die die Standard‑Font enthält. |

### DocumentFontsSubsystem(Map&lt;String,String&gt; fontsSubstitutions) {#DocumentFontsSubsystem-java.util.Map-java.lang.String-java.lang.String--}
```
public DocumentFontsSubsystem(Map<String,String> fontsSubstitutions)
```


Initialisiert eine neue Instanz der Klasse [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | Die Schriftarten‑Ersetzungen. |

### DocumentFontsSubsystem() {#DocumentFontsSubsystem--}
```
public DocumentFontsSubsystem()
```


Initialisiert eine neue Instanz der Klasse [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).

### getDefault() {#getDefault--}
```
public static DocumentFontsSubsystem getDefault()
```


Liest oder setzt die statische Standardinstanz.

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem)
### setDefault(DocumentFontsSubsystem value) {#setDefault-com.aspose.note.fonts.DocumentFontsSubsystem-}
```
public static void setDefault(DocumentFontsSubsystem value)
```


Liest oder setzt die statische Standardinstanz.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) |  |

### usingDefaultFont(String defaultFontName) {#usingDefaultFont-java.lang.String-}
```
public static DocumentFontsSubsystem usingDefaultFont(String defaultFontName)
```


Erstelle eine neue DocumentFontsSubsystem-Instanz mit dem angegebenen Standard‑Schriftartnamen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| defaultFontName | java.lang.String | Der Standard‑Schriftartname. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFont(String defaultFontName, Map&lt;String,String&gt; fontsSubstitutions) {#usingDefaultFont-java.lang.String-java.util.Map-java.lang.String-java.lang.String--}
```
public static DocumentFontsSubsystem usingDefaultFont(String defaultFontName, Map<String,String> fontsSubstitutions)
```


Erstelle eine neue DocumentFontsSubsystem-Instanz mit dem angegebenen Standard‑Schriftartnamen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| defaultFontName | java.lang.String | Der Standard‑Schriftartname. |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | Die Schriftarten‑Ersetzungen. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFontFromFile(String filePath) {#usingDefaultFontFromFile-java.lang.String-}
```
public static DocumentFontsSubsystem usingDefaultFontFromFile(String filePath)
```


Erstelle eine neue DocumentFontsSubsystem-Instanz mit dem angegebenen Standard‑Schriftartnamen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| filePath | java.lang.String | Die Datei, die den Standard‑Schriftartnamen enthält. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFontFromFile(String filePath, Map&lt;String,String&gt; fontsSubstitutions) {#usingDefaultFontFromFile-java.lang.String-java.util.Map-java.lang.String-java.lang.String--}
```
public static DocumentFontsSubsystem usingDefaultFontFromFile(String filePath, Map<String,String> fontsSubstitutions)
```


Erstelle eine neue DocumentFontsSubsystem-Instanz mit einer Schriftart aus der angegebenen Datei als Standard.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| filePath | java.lang.String | Die Datei, die den Standard‑Schriftartnamen enthält. |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | Die Schriftarten‑Ersetzungen. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFontFromStream(InputStream defaultFontStream) {#usingDefaultFontFromStream-java.io.InputStream-}
```
public static DocumentFontsSubsystem usingDefaultFontFromStream(InputStream defaultFontStream)
```


Erstelle eine neue DocumentFontsSubsystem-Instanz mit einer Schriftart aus dem angegebenen Stream als Standard.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| defaultFontStream | java.io.InputStream | Der Stream, der den Standard‑Schriftartnamen enthält. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFontFromStream(InputStream defaultFontStream, Map&lt;String,String&gt; fontsSubstitutions) {#usingDefaultFontFromStream-java.io.InputStream-java.util.Map-java.lang.String-java.lang.String--}
```
public static DocumentFontsSubsystem usingDefaultFontFromStream(InputStream defaultFontStream, Map<String,String> fontsSubstitutions)
```


Erstelle eine neue DocumentFontsSubsystem-Instanz mit einer Schriftart aus dem angegebenen Stream als Standard.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| defaultFontStream | java.io.InputStream | Der Stream, der den Standard‑Schriftartnamen enthält. |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | Die Schriftarten‑Ersetzungen. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
