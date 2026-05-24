---
title: "NumberList"
second_title: "Aspose.Note für Java API-Referenz"
description: "Stellt die nummerierte oder Aufzählungsliste dar."
type: docs
weight: 64
url: /de/java/com.aspose.note/numberlist/
---

**Inheritance:**
java.lang.Object
```
public class NumberList
```

Stellt die nummerierte oder Aufzählungsliste dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [NumberList(String bulletedSymbol, String font, int fontSize)](#NumberList-java.lang.String-java.lang.String-int-) | Initialisiert eine neue Instanz der `NumberList`-Klasse. |
| [NumberList(String format, byte numberFormat, String font, int fontSize)](#NumberList-java.lang.String-byte-java.lang.String-int-) | Initialisiert eine neue Instanz der `NumberList`-Klasse. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(NumberList other)](#equals-com.aspose.note.NumberList-) | Bestimmt, ob das angegebene Objekt dem aktuellen Objekt gleich ist. |
| [equals(Object obj)](#equals-java.lang.Object-) | Bestimmt, ob das angegebene Objekt dem aktuellen Objekt gleich ist. |
| [getFont()](#getFont--) | Liest oder setzt den Namen der Schriftart. |
| [getFontColor()](#getFontColor--) | Liest oder setzt die Schriftfarbe. |
| [getFontSize()](#getFontSize--) | Liest oder setzt die Schriftgröße. |
| [getFormat()](#getFormat--) | Liest oder setzt das Format der Zeilenüberschrift. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Liest oder setzt die zuletzt geänderte Zeit. |
| [getNumberFormat()](#getNumberFormat--) | Liest oder setzt das Zahlenformat, das für eine Gruppe automatisch nummerierter Objekte verwendet wird. |
| [getNumberedListHeader(int sequenceNumber)](#getNumberedListHeader-int-) | Liest die Überschrift der nummerierten Liste. |
| [getRestart()](#getRestart--) | Liest oder setzt den numerischen Wert, der den automatischen Nummernwert des Listenelements überschreibt. |
| [hashCode()](#hashCode--) | Dient als Hash-Funktion für den Typ. |
| [isBold()](#isBold--) | Liest oder setzt einen Wert, der angibt, ob der Textstil fett ist. |
| [isItalic()](#isItalic--) | Liest oder setzt einen Wert, der angibt, ob der Textstil kursiv ist. |
| [setBold(boolean value)](#setBold-boolean-) | Liest oder setzt einen Wert, der angibt, ob der Textstil fett ist. |
| [setFont(String value)](#setFont-java.lang.String-) | Liest oder setzt den Namen der Schriftart. |
| [setFontColor(Color value)](#setFontColor-java.awt.Color-) | Liest oder setzt die Schriftfarbe. |
| [setFontSize(int value)](#setFontSize-int-) | Liest oder setzt die Schriftgröße. |
| [setFormat(String value)](#setFormat-java.lang.String-) | Liest oder setzt das Format der Zeilenüberschrift. |
| [setItalic(boolean value)](#setItalic-boolean-) | Liest oder setzt einen Wert, der angibt, ob der Textstil kursiv ist. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Liest oder setzt die zuletzt geänderte Zeit. |
| [setNumberFormat(Byte value)](#setNumberFormat-java.lang.Byte-) | Liest oder setzt das Zahlenformat, das für eine Gruppe automatisch nummerierter Objekte verwendet wird. |
| [setRestart(int value)](#setRestart-int-) | Liest oder setzt den numerischen Wert, der den automatischen Nummernwert des Listenelements überschreibt. |
### NumberList(String bulletedSymbol, String font, int fontSize) {#NumberList-java.lang.String-java.lang.String-int-}
```
public NumberList(String bulletedSymbol, String font, int fontSize)
```


Initialisiert eine neue Instanz der `NumberList`-Klasse. Diese Instanz stellt eine Aufzählungsliste dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| bulletedSymbol | java.lang.String | Ein Symbol, das einen Aufzählungspunkt darstellt. |
| Schriftart | java.lang.String | Eine Schriftart für den Aufzählungspunkt. |
| fontSize | int | Eine Schriftgröße für den Aufzählungspunkt. |

### NumberList(String format, byte numberFormat, String font, int fontSize) {#NumberList-java.lang.String-byte-java.lang.String-int-}
```
public NumberList(String format, byte numberFormat, String font, int fontSize)
```


Initialisiert eine neue Instanz der `NumberList`-Klasse. Diese Instanz stellt eine nummerierte Liste dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| format | java.lang.String | Das Format der nummerierten Überschrift. |
| numberFormat | byte | Das Format der Nummer in der Überschrift. |
| Schriftart | java.lang.String | Eine Schriftart für die nummerierte Überschrift. |
| fontSize | int | Eine Schriftgröße für die nummerierte Überschrift. |

### equals(NumberList other) {#equals-com.aspose.note.NumberList-}
```
public boolean equals(NumberList other)
```


Bestimmt, ob das angegebene Objekt dem aktuellen Objekt gleich ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| other | [NumberList](../../com.aspose.note/numberlist) | Das Objekt. |

**Returns:**
boolean - Der `bool`.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Bestimmt, ob das angegebene Objekt dem aktuellen Objekt gleich ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| obj | java.lang.Object | Das Objekt. |

**Returns:**
boolean - Der `bool`.
### getFont() {#getFont--}
```
public String getFont()
```


Liest oder setzt den Namen der Schriftart.

**Returns:**
java.lang.String
### getFontColor() {#getFontColor--}
```
public Color getFontColor()
```


Liest oder setzt die Schriftfarbe.

**Returns:**
java.awt.Color
### getFontSize() {#getFontSize--}
```
public int getFontSize()
```


Liest oder setzt die Schriftgröße.

**Returns:**
int
### getFormat() {#getFormat--}
```
public String getFormat()
```


Liest oder setzt das Format der Zeilenüberschrift. Für Aufzählungslisten stellt ein Aufzählungszeichen dar.

**Returns:**
java.lang.String
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Liest oder setzt die zuletzt geänderte Zeit.

**Returns:**
java.util.Date
### getNumberFormat() {#getNumberFormat--}
```
public Byte getNumberFormat()
```


Liest oder setzt das Zahlenformat, das für eine Gruppe automatisch nummerierter Objekte verwendet wird. Sollte für Aufzählungslisten null sein.

**Returns:**
java.lang.Byte
### getNumberedListHeader(int sequenceNumber) {#getNumberedListHeader-int-}
```
public String getNumberedListHeader(int sequenceNumber)
```


Liest die Überschrift der nummerierten Liste.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| sequenceNumber | int | Die Sequenznummer in der nummerierten Liste. |

**Returns:**
java.lang.String - Eine Zeichenkettenrepräsentation der angegebenen Sequenznummer.
### getRestart() {#getRestart--}
```
public int getRestart()
```


Liest oder setzt den numerischen Wert, der den automatischen Nummernwert des Listenelements überschreibt.

**Returns:**
int
### hashCode() {#hashCode--}
```
public int hashCode()
```


Dient als Hash-Funktion für den Typ.

**Returns:**
int - Der `int`.
### isBold() {#isBold--}
```
public boolean isBold()
```


Liest oder setzt einen Wert, der angibt, ob der Textstil fett ist.

**Returns:**
boolean
### isItalic() {#isItalic--}
```
public boolean isItalic()
```


Liest oder setzt einen Wert, der angibt, ob der Textstil kursiv ist.

**Returns:**
boolean
### setBold(boolean value) {#setBold-boolean-}
```
public void setBold(boolean value)
```


Liest oder setzt einen Wert, der angibt, ob der Textstil fett ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setFont(String value) {#setFont-java.lang.String-}
```
public void setFont(String value)
```


Liest oder setzt den Namen der Schriftart.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setFontColor(Color value) {#setFontColor-java.awt.Color-}
```
public void setFontColor(Color value)
```


Liest oder setzt die Schriftfarbe.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.awt.Color |  |

### setFontSize(int value) {#setFontSize-int-}
```
public void setFontSize(int value)
```


Liest oder setzt die Schriftgröße.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setFormat(String value) {#setFormat-java.lang.String-}
```
public void setFormat(String value)
```


Liest oder setzt das Format der Zeilenüberschrift. Für Aufzählungslisten stellt ein Aufzählungszeichen dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setItalic(boolean value) {#setItalic-boolean-}
```
public void setItalic(boolean value)
```


Liest oder setzt einen Wert, der angibt, ob der Textstil kursiv ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Liest oder setzt die zuletzt geänderte Zeit.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.Date |  |

### setNumberFormat(Byte value) {#setNumberFormat-java.lang.Byte-}
```
public void setNumberFormat(Byte value)
```


Liest oder setzt das Zahlenformat, das für eine Gruppe automatisch nummerierter Objekte verwendet wird. Sollte für Aufzählungslisten null sein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.Byte |  |

### setRestart(int value) {#setRestart-int-}
```
public void setRestart(int value)
```


Liest oder setzt den numerischen Wert, der den automatischen Nummernwert des Listenelements überschreibt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

