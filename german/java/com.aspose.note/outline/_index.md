---
title: "Outline"
second_title: "Aspose.Note für Java API-Referenz"
description: "Stellt eine Gliederung dar."
type: docs
weight: 66
url: /de/java/com.aspose.note/outline/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode, com.aspose.note.IndentatedNode

**All Implemented Interfaces:**
[com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode)
```
public final class Outline extends IndentatedNode<IOutlineChildNode,Outline> implements IPageChildNode
```

Stellt eine Gliederung dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [Outline()](#Outline--) | Initialisiert eine neue Instanz der [Outline](../../com.aspose.note/outline) Klasse. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Akzeptiert den Besucher des Knotens. |
| [getDescendantsCannotBeMoved()](#getDescendantsCannotBeMoved--) | Ermittelt, ob Nachkommen des Outline verschoben werden können. |
| [getHorizontalOffset()](#getHorizontalOffset--) | Liest oder setzt den horizontalen Versatz. |
| [getInternalIndentPosition()](#getInternalIndentPosition--) |  |
| [getLastModifiedTime()](#getLastModifiedTime--) | Liest oder setzt die zuletzt geänderte Zeit. |
| [getMaxHeight()](#getMaxHeight--) | Liest oder setzt die maximale Höhe. |
| [getMaxWidth()](#getMaxWidth--) | Liest oder setzt die maximale Breite. |
| [getMinWidth()](#getMinWidth--) | Liest oder setzt die minimale Breite. |
| [getReservedWidth()](#getReservedWidth--) | Liest oder setzt die reservierte Breite. |
| [getVerticalOffset()](#getVerticalOffset--) | Liest oder setzt den vertikalen Versatz. |
| [setDescendantsCannotBeMoved(boolean value)](#setDescendantsCannotBeMoved-boolean-) | Ermittelt, ob Nachkommen des Outline verschoben werden können. |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | Liest oder setzt den horizontalen Versatz. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Liest oder setzt die zuletzt geänderte Zeit. |
| [setMaxHeight(float value)](#setMaxHeight-float-) | Liest oder setzt die maximale Höhe. |
| [setMaxWidth(float value)](#setMaxWidth-float-) | Liest oder setzt die maximale Breite. |
| [setMinWidth(float value)](#setMinWidth-float-) | Liest oder setzt die minimale Breite. |
| [setReservedWidth(float value)](#setReservedWidth-float-) | Liest oder setzt die reservierte Breite. |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | Liest oder setzt den vertikalen Versatz. |
### Outline() {#Outline--}
```
public Outline()
```


Initialisiert eine neue Instanz der [Outline](../../com.aspose.note/outline) Klasse.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Akzeptiert den Besucher des Knotens.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | Das Objekt einer Klasse, die von `DocumentVisitor` abgeleitet ist. |

### getDescendantsCannotBeMoved() {#getDescendantsCannotBeMoved--}
```
public boolean getDescendantsCannotBeMoved()
```


Ermittelt, ob Nachkommen des Outline verschoben werden können.

**Returns:**
boolean
### getHorizontalOffset() {#getHorizontalOffset--}
```
public float getHorizontalOffset()
```


Liest oder setzt den horizontalen Versatz.

**Returns:**
float
### getInternalIndentPosition() {#getInternalIndentPosition--}
```
public int getInternalIndentPosition()
```


Ermittelt die Anzahl der Elemente, die im RgOutlineIndentDistance-Array summiert werden, um die Einzugsgröße zu erhalten.

**Returns:**
int
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Liest oder setzt die zuletzt geänderte Zeit.

**Returns:**
java.util.Date
### getMaxHeight() {#getMaxHeight--}
```
public float getMaxHeight()
```


Liest oder setzt die maximale Höhe.

**Returns:**
float
### getMaxWidth() {#getMaxWidth--}
```
public float getMaxWidth()
```


Liest oder setzt die maximale Breite.

**Returns:**
float
### getMinWidth() {#getMinWidth--}
```
public float getMinWidth()
```


Liest oder setzt die minimale Breite.

**Returns:**
float
### getReservedWidth() {#getReservedWidth--}
```
public float getReservedWidth()
```


Liest oder setzt die reservierte Breite.

**Returns:**
float
### getVerticalOffset() {#getVerticalOffset--}
```
public float getVerticalOffset()
```


Liest oder setzt den vertikalen Versatz.

**Returns:**
float
### setDescendantsCannotBeMoved(boolean value) {#setDescendantsCannotBeMoved-boolean-}
```
public void setDescendantsCannotBeMoved(boolean value)
```


Ermittelt, ob Nachkommen des Outline verschoben werden können.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public void setHorizontalOffset(float value)
```


Liest oder setzt den horizontalen Versatz.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | float |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Liest oder setzt die zuletzt geänderte Zeit.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.Date |  |

### setMaxHeight(float value) {#setMaxHeight-float-}
```
public void setMaxHeight(float value)
```


Liest oder setzt die maximale Höhe.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | float |  |

### setMaxWidth(float value) {#setMaxWidth-float-}
```
public void setMaxWidth(float value)
```


Liest oder setzt die maximale Breite.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | float |  |

### setMinWidth(float value) {#setMinWidth-float-}
```
public void setMinWidth(float value)
```


Liest oder setzt die minimale Breite.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | float |  |

### setReservedWidth(float value) {#setReservedWidth-float-}
```
public void setReservedWidth(float value)
```


Liest oder setzt die reservierte Breite.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | float |  |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public void setVerticalOffset(float value)
```


Liest oder setzt den vertikalen Versatz.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | float |  |

