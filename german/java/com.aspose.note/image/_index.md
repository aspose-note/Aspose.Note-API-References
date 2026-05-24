---
title: "Bild"
second_title: "Aspose.Note für Java API-Referenz"
description: "Stellt ein Bild dar."
type: docs
weight: 33
url: /de/java/com.aspose.note/image/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode

**All Implemented Interfaces:**
[com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode), [com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode), [com.aspose.note.ITaggable](../../com.aspose.note/itaggable)
```
public final class Image extends CompositeNode<Loop> implements IPageChildNode, IOutlineElementChildNode, ITaggable
```

Stellt ein Bild dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [Image(String path)](#Image-java.lang.String-) | Initialisiert eine neue Instanz der `Image`-Klasse. |
| [Image(String fileName, InputStream imageStream)](#Image-java.lang.String-java.io.InputStream-) | Initialisiert eine neue Instanz der `Image`-Klasse. |
| [Image()](#Image--) | Initialisiert eine neue Instanz der `Image`-Klasse. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Akzeptiert den Besucher des Knotens. |
| [getAlignment()](#getAlignment--) | Ruft die Ausrichtung ab. |
| [getAlternativeTextDescription()](#getAlternativeTextDescription--) | Liest einen Body-Alternativtext für das Bild. |
| [getAlternativeTextTitle()](#getAlternativeTextTitle--) | Liest einen Titel des Alternativtexts für das Bild. |
| [getBytes()](#getBytes--) | Liest den Bild-Datenspeicher. |
| [getFileName()](#getFileName--) | Liest den Dateinamen. |
| [getFilePath()](#getFilePath--) | Liest den Pfad zur Bilddatei. |
| [getFormat()](#getFormat--) | Liest das Format des Bildes. |
| [getHeight()](#getHeight--) | Liest die Höhe. |
| [getHorizontalOffset()](#getHorizontalOffset--) | Liest den horizontalen Versatz. |
| [getHyperlinkUrl()](#getHyperlinkUrl--) | Liest den mit dem Bild verknüpften Hyperlink. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Ruft die zuletzt geänderte Zeit ab. |
| [getOriginalHeight()](#getOriginalHeight--) | Liest die ursprüngliche Höhe. |
| [getOriginalWidth()](#getOriginalWidth--) | Liest die ursprüngliche Breite. |
| [getTags()](#getTags--) | Liest die Liste aller Tags eines Bildes. |
| [getVerticalOffset()](#getVerticalOffset--) | Ermittelt den vertikalen Versatz. |
| [getWidth()](#getWidth--) | Liest die Breite. |
| [isBackground()](#isBackground--) | Liest, ob das Bild ein Hintergrundbild ist. |
| [replace(Image newImage)](#replace-com.aspose.note.Image-) | Ersetzt die aktuellen Bilddaten durch die Daten des bereitgestellten Image-Objekts. |
| [setAlignment(int value)](#setAlignment-int-) | Legt die Ausrichtung fest. |
| [setAlternativeTextDescription(String value)](#setAlternativeTextDescription-java.lang.String-) | Legt einen Body-Alternativtext für das Bild fest. |
| [setAlternativeTextTitle(String value)](#setAlternativeTextTitle-java.lang.String-) | Legt einen Titel des Alternativtexts für das Bild fest. |
| [setBackground(boolean value)](#setBackground-boolean-) | Liest, ob das Bild ein Hintergrundbild ist. |
| [setHeight(float value)](#setHeight-float-) | Legt die Höhe fest. |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | Legt den horizontalen Versatz fest. |
| [setHyperlinkUrl(String value)](#setHyperlinkUrl-java.lang.String-) | Legt den mit dem Bild verknüpften Hyperlink fest. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Setzt die letzte Änderungszeit. |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | Legt den vertikalen Versatz fest. |
| [setWidth(float value)](#setWidth-float-) | Legt die Breite fest. |
### Image(String path) {#Image-java.lang.String-}
```
public Image(String path)
```


Initialisiert eine neue Instanz der `Image`-Klasse.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Pfad | java.lang.String | Eine Zeichenkette, die den Pfad zur Datei enthält, aus der das `Image` erstellt werden soll. |

### Image(String fileName, InputStream imageStream) {#Image-java.lang.String-java.io.InputStream-}
```
public Image(String fileName, InputStream imageStream)
```


Initialisiert eine neue Instanz der `Image`-Klasse.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileName | java.lang.String | Ein Name des Bildes. |
| imageStream | java.io.InputStream | Ein Stream, der das Bild enthält. |

### Image() {#Image--}
```
public Image()
```


Initialisiert eine neue Instanz der `Image`-Klasse.

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


Liest einen Body-Alternativtext für das Bild.

**Returns:**
java.lang.String
### getAlternativeTextTitle() {#getAlternativeTextTitle--}
```
public final String getAlternativeTextTitle()
```


Liest einen Titel des Alternativtexts für das Bild.

**Returns:**
java.lang.String
### getBytes() {#getBytes--}
```
public byte[] getBytes()
```


Liest den Bild-Datenspeicher.

**Returns:**
byte[]
### getFileName() {#getFileName--}
```
public String getFileName()
```


Liest den Dateinamen.

**Returns:**
java.lang.String
### getFilePath() {#getFilePath--}
```
public String getFilePath()
```


Liest den Pfad zur Bilddatei.

**Returns:**
java.lang.String
### getFormat() {#getFormat--}
```
public final System.Drawing.Imaging.ImageFormat getFormat()
```


Liest das Format des Bildes.

**Returns:**
com.aspose.ms.System.Drawing.Imaging.ImageFormat
### getHeight() {#getHeight--}
```
public final float getHeight()
```


Liefert die Höhe. Dies ist die tatsächliche Höhe des Bildes im MS OneNote-Dokument.

**Returns:**
float
### getHorizontalOffset() {#getHorizontalOffset--}
```
public float getHorizontalOffset()
```


Liest den horizontalen Versatz.

**Returns:**
float
### getHyperlinkUrl() {#getHyperlinkUrl--}
```
public String getHyperlinkUrl()
```


Liest den mit dem Bild verknüpften Hyperlink.

**Returns:**
java.lang.String
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Ruft die zuletzt geänderte Zeit ab.

**Returns:**
java.util.Date
### getOriginalHeight() {#getOriginalHeight--}
```
public float getOriginalHeight()
```


Liefert die ursprüngliche Höhe. Dies ist die ursprüngliche Breite des Bildes, bevor es skaliert wird.

**Returns:**
float
### getOriginalWidth() {#getOriginalWidth--}
```
public float getOriginalWidth()
```


Liefert die ursprüngliche Breite. Dies ist die ursprüngliche Breite des Bildes, bevor es skaliert wird.

**Returns:**
float
### getTags() {#getTags--}
```
public final System.Collections.Generic.List<ITag> getTags()
```


Liest die Liste aller Tags eines Bildes.

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.note.ITag&gt;
### getVerticalOffset() {#getVerticalOffset--}
```
public float getVerticalOffset()
```


Ermittelt den vertikalen Versatz.

**Returns:**
float
### getWidth() {#getWidth--}
```
public final float getWidth()
```


Liefert die Breite. Dies ist die tatsächliche Breite des Bildes im MS OneNote-Dokument.

**Returns:**
float
### isBackground() {#isBackground--}
```
public final boolean isBackground()
```


Liest, ob das Bild ein Hintergrundbild ist.

**Returns:**
boolean
### replace(Image newImage) {#replace-com.aspose.note.Image-}
```
public void replace(Image newImage)
```


Ersetzt die aktuellen Bilddaten durch die Daten des bereitgestellten Image-Objekts.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| newImage | [Image](../../com.aspose.note/image) |  |

### setAlignment(int value) {#setAlignment-int-}
```
public void setAlignment(int value)
```


Legt die Ausrichtung fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setAlternativeTextDescription(String value) {#setAlternativeTextDescription-java.lang.String-}
```
public final void setAlternativeTextDescription(String value)
```


Legt einen Body-Alternativtext für das Bild fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setAlternativeTextTitle(String value) {#setAlternativeTextTitle-java.lang.String-}
```
public final void setAlternativeTextTitle(String value)
```


Legt einen Titel des Alternativtexts für das Bild fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setBackground(boolean value) {#setBackground-boolean-}
```
public final void setBackground(boolean value)
```


Liest, ob das Bild ein Hintergrundbild ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setHeight(float value) {#setHeight-float-}
```
public final void setHeight(float value)
```


Setzt die Höhe. Dies ist die tatsächliche Höhe des Bildes im MS OneNote-Dokument.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | float |  |

### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public void setHorizontalOffset(float value)
```


Legt den horizontalen Versatz fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | float |  |

### setHyperlinkUrl(String value) {#setHyperlinkUrl-java.lang.String-}
```
public void setHyperlinkUrl(String value)
```


Legt den mit dem Bild verknüpften Hyperlink fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Setzt die letzte Änderungszeit.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.Date |  |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public void setVerticalOffset(float value)
```


Legt den vertikalen Versatz fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | float |  |

### setWidth(float value) {#setWidth-float-}
```
public final void setWidth(float value)
```


Setzt die Breite. Dies ist die tatsächliche Breite des Bildes im MS OneNote-Dokument.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | float |  |

