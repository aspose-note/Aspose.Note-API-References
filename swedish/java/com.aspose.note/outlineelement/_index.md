---
title: "OutlineElement"
second_title: "Aspose.Note for Java API-referens"
description: "Representerar ett OutlineElement."
type: docs
weight: 67
url: /sv/java/com.aspose.note/outlineelement/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode, com.aspose.note.IndentatedNode

**All Implemented Interfaces:**
[com.aspose.note.IOutlineChildNode](../../com.aspose.note/ioutlinechildnode), [com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode)
```
public final class OutlineElement extends IndentatedNode<IOutlineElementChildNode,OutlineElement> implements IOutlineChildNode, IOutlineElementChildNode
```

Representerar ett OutlineElement.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [OutlineElement()](#OutlineElement--) | Initierar en ny instans av klassen `OutlineElement`. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepterar nodens besökare. |
| [getAuthorMostRecent()](#getAuthorMostRecent--) | Hämtar den senast ändrade författaren för ett outline‑element. |
| [getAuthorOriginal()](#getAuthorOriginal--) | Hämtar den ursprungliga författaren för ett outline‑element. |
| [getCreationTime()](#getCreationTime--) | Hämtar eller anger skapningstiden. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Hämtar eller anger den senast ändrade tiden. |
| [getNumberList()](#getNumberList--) | Hämtar eller anger stilen för rubriken i en numrerad lista. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Hämtar eller anger skapningstiden. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Hämtar eller anger den senast ändrade tiden. |
| [setNumberList(NumberList value)](#setNumberList-com.aspose.note.NumberList-) | Hämtar eller anger stilen för rubriken i en numrerad lista. |
### OutlineElement() {#OutlineElement--}
```
public OutlineElement()
```


Initierar en ny instans av klassen `OutlineElement`.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Accepterar nodens besökare.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | Objektet av en klass som är härledd från `DocumentVisitor`. |

### getAuthorMostRecent() {#getAuthorMostRecent--}
```
public final String getAuthorMostRecent()
```


Hämtar den senast ändrade författaren för ett outline‑element.

Värde: Den senast ändrade författaren.

**Returns:**
java.lang.String
### getAuthorOriginal() {#getAuthorOriginal--}
```
public final String getAuthorOriginal()
```


Hämtar den ursprungliga författaren för ett outline‑element.

Värde: Den ursprungliga författaren.

**Returns:**
java.lang.String
### getCreationTime() {#getCreationTime--}
```
public Date getCreationTime()
```


Hämtar eller anger skapningstiden.

**Returns:**
java.util.Date
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Hämtar eller anger den senast ändrade tiden.

**Returns:**
java.util.Date
### getNumberList() {#getNumberList--}
```
public NumberList getNumberList()
```


Hämtar eller anger stilen för rubriken i en numrerad lista.

**Returns:**
[NumberList](../../com.aspose.note/numberlist)
### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public void setCreationTime(Date value)
```


Hämtar eller anger skapningstiden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.Date |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Hämtar eller anger den senast ändrade tiden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.Date |  |

### setNumberList(NumberList value) {#setNumberList-com.aspose.note.NumberList-}
```
public void setNumberList(NumberList value)
```


Hämtar eller anger stilen för rubriken i en numrerad lista.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [NumberList](../../com.aspose.note/numberlist) |  |

