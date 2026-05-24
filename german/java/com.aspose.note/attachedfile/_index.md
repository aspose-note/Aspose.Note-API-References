---
title: "AttachedFile"
second_title: "Aspose.Note für Java API-Referenz"
description: "Stellt eine angehängte Datei dar."
type: docs
weight: 11
url: /de/java/com.aspose.note/attachedfile/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node)

**All Implemented Interfaces:**
[com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode), [com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode), [com.aspose.note.ITaggable](../../com.aspose.note/itaggable)
```
public class AttachedFile extends Node implements IPageChildNode, IOutlineElementChildNode, ITaggable
```

Stellt eine angehängte Datei dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [AttachedFile(String path)](#AttachedFile-java.lang.String-) | Initialisiert eine neue Instanz der `AttachedFile`‑Klasse. |
| [AttachedFile(String path, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)](#AttachedFile-java.lang.String-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-) | Initialisiert eine neue Instanz der `AttachedFile`‑Klasse. |
| [AttachedFile(String fileName, InputStream attachedFileStream)](#AttachedFile-java.lang.String-java.io.InputStream-) | Initialisiert eine neue Instanz der `AttachedFile`‑Klasse. |
| [AttachedFile(String fileName, InputStream attachedFileStream, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)](#AttachedFile-java.lang.String-java.io.InputStream-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-) | Initialisiert eine neue Instanz der `AttachedFile`‑Klasse. |
| [AttachedFile()](#AttachedFile--) | Initialisiert eine neue Instanz der `AttachedFile`‑Klasse. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Akzeptiert den Besucher des Knotens. |
| [getAlignment()](#getAlignment--) | Ruft die Ausrichtung ab. |
| [getAlternativeTextDescription()](#getAlternativeTextDescription--) | Liest oder setzt einen alternativen Textkörper für das Symbol der angehängten Datei. |
| [getAlternativeTextTitle()](#getAlternativeTextTitle--) | Liest oder setzt einen Titel des alternativen Textes für das Symbol der angehängten Datei. |
| [getBytes()](#getBytes--) | Liest die Binärdaten für eine eingebettete Datei. |
| [getExtension()](#getExtension--) | Liest die Erweiterung einer eingebetteten Datei. |
| [getFileName()](#getFileName--) | Liest den Namen der eingebetteten Datei. |
| [getFilePath()](#getFilePath--) | Liest den Pfad zur Originaldatei. |
| [getHeight()](#getHeight--) | Liest die ursprüngliche Höhe des Symbols der eingebetteten Datei. |
| [getHorizontalOffset()](#getHorizontalOffset--) | Liest den horizontalen Versatz. |
| [getIcon()](#getIcon--) | Liest die Binärdaten für das Symbol, das mit der eingebetteten Datei verknüpft ist. |
| [getIconExtension()](#getIconExtension--) | Liest die Erweiterung des Symbols. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Liest die zuletzt geänderte Zeit. |
| [getMaxHeight()](#getMaxHeight--) | Ermittelt die maximale Höhe, um das eingebettete Dateisymbol anzuzeigen. |
| [getMaxWidth()](#getMaxWidth--) | Ermittelt die maximale Breite, um das eingebettete Dateisymbol anzuzeigen. |
| [getParsingErrorInfo()](#getParsingErrorInfo--) | Ermittelt die Daten über den Fehler, der beim Zugriff auf die Datei aufgetreten ist. |
| [getTags()](#getTags--) | Ermittelt die Liste der Tags einer angehängten Datei. |
| [getText()](#getText--) | Ermittelt die Textdarstellung der eingebetteten Datei. |
| [getVerticalOffset()](#getVerticalOffset--) | Ermittelt den vertikalen Versatz. |
| [getWidth()](#getWidth--) | Ermittelt die ursprüngliche Breite des eingebetteten Dateisymbols. |
| [isPrintout()](#isPrintout--) | Ermittelt einen Wert, der angibt, ob die Ansicht der Datei ein Ausdruck ist. |
| [isSizeSetByUser()](#isSizeSetByUser--) | Ermittelt einen Wert, der angibt, ob die Größe des Symbols vom Benutzer explizit aktualisiert wurde. |
| [setAlignment(int value)](#setAlignment-int-) | Legt die Ausrichtung fest. |
| [setAlternativeTextDescription(String value)](#setAlternativeTextDescription-java.lang.String-) | Liest oder setzt einen alternativen Textkörper für das Symbol der angehängten Datei. |
| [setAlternativeTextTitle(String value)](#setAlternativeTextTitle-java.lang.String-) | Liest oder setzt einen Titel des alternativen Textes für das Symbol der angehängten Datei. |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | Legt den horizontalen Versatz fest. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Legt die zuletzt geänderte Zeit fest. |
| [setMaxHeight(float value)](#setMaxHeight-float-) | Legt die maximale Höhe fest, um das eingebettete Dateisymbol anzuzeigen. |
| [setMaxWidth(float value)](#setMaxWidth-float-) | Legt die maximale Breite fest, um das eingebettete Dateisymbol anzuzeigen. |
| [setPrintout(boolean value)](#setPrintout-boolean-) | Legt einen Wert fest, der angibt, ob die Ansicht der Datei ein Ausdruck ist. |
| [setSizeSetByUser(boolean value)](#setSizeSetByUser-boolean-) | Legt einen Wert fest, der angibt, ob die Größe des Symbols vom Benutzer explizit aktualisiert wurde. |
| [setText(String value)](#setText-java.lang.String-) | Legt die Textdarstellung der eingebetteten Datei fest. |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | Legt den vertikalen Versatz fest. |
### AttachedFile(String path) {#AttachedFile-java.lang.String-}
```
public AttachedFile(String path)
```


Initialisiert eine neue Instanz der `AttachedFile`‑Klasse.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Pfad | java.lang.String | Eine Zeichenkette, die den Pfad zur Datei enthält, aus der das `AttachedFile` erstellt werden soll. |

### AttachedFile(String path, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat) {#AttachedFile-java.lang.String-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-}
```
public AttachedFile(String path, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)
```


Initialisiert eine neue Instanz der `AttachedFile`‑Klasse.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Pfad | java.lang.String | Eine Zeichenkette, die den Pfad zur Datei enthält, aus der das `AttachedFile` erstellt werden soll. |
| Symbol | java.io.InputStream | Ein Symbol für die angehängte Datei. |
| Symbolformat | com.aspose.ms.System.Drawing.Imaging.ImageFormat |  |

### AttachedFile(String fileName, InputStream attachedFileStream) {#AttachedFile-java.lang.String-java.io.InputStream-}
```
public AttachedFile(String fileName, InputStream attachedFileStream)
```


Initialisiert eine neue Instanz der `AttachedFile`‑Klasse.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileName | java.lang.String | Ein Name der angehängten Datei. |
| attachedFileStream | java.io.InputStream | Ein Stream, der die Bytes der angehängten Datei enthält. |

### AttachedFile(String fileName, InputStream attachedFileStream, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat) {#AttachedFile-java.lang.String-java.io.InputStream-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-}
```
public AttachedFile(String fileName, InputStream attachedFileStream, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)
```


Initialisiert eine neue Instanz der `AttachedFile`‑Klasse.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileName | java.lang.String | Ein Name der angehängten Datei. |
| attachedFileStream | java.io.InputStream | Ein Stream, der die Bytes der angehängten Datei enthält. |
| Symbol | java.io.InputStream | Ein Symbol für die angehängte Datei. |
| Symbolformat | com.aspose.ms.System.Drawing.Imaging.ImageFormat | Ein Format des Symbols der angehängten Datei. |

### AttachedFile() {#AttachedFile--}
```
public AttachedFile()
```


Initialisiert eine neue Instanz der `AttachedFile`‑Klasse.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Akzeptiert den Besucher des Knotens.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | Das Objekt einer Klasse, die von `DocumentVisitor` abgeleitet ist. |

### getAlignment() {#getAlignment--}
```
public int getAlignment()
```


Ruft die Ausrichtung ab.

**Returns:**
int
### getAlternativeTextDescription() {#getAlternativeTextDescription--}
```
public final String getAlternativeTextDescription()
```


Liest oder setzt einen alternativen Textkörper für das Symbol der angehängten Datei.

**Returns:**
java.lang.String
### getAlternativeTextTitle() {#getAlternativeTextTitle--}
```
public final String getAlternativeTextTitle()
```


Liest oder setzt einen Titel des alternativen Textes für das Symbol der angehängten Datei.

**Returns:**
java.lang.String
### getBytes() {#getBytes--}
```
public byte[] getBytes()
```


Liest die Binärdaten für eine eingebettete Datei.

**Returns:**
byte[]
### getExtension() {#getExtension--}
```
public String getExtension()
```


Liest die Erweiterung einer eingebetteten Datei.

**Returns:**
java.lang.String
### getFileName() {#getFileName--}
```
public String getFileName()
```


Liest den Namen der eingebetteten Datei.

**Returns:**
java.lang.String
### getFilePath() {#getFilePath--}
```
public String getFilePath()
```


Liest den Pfad zur Originaldatei.

**Returns:**
java.lang.String
### getHeight() {#getHeight--}
```
public float getHeight()
```


Liest die ursprüngliche Höhe des Symbols der eingebetteten Datei.

**Returns:**
float
### getHorizontalOffset() {#getHorizontalOffset--}
```
public float getHorizontalOffset()
```


Liest den horizontalen Versatz.

**Returns:**
float
### getIcon() {#getIcon--}
```
public byte[] getIcon()
```


Liest die Binärdaten für das Symbol, das mit der eingebetteten Datei verknüpft ist.

**Returns:**
byte[]
### getIconExtension() {#getIconExtension--}
```
public String getIconExtension()
```


Liest die Erweiterung des Symbols.

**Returns:**
java.lang.String
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Liest die zuletzt geänderte Zeit.

**Returns:**
java.util.Date
### getMaxHeight() {#getMaxHeight--}
```
public float getMaxHeight()
```


Ermittelt die maximale Höhe, um das eingebettete Dateisymbol anzuzeigen.

**Returns:**
float
### getMaxWidth() {#getMaxWidth--}
```
public float getMaxWidth()
```


Ermittelt die maximale Breite, um das eingebettete Dateisymbol anzuzeigen.

**Returns:**
float
### getParsingErrorInfo() {#getParsingErrorInfo--}
```
public final ParsingErrorInfo getParsingErrorInfo()
```


Ermittelt die Daten über den Fehler, der beim Zugriff auf die Datei aufgetreten ist.

**Returns:**
[ParsingErrorInfo](../../com.aspose.note.infrastructure/parsingerrorinfo)
### getTags() {#getTags--}
```
public final System.Collections.Generic.List<ITag> getTags()
```


Ermittelt die Liste der Tags einer angehängten Datei.

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.note.ITag&gt;
### getText() {#getText--}
```
public String getText()
```


Liefert die Textdarstellung der eingebetteten Datei. Der String DARF KEINE Zeichen mit dem Wert 10 (Zeilenumbruch) oder 13 (Wagenrücklauf) enthalten.

**Returns:**
java.lang.String
### getVerticalOffset() {#getVerticalOffset--}
```
public float getVerticalOffset()
```


Ermittelt den vertikalen Versatz.

**Returns:**
float
### getWidth() {#getWidth--}
```
public float getWidth()
```


Ermittelt die ursprüngliche Breite des eingebetteten Dateisymbols.

**Returns:**
float
### isPrintout() {#isPrintout--}
```
public boolean isPrintout()
```


Ermittelt einen Wert, der angibt, ob die Ansicht der Datei ein Ausdruck ist.

**Returns:**
boolean
### isSizeSetByUser() {#isSizeSetByUser--}
```
public boolean isSizeSetByUser()
```


Ermittelt einen Wert, der angibt, ob die Größe des Symbols vom Benutzer explizit aktualisiert wurde.

**Returns:**
boolean
### setAlignment(int value) {#setAlignment-int-}
```
public void setAlignment(int value)
```


Legt die Ausrichtung fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | Wert von Alignment. |

### setAlternativeTextDescription(String value) {#setAlternativeTextDescription-java.lang.String-}
```
public final void setAlternativeTextDescription(String value)
```


Liest oder setzt einen alternativen Textkörper für das Symbol der angehängten Datei.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setAlternativeTextTitle(String value) {#setAlternativeTextTitle-java.lang.String-}
```
public final void setAlternativeTextTitle(String value)
```


Liest oder setzt einen Titel des alternativen Textes für das Symbol der angehängten Datei.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public void setHorizontalOffset(float value)
```


Legt den horizontalen Versatz fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | float | Wert von Offsets. |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Legt die zuletzt geänderte Zeit fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.Date | Wert von Date. |

### setMaxHeight(float value) {#setMaxHeight-float-}
```
public void setMaxHeight(float value)
```


Legt die maximale Höhe fest, um das eingebettete Dateisymbol anzuzeigen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | float | Wert der maximalen Höhe. |

### setMaxWidth(float value) {#setMaxWidth-float-}
```
public void setMaxWidth(float value)
```


Legt die maximale Breite fest, um das eingebettete Dateisymbol anzuzeigen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | float | Wert der maximalen Breite. |

### setPrintout(boolean value) {#setPrintout-boolean-}
```
public void setPrintout(boolean value)
```


Legt einen Wert fest, der angibt, ob die Ansicht der Datei ein Ausdruck ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | Neuer Wert. |

### setSizeSetByUser(boolean value) {#setSizeSetByUser-boolean-}
```
public void setSizeSetByUser(boolean value)
```


Legt einen Wert fest, der angibt, ob die Größe des Symbols vom Benutzer explizit aktualisiert wurde.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | Neuer Wert. |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Setzt die Textdarstellung der eingebetteten Datei. Der String DARF KEINE Zeichen mit dem Wert 10 (Zeilenumbruch) oder 13 (Wagenrücklauf) enthalten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | Wert von Text. |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public void setVerticalOffset(float value)
```


Legt den vertikalen Versatz fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | float | Wert von Offset. |

