---
title: "Title"
second_title: "Aspose.Note für Java API-Referenz"
description: "Stellt einen Titel dar."
type: docs
weight: 95
url: /de/java/com.aspose.note/title/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase)

**All Implemented Interfaces:**
com.aspose.note.ICompositeNodeT, [com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode)
```
public final class Title extends CompositeNodeBase implements ICompositeNodeT<RichText>, IPageChildNode
```

Stellt einen Titel dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [Title()](#Title--) | Initialisiert eine neue Instanz der `Title`-Klasse. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [&lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass)](#-T1-getChildNodes-java.lang.Class-T1--) | Ruft alle untergeordneten Knoten nach Knotentyp ab. |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Akzeptiert den Besucher des Knotens. |
| [getChildNodes(int type)](#getChildNodes-int-) |  |
| [getHorizontalOffset()](#getHorizontalOffset--) | Liest oder setzt den horizontalen Versatz. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Liest oder setzt die zuletzt geänderte Zeit. |
| [getTitleDate()](#getTitleDate--) | Ermittelt oder setzt die Zeichenkettenrepräsentation des Datums im Titel. |
| [getTitleText()](#getTitleText--) | Ermittelt oder setzt den Text des Titels. |
| [getTitleTime()](#getTitleTime--) | Ermittelt oder setzt die Zeichenkettenrepräsentation der Zeit im Titel. |
| [getVerticalOffset()](#getVerticalOffset--) | Liest oder setzt den vertikalen Versatz. |
| [isComposite()](#isComposite--) | Ermittelt einen Wert, der angibt, ob dieser Knoten zusammengesetzt ist. |
| [iterator()](#iterator--) | Gibt einen Enumerator zurück, der die Kindknoten des [Title](../../com.aspose.note/title) durchläuft. |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | Liest oder setzt den horizontalen Versatz. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Liest oder setzt die zuletzt geänderte Zeit. |
| [setTitleDate(RichText value)](#setTitleDate-com.aspose.note.RichText-) | Ermittelt oder setzt die Zeichenkettenrepräsentation des Datums im Titel. |
| [setTitleText(RichText value)](#setTitleText-com.aspose.note.RichText-) | Ermittelt oder setzt den Text des Titels. |
| [setTitleTime(RichText value)](#setTitleTime-com.aspose.note.RichText-) | Ermittelt oder setzt die Zeichenkettenrepräsentation der Zeit im Titel. |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | Liest oder setzt den vertikalen Versatz. |
### Title() {#Title--}
```
public Title()
```


Initialisiert eine neue Instanz der `Title`-Klasse.

### &lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass) {#-T1-getChildNodes-java.lang.Class-T1--}
```
public List<T1> <T1>getChildNodes(Class<T1> typeParameterClass)
```


Ruft alle untergeordneten Knoten nach Knotentyp ab.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| typeParameterClass | java.lang.Class&lt;T1&gt; |  |

**Returns:**
java.util.List&lt;T1&gt; - Eine Liste von Kindknoten.

`T1`: Der Typ der Elemente in der zurückgegebenen Liste.
### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Akzeptiert den Besucher des Knotens.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | Das Objekt einer Klasse, die von `DocumentVisitor` abgeleitet ist. |

### getChildNodes(int type) {#getChildNodes-int-}
```
public List<INode> getChildNodes(int type)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| type | int |  |

**Returns:**
java.util.List&lt;com.aspose.note.INode&gt;
### getHorizontalOffset() {#getHorizontalOffset--}
```
public final float getHorizontalOffset()
```


Liest oder setzt den horizontalen Versatz.

**Returns:**
float
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Liest oder setzt die zuletzt geänderte Zeit.

**Returns:**
java.util.Date
### getTitleDate() {#getTitleDate--}
```
public final RichText getTitleDate()
```


Ermittelt oder setzt die Zeichenkettenrepräsentation des Datums im Titel.

**Returns:**
[RichText](../../com.aspose.note/richtext)
### getTitleText() {#getTitleText--}
```
public RichText getTitleText()
```


Ermittelt oder setzt den Text des Titels.

**Returns:**
[RichText](../../com.aspose.note/richtext)
### getTitleTime() {#getTitleTime--}
```
public final RichText getTitleTime()
```


Ermittelt oder setzt die Zeichenkettenrepräsentation der Zeit im Titel.

**Returns:**
[RichText](../../com.aspose.note/richtext)
### getVerticalOffset() {#getVerticalOffset--}
```
public final float getVerticalOffset()
```


Liest oder setzt den vertikalen Versatz.

**Returns:**
float
### isComposite() {#isComposite--}
```
public boolean isComposite()
```


Ermittelt einen Wert, der angibt, ob dieser Knoten zusammengesetzt ist. Wenn true, kann der Knoten Kindknoten haben.

**Returns:**
boolean
### iterator() {#iterator--}
```
public final System.Collections.Generic.IGenericEnumerator<RichText> iterator()
```


Gibt einen Enumerator zurück, der die Kindknoten des [Title](../../com.aspose.note/title) durchläuft.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.note.RichText&gt; - Der IEnumerator.
### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public final void setHorizontalOffset(float value)
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

### setTitleDate(RichText value) {#setTitleDate-com.aspose.note.RichText-}
```
public final void setTitleDate(RichText value)
```


Ermittelt oder setzt die Zeichenkettenrepräsentation des Datums im Titel.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [RichText](../../com.aspose.note/richtext) |  |

### setTitleText(RichText value) {#setTitleText-com.aspose.note.RichText-}
```
public final void setTitleText(RichText value)
```


Ermittelt oder setzt den Text des Titels.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [RichText](../../com.aspose.note/richtext) |  |

### setTitleTime(RichText value) {#setTitleTime-com.aspose.note.RichText-}
```
public final void setTitleTime(RichText value)
```


Ermittelt oder setzt die Zeichenkettenrepräsentation der Zeit im Titel.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [RichText](../../com.aspose.note/richtext) |  |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public final void setVerticalOffset(float value)
```


Liest oder setzt den vertikalen Versatz.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | float |  |

