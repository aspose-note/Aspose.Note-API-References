---
title: "Title"
second_title: "Riferimento API di Aspose.Note per Java"
description: "Rappresenta un titolo."
type: docs
weight: 95
url: /it/java/com.aspose.note/title/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase)

**All Implemented Interfaces:**
com.aspose.note.ICompositeNodeT, [com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode)
```
public final class Title extends CompositeNodeBase implements ICompositeNodeT<RichText>, IPageChildNode
```

Rappresenta un titolo.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [Title()](#Title--) | Inizializza una nuova istanza della classe `Title`. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [&lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass)](#-T1-getChildNodes-java.lang.Class-T1--) | Ottieni tutti i nodi figli per tipo di nodo. |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accetta il visitatore del nodo. |
| [getChildNodes(int type)](#getChildNodes-int-) |  |
| [getHorizontalOffset()](#getHorizontalOffset--) | Ottiene o imposta lo spostamento orizzontale. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Ottiene o imposta l'ora dell'ultima modifica. |
| [getTitleDate()](#getTitleDate--) | Ottiene o imposta una rappresentazione stringa della data nel titolo. |
| [getTitleText()](#getTitleText--) | Ottiene o imposta il testo del titolo. |
| [getTitleTime()](#getTitleTime--) | Ottiene o imposta una rappresentazione stringa dell'ora nel titolo. |
| [getVerticalOffset()](#getVerticalOffset--) | Ottiene o imposta lo spostamento verticale. |
| [isComposite()](#isComposite--) | Ottiene un valore che indica se questo nodo è composito. |
| [iterator()](#iterator--) | Restituisce un enumeratore che itera attraverso i nodi figli del [Title](../../com.aspose.note/title). |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | Ottiene o imposta lo spostamento orizzontale. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Ottiene o imposta l'ora dell'ultima modifica. |
| [setTitleDate(RichText value)](#setTitleDate-com.aspose.note.RichText-) | Ottiene o imposta una rappresentazione stringa della data nel titolo. |
| [setTitleText(RichText value)](#setTitleText-com.aspose.note.RichText-) | Ottiene o imposta il testo del titolo. |
| [setTitleTime(RichText value)](#setTitleTime-com.aspose.note.RichText-) | Ottiene o imposta una rappresentazione stringa dell'ora nel titolo. |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | Ottiene o imposta lo spostamento verticale. |
### Title() {#Title--}
```
public Title()
```


Inizializza una nuova istanza della classe `Title`.

### &lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass) {#-T1-getChildNodes-java.lang.Class-T1--}
```
public List<T1> <T1>getChildNodes(Class<T1> typeParameterClass)
```


Ottieni tutti i nodi figli per tipo di nodo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| typeParameterClass | java.lang.Class&lt;T1&gt; |  |

**Returns:**
java.util.List&lt;T1&gt; - Un elenco di nodi figli.

`T1`: Il tipo di elementi nella lista restituita.
### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Accetta il visitatore del nodo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | L'oggetto di una classe derivata da `DocumentVisitor`. |

### getChildNodes(int type) {#getChildNodes-int-}
```
public List<INode> getChildNodes(int type)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| tipo | int |  |

**Returns:**
java.util.List&lt;com.aspose.note.INode&gt;
### getHorizontalOffset() {#getHorizontalOffset--}
```
public final float getHorizontalOffset()
```


Ottiene o imposta lo spostamento orizzontale.

**Returns:**
float
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Ottiene o imposta l'ora dell'ultima modifica.

**Returns:**
java.util.Date
### getTitleDate() {#getTitleDate--}
```
public final RichText getTitleDate()
```


Ottiene o imposta una rappresentazione stringa della data nel titolo.

**Returns:**
[RichText](../../com.aspose.note/richtext)
### getTitleText() {#getTitleText--}
```
public RichText getTitleText()
```


Ottiene o imposta il testo del titolo.

**Returns:**
[RichText](../../com.aspose.note/richtext)
### getTitleTime() {#getTitleTime--}
```
public final RichText getTitleTime()
```


Ottiene o imposta una rappresentazione stringa dell'ora nel titolo.

**Returns:**
[RichText](../../com.aspose.note/richtext)
### getVerticalOffset() {#getVerticalOffset--}
```
public final float getVerticalOffset()
```


Ottiene o imposta lo spostamento verticale.

**Returns:**
float
### isComposite() {#isComposite--}
```
public boolean isComposite()
```


Ottiene un valore che indica se questo nodo è composito. Se vero, il nodo può avere nodi figli.

**Returns:**
boolean
### iterator() {#iterator--}
```
public final System.Collections.Generic.IGenericEnumerator<RichText> iterator()
```


Restituisce un enumeratore che itera attraverso i nodi figli del [Title](../../com.aspose.note/title).

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.note.RichText&gt; - L' IEnumerator.
### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public final void setHorizontalOffset(float value)
```


Ottiene o imposta lo spostamento orizzontale.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | float |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Ottiene o imposta l'ora dell'ultima modifica.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.util.Date |  |

### setTitleDate(RichText value) {#setTitleDate-com.aspose.note.RichText-}
```
public final void setTitleDate(RichText value)
```


Ottiene o imposta una rappresentazione stringa della data nel titolo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [RichText](../../com.aspose.note/richtext) |  |

### setTitleText(RichText value) {#setTitleText-com.aspose.note.RichText-}
```
public final void setTitleText(RichText value)
```


Ottiene o imposta il testo del titolo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [RichText](../../com.aspose.note/richtext) |  |

### setTitleTime(RichText value) {#setTitleTime-com.aspose.note.RichText-}
```
public final void setTitleTime(RichText value)
```


Ottiene o imposta una rappresentazione stringa dell'ora nel titolo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [RichText](../../com.aspose.note/richtext) |  |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public final void setVerticalOffset(float value)
```


Ottiene o imposta lo spostamento verticale.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | float |  |

