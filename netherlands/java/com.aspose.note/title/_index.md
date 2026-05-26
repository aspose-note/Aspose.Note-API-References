---
title: "Title"
second_title: "Aspose.Note for Java API-referentie"
description: "Stelt een titel voor."
type: docs
weight: 95
url: /nl/java/com.aspose.note/title/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase)

**All Implemented Interfaces:**
com.aspose.note.ICompositeNodeT, [com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode)
```
public final class Title extends CompositeNodeBase implements ICompositeNodeT<RichText>, IPageChildNode
```

Stelt een titel voor.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [Title()](#Title--) | Initialiseert een nieuw exemplaar van de `Title`-klasse. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [&lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass)](#-T1-getChildNodes-java.lang.Class-T1--) | Haalt alle kindknopen op op basis van het knooptype. |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepteert de bezoeker van de node. |
| [getChildNodes(int type)](#getChildNodes-int-) |  |
| [getHorizontalOffset()](#getHorizontalOffset--) | Haalt op of stelt de horizontale offset in. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Haalt op of stelt de laatst gewijzigde tijd in. |
| [getTitleDate()](#getTitleDate--) | Haalt op of stelt een tekenreeksrepresentatie van de datum in de titel in. |
| [getTitleText()](#getTitleText--) | Haalt op of stelt de tekst van de titel in. |
| [getTitleTime()](#getTitleTime--) | Haalt op of stelt een tekenreeksrepresentatie van de tijd in de titel in. |
| [getVerticalOffset()](#getVerticalOffset--) | Haalt op of stelt de verticale offset in. |
| [isComposite()](#isComposite--) | Haalt een waarde op die aangeeft of dit knooppunt samengesteld is. |
| [iterator()](#iterator--) | Retourneert een enumerator die door de onderliggende knooppunten van de [Title](../../com.aspose.note/title) iterereert. |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | Haalt op of stelt de horizontale offset in. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Haalt op of stelt de laatst gewijzigde tijd in. |
| [setTitleDate(RichText value)](#setTitleDate-com.aspose.note.RichText-) | Haalt op of stelt een tekenreeksrepresentatie van de datum in de titel in. |
| [setTitleText(RichText value)](#setTitleText-com.aspose.note.RichText-) | Haalt op of stelt de tekst van de titel in. |
| [setTitleTime(RichText value)](#setTitleTime-com.aspose.note.RichText-) | Haalt op of stelt een tekenreeksrepresentatie van de tijd in de titel in. |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | Haalt op of stelt de verticale offset in. |
### Title() {#Title--}
```
public Title()
```


Initialiseert een nieuw exemplaar van de `Title`-klasse.

### &lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass) {#-T1-getChildNodes-java.lang.Class-T1--}
```
public List<T1> <T1>getChildNodes(Class<T1> typeParameterClass)
```


Haalt alle kindknopen op op basis van het knooptype.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| typeParameterClass | java.lang.Class&lt;T1&gt; |  |

**Returns:**
java.util.List&lt;T1&gt; - Een lijst van kindknooppunten.

`T1`: Het type van elementen in de geretourneerde lijst.
### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Accepteert de bezoeker van de node.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | Het object van een klasse die afgeleid is van de `DocumentVisitor`. |

### getChildNodes(int type) {#getChildNodes-int-}
```
public List<INode> getChildNodes(int type)
```




**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| type | int |  |

**Returns:**
java.util.List&lt;com.aspose.note.INode&gt;
### getHorizontalOffset() {#getHorizontalOffset--}
```
public final float getHorizontalOffset()
```


Haalt op of stelt de horizontale offset in.

**Returns:**
float
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Haalt op of stelt de laatst gewijzigde tijd in.

**Returns:**
java.util.Date
### getTitleDate() {#getTitleDate--}
```
public final RichText getTitleDate()
```


Haalt op of stelt een tekenreeksrepresentatie van de datum in de titel in.

**Returns:**
[RichText](../../com.aspose.note/richtext)
### getTitleText() {#getTitleText--}
```
public RichText getTitleText()
```


Haalt op of stelt de tekst van de titel in.

**Returns:**
[RichText](../../com.aspose.note/richtext)
### getTitleTime() {#getTitleTime--}
```
public final RichText getTitleTime()
```


Haalt op of stelt een tekenreeksrepresentatie van de tijd in de titel in.

**Returns:**
[RichText](../../com.aspose.note/richtext)
### getVerticalOffset() {#getVerticalOffset--}
```
public final float getVerticalOffset()
```


Haalt op of stelt de verticale offset in.

**Returns:**
float
### isComposite() {#isComposite--}
```
public boolean isComposite()
```


Haalt een waarde op die aangeeft of dit knooppunt samengesteld is. Indien waar kan het knooppunt onderliggende knooppunten hebben.

**Returns:**
boolean
### iterator() {#iterator--}
```
public final System.Collections.Generic.IGenericEnumerator<RichText> iterator()
```


Retourneert een enumerator die door de onderliggende knooppunten van de [Title](../../com.aspose.note/title) iterereert.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.note.RichText&gt; - De IEnumerator.
### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public final void setHorizontalOffset(float value)
```


Haalt op of stelt de horizontale offset in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | float |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Haalt op of stelt de laatst gewijzigde tijd in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.util.Date |  |

### setTitleDate(RichText value) {#setTitleDate-com.aspose.note.RichText-}
```
public final void setTitleDate(RichText value)
```


Haalt op of stelt een tekenreeksrepresentatie van de datum in de titel in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [RichText](../../com.aspose.note/richtext) |  |

### setTitleText(RichText value) {#setTitleText-com.aspose.note.RichText-}
```
public final void setTitleText(RichText value)
```


Haalt op of stelt de tekst van de titel in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [RichText](../../com.aspose.note/richtext) |  |

### setTitleTime(RichText value) {#setTitleTime-com.aspose.note.RichText-}
```
public final void setTitleTime(RichText value)
```


Haalt op of stelt een tekenreeksrepresentatie van de tijd in de titel in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [RichText](../../com.aspose.note/richtext) |  |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public final void setVerticalOffset(float value)
```


Haalt op of stelt de verticale offset in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | float |  |

