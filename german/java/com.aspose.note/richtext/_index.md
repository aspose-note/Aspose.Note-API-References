---
title: "RichText"
second_title: "Aspose.Note für Java API-Referenz"
description: "Stellt einen Rich-Text dar."
type: docs
weight: 82
url: /de/java/com.aspose.note/richtext/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node)

**All Implemented Interfaces:**
[com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode), [com.aspose.note.ITaggable](../../com.aspose.note/itaggable), com.aspose.ms.System.Collections.Generic.IGenericEnumerable
```
public class RichText extends Node implements IOutlineElementChildNode, ITaggable, System.Collections.Generic.IGenericEnumerable<Character>
```

Stellt einen Rich-Text dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [RichText()](#RichText--) | Initialisiert eine neue Instanz der Klasse [RichText](../../com.aspose.note/richtext). |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Akzeptiert den Besucher des Knotens. |
| [append(String value)](#append-java.lang.String-) | Fügt einen String zum letzten Textbereich hinzu. |
| [append(String value, TextStyle style)](#append-java.lang.String-com.aspose.note.TextStyle-) | Fügt einen String am Ende hinzu. |
| [appendFront(String value)](#appendFront-java.lang.String-) | Fügt einen String am Anfang des ersten Textbereichs hinzu. |
| [appendFront(String value, TextStyle style)](#appendFront-java.lang.String-com.aspose.note.TextStyle-) | Fügt einen String am Anfang hinzu. |
| [clear()](#clear--) | Löscht den Inhalt dieser Instanz. |
| [getAlignment()](#getAlignment--) | Ruft die Ausrichtung ab. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Liest die zuletzt geänderte Zeit. |
| [getLength()](#getLength--) |  |
| [getLineSpacing()](#getLineSpacing--) | Ermittelt den Zeilenabstand. |
| [getParagraphStyle()](#getParagraphStyle--) | Ermittelt den Absatzstil. |
| [getSpaceAfter()](#getSpaceAfter--) | Ermittelt den minimalen Abstand nach. |
| [getSpaceBefore()](#getSpaceBefore--) | Ermittelt den minimalen Abstand vor. |
| [getStyles()](#getStyles--) | Ermittelt die Stile. |
| [getTags()](#getTags--) | Ermittelt die Liste aller Tags eines Absatzes. |
| [getText()](#getText--) | Ermittelt den Text. |
| [getTextRuns()](#getTextRuns--) |  |
| [indexOf(char value)](#indexOf-char-) | Gibt den nullbasierten Index des ersten Vorkommens des angegebenen Unicode-Zeichens in diesem String zurück. |
| [indexOf(char value, int startIndex)](#indexOf-char-int-) | Gibt den nullbasierten Index des ersten Vorkommens des angegebenen Unicode-Zeichens in diesem String zurück. |
| [indexOf(char value, int startIndex, int count)](#indexOf-char-int-int-) | Gibt den nullbasierten Index des ersten Vorkommens des angegebenen Zeichens in dieser Instanz zurück. |
| [indexOf(String value)](#indexOf-java.lang.String-) | Gibt den nullbasierten Index des ersten Vorkommens der angegebenen Zeichenkette in dieser Instanz zurück. |
| [indexOf(String value, int startIndex)](#indexOf-java.lang.String-int-) | Gibt den nullbasierten Index des ersten Vorkommens der angegebenen Zeichenkette in dieser Instanz zurück. |
| [indexOf(String value, int startIndex, int count)](#indexOf-java.lang.String-int-int-) | Gibt den nullbasierten Index des ersten Vorkommens der angegebenen Zeichenkette in dieser Instanz zurück. |
| [indexOf(String value, int startIndex, int count, short comparisonType)](#indexOf-java.lang.String-int-int-short-) | Gibt den nullbasierten Index des ersten Vorkommens der angegebenen Zeichenkette in der aktuellen Instanz zurück. |
| [indexOf(String value, short comparisonType)](#indexOf-java.lang.String-short-) | Gibt den nullbasierten Index des ersten Vorkommens der angegebenen Zeichenkette in der aktuellen Instanz zurück. |
| [indexOf_Rename_Namesake(String value, int startIndex, short comparisonType)](#indexOf-Rename-Namesake-java.lang.String-int-short-) | Gibt den nullbasierten Index des ersten Vorkommens der angegebenen Zeichenkette in der aktuellen Instanz zurück. |
| [insert(int startIndex, String value)](#insert-int-java.lang.String-) | Fügt eine angegebene Zeichenkette an einer angegebenen Indexposition in dieser Instanz ein. |
| [insert(int startIndex, String value, TextStyle style)](#insert-int-java.lang.String-com.aspose.note.TextStyle-) | Fügt eine angegebene Zeichenkette mit angegebenem Stil an einer angegebenen Indexposition in dieser Instanz ein. |
| [iterator()](#iterator--) |  |
| [remove(int startIndex)](#remove-int-) | Entfernt alle Zeichen in der aktuellen Instanz, beginnend an einer angegebenen Position und bis zur letzten Position. |
| [remove(int startIndex, int count)](#remove-int-int-) | Entfernt eine angegebene Anzahl von Zeichen in der aktuellen Instanz, beginnend an einer angegebenen Position. |
| [replace(char oldChar, char newChar)](#replace-char-char-) | Ersetzt alle Vorkommen eines angegebenen Unicode-Zeichens in dieser Instanz durch ein anderes angegebenes Unicode-Zeichen. |
| [replace(String oldValue, String newValue)](#replace-java.lang.String-java.lang.String-) | Ersetzt alle Vorkommen einer angegebenen Zeichenkette in der aktuellen Instanz durch eine andere angegebene Zeichenkette. |
| [replace(String oldValue, String newValue, TextStyle style)](#replace-java.lang.String-java.lang.String-com.aspose.note.TextStyle-) | Ersetzt alle Vorkommen einer angegebenen Zeichenkette in der aktuellen Instanz durch eine andere angegebene Zeichenkette im angegebenen Stil. |
| [setAlignment(int value)](#setAlignment-int-) | Legt die Ausrichtung fest. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Legt die zuletzt geänderte Zeit fest. |
| [setLineSpacing(float value)](#setLineSpacing-float-) |  |
| [setLineSpacing(Float value)](#setLineSpacing-java.lang.Float-) | Setzt den Zeilenabstand. |
| [setParagraphStyle(ParagraphStyle value)](#setParagraphStyle-com.aspose.note.ParagraphStyle-) | Setzt den Absatzstil. |
| [setSpaceAfter(float value)](#setSpaceAfter-float-) |  |
| [setSpaceAfter(Float value)](#setSpaceAfter-java.lang.Float-) | Setzt den minimalen Abstand nach. |
| [setSpaceBefore(float value)](#setSpaceBefore-float-) |  |
| [setSpaceBefore(Float value)](#setSpaceBefore-java.lang.Float-) | Legt die minimale Menge an Abstand davor fest. |
| [setText(String value)](#setText-java.lang.String-) | Legt den Text fest. |
| [trim()](#trim--) | Entfernt alle führenden und nachfolgenden Leerzeichen. |
| [trim(char trimChar)](#trim-char-) | Entfernt alle führenden und nachfolgenden Vorkommen eines Zeichens. |
| [trim(char[] trimChars)](#trim-char...-) | Entfernt alle führenden und nachfolgenden Vorkommen einer Menge von Zeichen, die in einem Array angegeben sind. |
| [trimEnd()](#trimEnd--) | Entfernt alle nachfolgenden Leerzeichen. |
| [trimEnd(char trimChar)](#trimEnd-char-) | Entfernt alle nachfolgenden Vorkommen eines Zeichens. |
| [trimEnd(char[] trimChars)](#trimEnd-char...-) | Entfernt alle nachfolgenden Vorkommen einer Menge von Zeichen, die in einem Array angegeben sind. |
| [trimStart()](#trimStart--) | Entfernt alle führenden Leerzeichen. |
| [trimStart(char trimChar)](#trimStart-char-) | Entfernt alle führenden Vorkommen eines angegebenen Zeichens. |
| [trimStart(char[] trimChars)](#trimStart-char...-) | Entfernt alle führenden Vorkommen einer Menge von Zeichen, die in einem Array angegeben sind. |
### RichText() {#RichText--}
```
public RichText()
```


Initialisiert eine neue Instanz der Klasse [RichText](../../com.aspose.note/richtext).

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Akzeptiert den Besucher des Knotens.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | Das Objekt einer von der [DocumentVisitor](../../com.aspose.note/documentvisitor) abgeleiteten Klasse. |

### append(String value) {#append-java.lang.String-}
```
public RichText append(String value)
```


Fügt einen String zum letzten Textbereich hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | Der hinzugefügte Wert. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### append(String value, TextStyle style) {#append-java.lang.String-com.aspose.note.TextStyle-}
```
public final RichText append(String value, TextStyle style)
```


Fügt einen String am Ende hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | Der hinzugefügte Wert. |
| style | [TextStyle](../../com.aspose.note/textstyle) | Der Stil der hinzugefügten Zeichenkette. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### appendFront(String value) {#appendFront-java.lang.String-}
```
public RichText appendFront(String value)
```


Fügt einen String am Anfang des ersten Textbereichs hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | Der hinzugefügte Wert. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### appendFront(String value, TextStyle style) {#appendFront-java.lang.String-com.aspose.note.TextStyle-}
```
public RichText appendFront(String value, TextStyle style)
```


Fügt einen String am Anfang hinzu.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | Der hinzugefügte Wert. |
| style | [TextStyle](../../com.aspose.note/textstyle) | Der Stil der hinzugefügten Zeichenkette. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### clear() {#clear--}
```
public final RichText clear()
```


Löscht den Inhalt dieser Instanz.

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### getAlignment() {#getAlignment--}
```
public int getAlignment()
```


Ruft die Ausrichtung ab.

**Returns:**
int
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Liest die zuletzt geänderte Zeit.

**Returns:**
java.util.Date
### getLength() {#getLength--}
```
public final int getLength()
```




**Returns:**
int
### getLineSpacing() {#getLineSpacing--}
```
public Float getLineSpacing()
```


Ermittelt den Zeilenabstand.

**Returns:**
java.lang.Float
### getParagraphStyle() {#getParagraphStyle--}
```
public final ParagraphStyle getParagraphStyle()
```


Liest den Absatzstil. Diese Einstellungen werden verwendet, wenn kein passendes TextStyle-Objekt in der [getStyles](../../com.aspose.note/richtext\#getStyles) Sammlung vorhanden ist oder dieses Objekt die benötigte Einstellung nicht angibt.

**Returns:**
[ParagraphStyle](../../com.aspose.note/paragraphstyle)
### getSpaceAfter() {#getSpaceAfter--}
```
public Float getSpaceAfter()
```


Ermittelt den minimalen Abstand nach.

**Returns:**
java.lang.Float
### getSpaceBefore() {#getSpaceBefore--}
```
public Float getSpaceBefore()
```


Ermittelt den minimalen Abstand vor.

**Returns:**
java.lang.Float
### getStyles() {#getStyles--}
```
public System.Collections.Generic.IGenericEnumerable<TextStyle> getStyles()
```


Ermittelt die Stile.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerable&lt;com.aspose.note.TextStyle&gt;
### getTags() {#getTags--}
```
public final System.Collections.Generic.List<ITag> getTags()
```


Ermittelt die Liste aller Tags eines Absatzes.

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.note.ITag&gt;
### getText() {#getText--}
```
public final String getText()
```


Liest den Text. Die Zeichenkette MUSS NICHT Zeichen mit dem Wert 10 (Zeilenumbruch) enthalten.

**Returns:**
java.lang.String
### getTextRuns() {#getTextRuns--}
```
public final System.Collections.Generic.IGenericEnumerable<TextRun> getTextRuns()
```




**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerable&lt;com.aspose.note.TextRun&gt;
### indexOf(char value) {#indexOf-char-}
```
public final int indexOf(char value)
```


Gibt den nullbasierten Index des ersten Vorkommens des angegebenen Unicode-Zeichens in diesem String zurück.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | char | Der Wert. |

**Returns:**
int - Der `int`.
### indexOf(char value, int startIndex) {#indexOf-char-int-}
```
public final int indexOf(char value, int startIndex)
```


Gibt den nullbasierten Index des ersten Vorkommens des angegebenen Unicode-Zeichens in dieser Zeichenkette zurück. Die Suche beginnt an einer angegebenen Zeichenposition.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | char | Der Wert. |
| startIndex | int | Die Startposition der Suche |

**Returns:**
int - Der `int`.
### indexOf(char value, int startIndex, int count) {#indexOf-char-int-int-}
```
public final int indexOf(char value, int startIndex, int count)
```


Gibt den nullbasierten Index des ersten Vorkommens des angegebenen Zeichens in dieser Instanz zurück. Die Suche beginnt an einer angegebenen Zeichenposition und prüft eine angegebene Anzahl von Zeichenpositionen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | char | Der Wert. |
| startIndex | int | Die Startposition der Suche |
| count | int | Die Anzahl. |

**Returns:**
int - Der `int`.
### indexOf(String value) {#indexOf-java.lang.String-}
```
public final int indexOf(String value)
```


Gibt den nullbasierten Index des ersten Vorkommens der angegebenen Zeichenkette in dieser Instanz zurück.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | Der Wert. |

**Returns:**
int - Der `int`.
### indexOf(String value, int startIndex) {#indexOf-java.lang.String-int-}
```
public final int indexOf(String value, int startIndex)
```


Gibt den nullbasierten Index des ersten Vorkommens der angegebenen Zeichenkette in dieser Instanz zurück. Die Suche beginnt an einer angegebenen Zeichenposition.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | Der Wert. |
| startIndex | int | Die Startposition der Suche |

**Returns:**
int - Der `int`.
### indexOf(String value, int startIndex, int count) {#indexOf-java.lang.String-int-int-}
```
public final int indexOf(String value, int startIndex, int count)
```


Gibt den nullbasierten Index des ersten Vorkommens der angegebenen Zeichenkette in dieser Instanz zurück. Die Suche beginnt an einer angegebenen Zeichenposition und untersucht eine angegebene Anzahl von Zeichenpositionen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | Der Wert. |
| startIndex | int | Die Startposition der Suche |
| count | int | Die Anzahl. |

**Returns:**
int - Der `int`.
### indexOf(String value, int startIndex, int count, short comparisonType) {#indexOf-java.lang.String-int-int-short-}
```
public final int indexOf(String value, int startIndex, int count, short comparisonType)
```


Gibt den nullbasierten Index des ersten Vorkommens der angegebenen Zeichenkette in der aktuellen Instanz zurück.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | Der Wert. |
| startIndex | int | Die Startposition der Suche |
| count | int | Die Anzahl. |
| comparisonType | short | Der Typ der Suche, der für die angegebene Zeichenkette verwendet werden soll |

**Returns:**
int - Der `int`.
### indexOf(String value, short comparisonType) {#indexOf-java.lang.String-short-}
```
public final int indexOf(String value, short comparisonType)
```


Gibt den nullbasierten Index des ersten Vorkommens der angegebenen Zeichenkette in der aktuellen Instanz zurück. Ein Parameter gibt den Typ der Suche an, der für die angegebene Zeichenkette verwendet werden soll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | Der Wert. |
| comparisonType | short | Der Typ der Suche, der für die angegebene Zeichenkette verwendet werden soll |

**Returns:**
int - Der `int`.
### indexOf_Rename_Namesake(String value, int startIndex, short comparisonType) {#indexOf-Rename-Namesake-java.lang.String-int-short-}
```
public final int indexOf_Rename_Namesake(String value, int startIndex, short comparisonType)
```


Gibt den nullbasierten Index des ersten Vorkommens der angegebenen Zeichenkette in der aktuellen Instanz zurück. Parameter geben die Startposition der Suche in der aktuellen Zeichenkette und den Typ der Suche an, der für die angegebene Zeichenkette verwendet werden soll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | Der Wert. |
| startIndex | int | Die Startposition der Suche |
| comparisonType | short | Der Typ der Suche, der für die angegebene Zeichenkette verwendet werden soll |

**Returns:**
int - Der `int`.
### insert(int startIndex, String value) {#insert-int-java.lang.String-}
```
public final RichText insert(int startIndex, String value)
```


Fügt eine angegebene Zeichenkette an einer angegebenen Indexposition in dieser Instanz ein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startIndex | int | Der Startindex. |
| Wert | java.lang.String | Der Wert. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### insert(int startIndex, String value, TextStyle style) {#insert-int-java.lang.String-com.aspose.note.TextStyle-}
```
public final RichText insert(int startIndex, String value, TextStyle style)
```


Fügt eine angegebene Zeichenkette mit angegebenem Stil an einer angegebenen Indexposition in dieser Instanz ein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startIndex | int | Der Startindex. |
| Wert | java.lang.String | Der Wert. |
| style | [TextStyle](../../com.aspose.note/textstyle) | Der Stil. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<Character> iterator()
```




**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;java.lang.Character&gt;
### remove(int startIndex) {#remove-int-}
```
public final RichText remove(int startIndex)
```


Entfernt alle Zeichen in der aktuellen Instanz, beginnend an einer angegebenen Position und bis zur letzten Position.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startIndex | int | Der Startindex. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### remove(int startIndex, int count) {#remove-int-int-}
```
public final RichText remove(int startIndex, int count)
```


Entfernt eine angegebene Anzahl von Zeichen in der aktuellen Instanz, beginnend an einer angegebenen Position.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startIndex | int | Der Startindex. |
| count | int | Die Anzahl. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### replace(char oldChar, char newChar) {#replace-char-char-}
```
public final RichText replace(char oldChar, char newChar)
```


Ersetzt alle Vorkommen eines angegebenen Unicode-Zeichens in dieser Instanz durch ein anderes angegebenes Unicode-Zeichen.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| oldChar | char | Das alte Zeichen. |
| newChar | char | Das neue Zeichen. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### replace(String oldValue, String newValue) {#replace-java.lang.String-java.lang.String-}
```
public final RichText replace(String oldValue, String newValue)
```


Ersetzt alle Vorkommen einer angegebenen Zeichenkette in der aktuellen Instanz durch eine andere angegebene Zeichenkette.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| oldValue | java.lang.String | Der alte Wert. |
| newValue | java.lang.String | Der neue Wert. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### replace(String oldValue, String newValue, TextStyle style) {#replace-java.lang.String-java.lang.String-com.aspose.note.TextStyle-}
```
public final RichText replace(String oldValue, String newValue, TextStyle style)
```


Ersetzt alle Vorkommen einer angegebenen Zeichenkette in der aktuellen Instanz durch eine andere angegebene Zeichenkette im angegebenen Stil.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| oldValue | java.lang.String | Der alte Wert. |
| newValue | java.lang.String | Der neue Wert. |
| style | [TextStyle](../../com.aspose.note/textstyle) | Der Stil des neuen Wertes. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### setAlignment(int value) {#setAlignment-int-}
```
public void setAlignment(int value)
```


Legt die Ausrichtung fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Legt die zuletzt geänderte Zeit fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.Date |  |

### setLineSpacing(float value) {#setLineSpacing-float-}
```
public void setLineSpacing(float value)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | float |  |

### setLineSpacing(Float value) {#setLineSpacing-java.lang.Float-}
```
public void setLineSpacing(Float value)
```


Setzt den Zeilenabstand.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.Float |  |

### setParagraphStyle(ParagraphStyle value) {#setParagraphStyle-com.aspose.note.ParagraphStyle-}
```
public final void setParagraphStyle(ParagraphStyle value)
```


Legt den Absatzstil fest. Diese Einstellungen werden verwendet, wenn kein passendes TextStyle-Objekt in der [getStyles](../../com.aspose.note/richtext\#getStyles)-Sammlung vorhanden ist oder dieses Objekt keine erforderliche Einstellung angibt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [ParagraphStyle](../../com.aspose.note/paragraphstyle) |  |

### setSpaceAfter(float value) {#setSpaceAfter-float-}
```
public void setSpaceAfter(float value)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | float |  |

### setSpaceAfter(Float value) {#setSpaceAfter-java.lang.Float-}
```
public void setSpaceAfter(Float value)
```


Setzt den minimalen Abstand nach.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.Float |  |

### setSpaceBefore(float value) {#setSpaceBefore-float-}
```
public void setSpaceBefore(float value)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | float |  |

### setSpaceBefore(Float value) {#setSpaceBefore-java.lang.Float-}
```
public void setSpaceBefore(Float value)
```


Legt die minimale Menge an Abstand davor fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.Float |  |

### setText(String value) {#setText-java.lang.String-}
```
public final void setText(String value)
```


Setzt den Text. Der String DARF NICHT die Zeichen mit dem Wert 10 (Zeilenumbruch) enthalten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### trim() {#trim--}
```
public final RichText trim()
```


Entfernt alle führenden und nachfolgenden Leerzeichen.

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trim(char trimChar) {#trim-char-}
```
public final RichText trim(char trimChar)
```


Entfernt alle führenden und nachfolgenden Vorkommen eines Zeichens.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| trimChar | char | Das Trimmzeichen. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trim(char[] trimChars) {#trim-char...-}
```
public final RichText trim(char[] trimChars)
```


Entfernt alle führenden und nachfolgenden Vorkommen einer Menge von Zeichen, die in einem Array angegeben sind.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| trimChars | char[] | Die Trimmzeichen. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimEnd() {#trimEnd--}
```
public final RichText trimEnd()
```


Entfernt alle nachfolgenden Leerzeichen.

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimEnd(char trimChar) {#trimEnd-char-}
```
public final RichText trimEnd(char trimChar)
```


Entfernt alle nachfolgenden Vorkommen eines Zeichens.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| trimChar | char | Das Trimmzeichen. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimEnd(char[] trimChars) {#trimEnd-char...-}
```
public final RichText trimEnd(char[] trimChars)
```


Entfernt alle nachfolgenden Vorkommen einer Menge von Zeichen, die in einem Array angegeben sind.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| trimChars | char[] | Die Trimmzeichen. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimStart() {#trimStart--}
```
public final RichText trimStart()
```


Entfernt alle führenden Leerzeichen.

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimStart(char trimChar) {#trimStart-char-}
```
public final RichText trimStart(char trimChar)
```


Entfernt alle führenden Vorkommen eines angegebenen Zeichens.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| trimChar | char | Das Trimmzeichen. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimStart(char[] trimChars) {#trimStart-char...-}
```
public final RichText trimStart(char[] trimChars)
```


Entfernt alle führenden Vorkommen einer Menge von Zeichen, die in einem Array angegeben sind.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| trimChars | char[] | Die Trimmzeichen. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
