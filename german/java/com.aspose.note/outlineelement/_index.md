---
title: "OutlineElement"
second_title: "Aspose.Note für Java API-Referenz"
description: "Stellt ein OutlineElement dar."
type: docs
weight: 67
url: /de/java/com.aspose.note/outlineelement/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode, com.aspose.note.IndentatedNode

**All Implemented Interfaces:**
[com.aspose.note.IOutlineChildNode](../../com.aspose.note/ioutlinechildnode), [com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode)
```
public final class OutlineElement extends IndentatedNode<IOutlineElementChildNode,OutlineElement> implements IOutlineChildNode, IOutlineElementChildNode
```

Stellt ein OutlineElement dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [OutlineElement()](#OutlineElement--) | Initialisiert eine neue Instanz der `OutlineElement`-Klasse. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Akzeptiert den Besucher des Knotens. |
| [getAuthorMostRecent()](#getAuthorMostRecent--) | Liest den zuletzt bearbeiteten Autor eines Gliederungselements. |
| [getAuthorOriginal()](#getAuthorOriginal--) | Liest den ursprünglichen Autor eines Gliederungselements. |
| [getCreationTime()](#getCreationTime--) | Liest oder setzt die Erstellungszeit. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Liest oder setzt die zuletzt geänderte Zeit. |
| [getNumberList()](#getNumberList--) | Liest oder setzt den Stil für die Kopfzeile einer nummerierten Liste. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Liest oder setzt die Erstellungszeit. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Liest oder setzt die zuletzt geänderte Zeit. |
| [setNumberList(NumberList value)](#setNumberList-com.aspose.note.NumberList-) | Liest oder setzt den Stil für die Kopfzeile einer nummerierten Liste. |
### OutlineElement() {#OutlineElement--}
```
public OutlineElement()
```


Initialisiert eine neue Instanz der `OutlineElement`-Klasse.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Akzeptiert den Besucher des Knotens.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | Das Objekt einer Klasse, die von `DocumentVisitor` abgeleitet ist. |

### getAuthorMostRecent() {#getAuthorMostRecent--}
```
public final String getAuthorMostRecent()
```


Liest den zuletzt bearbeiteten Autor eines Gliederungselements.

Wert: Der zuletzt bearbeitete Autor.

**Returns:**
java.lang.String
### getAuthorOriginal() {#getAuthorOriginal--}
```
public final String getAuthorOriginal()
```


Liest den ursprünglichen Autor eines Gliederungselements.

Wert: Der ursprüngliche Autor.

**Returns:**
java.lang.String
### getCreationTime() {#getCreationTime--}
```
public Date getCreationTime()
```


Liest oder setzt die Erstellungszeit.

**Returns:**
java.util.Date
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Liest oder setzt die zuletzt geänderte Zeit.

**Returns:**
java.util.Date
### getNumberList() {#getNumberList--}
```
public NumberList getNumberList()
```


Liest oder setzt den Stil für die Kopfzeile einer nummerierten Liste.

**Returns:**
[NumberList](../../com.aspose.note/numberlist)
### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public void setCreationTime(Date value)
```


Liest oder setzt die Erstellungszeit.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.Date |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Liest oder setzt die zuletzt geänderte Zeit.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.util.Date |  |

### setNumberList(NumberList value) {#setNumberList-com.aspose.note.NumberList-}
```
public void setNumberList(NumberList value)
```


Liest oder setzt den Stil für die Kopfzeile einer nummerierten Liste.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [NumberList](../../com.aspose.note/numberlist) |  |

