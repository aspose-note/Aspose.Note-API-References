---
title: "Title"
second_title: "Aspose.Note for Java API-referens"
description: "Representerar en titel."
type: docs
weight: 95
url: /sv/java/com.aspose.note/title/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase)

**All Implemented Interfaces:**
com.aspose.note.ICompositeNodeT, [com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode)
```
public final class Title extends CompositeNodeBase implements ICompositeNodeT<RichText>, IPageChildNode
```

Representerar en titel.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [Title()](#Title--) | Initierar en ny instans av klassen `Title`. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [&lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass)](#-T1-getChildNodes-java.lang.Class-T1--) | Hämta alla underordnade noder efter nodtypen. |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepterar nodens besökare. |
| [getChildNodes(int type)](#getChildNodes-int-) |  |
| [getHorizontalOffset()](#getHorizontalOffset--) | Hämtar eller anger den horisontella förskjutningen. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Hämtar eller anger den senast ändrade tiden. |
| [getTitleDate()](#getTitleDate--) | Hämtar eller anger en strängrepresentation av datumet i titeln. |
| [getTitleText()](#getTitleText--) | Hämtar eller anger texten i titeln. |
| [getTitleTime()](#getTitleTime--) | Hämtar eller anger en strängrepresentation av tiden i titeln. |
| [getVerticalOffset()](#getVerticalOffset--) | Hämtar eller anger den vertikala förskjutningen. |
| [isComposite()](#isComposite--) | Hämtar ett värde som indikerar om denna nod är sammansatt. |
| [iterator()](#iterator--) | Returnerar en enumerator som itererar genom undernoder till [Title](../../com.aspose.note/title). |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | Hämtar eller anger den horisontella förskjutningen. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Hämtar eller anger den senast ändrade tiden. |
| [setTitleDate(RichText value)](#setTitleDate-com.aspose.note.RichText-) | Hämtar eller anger en strängrepresentation av datumet i titeln. |
| [setTitleText(RichText value)](#setTitleText-com.aspose.note.RichText-) | Hämtar eller anger texten i titeln. |
| [setTitleTime(RichText value)](#setTitleTime-com.aspose.note.RichText-) | Hämtar eller anger en strängrepresentation av tiden i titeln. |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | Hämtar eller anger den vertikala förskjutningen. |
### Title() {#Title--}
```
public Title()
```


Initierar en ny instans av klassen `Title`.

### &lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass) {#-T1-getChildNodes-java.lang.Class-T1--}
```
public List<T1> <T1>getChildNodes(Class<T1> typeParameterClass)
```


Hämta alla underordnade noder efter nodtypen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| typeParameterClass | java.lang.Class&lt;T1&gt; |  |

**Returns:**
java.util.List&lt;T1&gt; - En lista med barnnoder.

`T1`: Typen av element i den returnerade listan.
### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Accepterar nodens besökare.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | Objektet av en klass som är härledd från `DocumentVisitor`. |

### getChildNodes(int type) {#getChildNodes-int-}
```
public List<INode> getChildNodes(int type)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| typ | int |  |

**Returns:**
java.util.List&lt;com.aspose.note.INode&gt;
### getHorizontalOffset() {#getHorizontalOffset--}
```
public final float getHorizontalOffset()
```


Hämtar eller anger den horisontella förskjutningen.

**Returns:**
float
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Hämtar eller anger den senast ändrade tiden.

**Returns:**
java.util.Date
### getTitleDate() {#getTitleDate--}
```
public final RichText getTitleDate()
```


Hämtar eller anger en strängrepresentation av datumet i titeln.

**Returns:**
[RichText](../../com.aspose.note/richtext)
### getTitleText() {#getTitleText--}
```
public RichText getTitleText()
```


Hämtar eller anger texten i titeln.

**Returns:**
[RichText](../../com.aspose.note/richtext)
### getTitleTime() {#getTitleTime--}
```
public final RichText getTitleTime()
```


Hämtar eller anger en strängrepresentation av tiden i titeln.

**Returns:**
[RichText](../../com.aspose.note/richtext)
### getVerticalOffset() {#getVerticalOffset--}
```
public final float getVerticalOffset()
```


Hämtar eller anger den vertikala förskjutningen.

**Returns:**
float
### isComposite() {#isComposite--}
```
public boolean isComposite()
```


Hämtar ett värde som indikerar om denna nod är sammansatt. Om sant kan noden ha undernoder.

**Returns:**
boolean
### iterator() {#iterator--}
```
public final System.Collections.Generic.IGenericEnumerator<RichText> iterator()
```


Returnerar en enumerator som itererar genom undernoder till [Title](../../com.aspose.note/title).

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.note.RichText&gt; - Enumeratorn.
### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public final void setHorizontalOffset(float value)
```


Hämtar eller anger den horisontella förskjutningen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | float |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Hämtar eller anger den senast ändrade tiden.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.util.Date |  |

### setTitleDate(RichText value) {#setTitleDate-com.aspose.note.RichText-}
```
public final void setTitleDate(RichText value)
```


Hämtar eller anger en strängrepresentation av datumet i titeln.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [RichText](../../com.aspose.note/richtext) |  |

### setTitleText(RichText value) {#setTitleText-com.aspose.note.RichText-}
```
public final void setTitleText(RichText value)
```


Hämtar eller anger texten i titeln.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [RichText](../../com.aspose.note/richtext) |  |

### setTitleTime(RichText value) {#setTitleTime-com.aspose.note.RichText-}
```
public final void setTitleTime(RichText value)
```


Hämtar eller anger en strängrepresentation av tiden i titeln.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [RichText](../../com.aspose.note/richtext) |  |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public final void setVerticalOffset(float value)
```


Hämtar eller anger den vertikala förskjutningen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | float |  |

