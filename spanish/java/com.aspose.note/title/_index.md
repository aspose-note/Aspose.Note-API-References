---
title: "Title"
second_title: "Referencia de API de Aspose.Note para Java"
description: "Representa un título."
type: docs
weight: 95
url: /es/java/com.aspose.note/title/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase)

**All Implemented Interfaces:**
com.aspose.note.ICompositeNodeT, [com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode)
```
public final class Title extends CompositeNodeBase implements ICompositeNodeT<RichText>, IPageChildNode
```

Representa un título.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [Title()](#Title--) | Inicializa una nueva instancia de la clase `Title`. |
## Métodos

| Método | Descripción |
| --- | --- |
| [&lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass)](#-T1-getChildNodes-java.lang.Class-T1--) | Obtiene todos los nodos hijos por el tipo de nodo. |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Acepta al visitante del nodo. |
| [getChildNodes(int type)](#getChildNodes-int-) |  |
| [getHorizontalOffset()](#getHorizontalOffset--) | Obtiene o establece el desplazamiento horizontal. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Obtiene o establece la hora de la última modificación. |
| [getTitleDate()](#getTitleDate--) | Obtiene o establece una representación en cadena de la fecha en el título. |
| [getTitleText()](#getTitleText--) | Obtiene o establece el texto del título. |
| [getTitleTime()](#getTitleTime--) | Obtiene o establece una representación en cadena del tiempo en el título. |
| [getVerticalOffset()](#getVerticalOffset--) | Obtiene o establece el desplazamiento vertical. |
| [isComposite()](#isComposite--) | Obtiene un valor que indica si este nodo es compuesto. |
| [iterator()](#iterator--) | Devuelve un enumerador que itera a través de los nodos hijos del [Title](../../com.aspose.note/title). |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | Obtiene o establece el desplazamiento horizontal. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Obtiene o establece la hora de la última modificación. |
| [setTitleDate(RichText value)](#setTitleDate-com.aspose.note.RichText-) | Obtiene o establece una representación en cadena de la fecha en el título. |
| [setTitleText(RichText value)](#setTitleText-com.aspose.note.RichText-) | Obtiene o establece el texto del título. |
| [setTitleTime(RichText value)](#setTitleTime-com.aspose.note.RichText-) | Obtiene o establece una representación en cadena del tiempo en el título. |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | Obtiene o establece el desplazamiento vertical. |
### Title() {#Title--}
```
public Title()
```


Inicializa una nueva instancia de la clase `Title`.

### &lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass) {#-T1-getChildNodes-java.lang.Class-T1--}
```
public List<T1> <T1>getChildNodes(Class<T1> typeParameterClass)
```


Obtiene todos los nodos hijos por el tipo de nodo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| typeParameterClass | java.lang.Class&lt;T1&gt; |  |

**Returns:**
java.util.List&lt;T1&gt; - Una lista de nodos hijos.

`T1`: El tipo de elementos en la lista devuelta.
### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Acepta al visitante del nodo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | El objeto de una clase derivada de `DocumentVisitor`. |

### getChildNodes(int type) {#getChildNodes-int-}
```
public List<INode> getChildNodes(int type)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| tipo | int |  |

**Returns:**
java.util.List&lt;com.aspose.note.INode&gt;
### getHorizontalOffset() {#getHorizontalOffset--}
```
public final float getHorizontalOffset()
```


Obtiene o establece el desplazamiento horizontal.

**Returns:**
float
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Obtiene o establece la hora de la última modificación.

**Returns:**
java.util.Date
### getTitleDate() {#getTitleDate--}
```
public final RichText getTitleDate()
```


Obtiene o establece una representación en cadena de la fecha en el título.

**Returns:**
[RichText](../../com.aspose.note/richtext)
### getTitleText() {#getTitleText--}
```
public RichText getTitleText()
```


Obtiene o establece el texto del título.

**Returns:**
[RichText](../../com.aspose.note/richtext)
### getTitleTime() {#getTitleTime--}
```
public final RichText getTitleTime()
```


Obtiene o establece una representación en cadena del tiempo en el título.

**Returns:**
[RichText](../../com.aspose.note/richtext)
### getVerticalOffset() {#getVerticalOffset--}
```
public final float getVerticalOffset()
```


Obtiene o establece el desplazamiento vertical.

**Returns:**
float
### isComposite() {#isComposite--}
```
public boolean isComposite()
```


Obtiene un valor que indica si este nodo es compuesto. Si es verdadero, el nodo puede tener nodos hijos.

**Returns:**
boolean
### iterator() {#iterator--}
```
public final System.Collections.Generic.IGenericEnumerator<RichText> iterator()
```


Devuelve un enumerador que itera a través de los nodos hijos del [Title](../../com.aspose.note/title).

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.note.RichText&gt; - El IEnumerator.
### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public final void setHorizontalOffset(float value)
```


Obtiene o establece el desplazamiento horizontal.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | float |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Obtiene o establece la hora de la última modificación.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.Date |  |

### setTitleDate(RichText value) {#setTitleDate-com.aspose.note.RichText-}
```
public final void setTitleDate(RichText value)
```


Obtiene o establece una representación en cadena de la fecha en el título.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [RichText](../../com.aspose.note/richtext) |  |

### setTitleText(RichText value) {#setTitleText-com.aspose.note.RichText-}
```
public final void setTitleText(RichText value)
```


Obtiene o establece el texto del título.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [RichText](../../com.aspose.note/richtext) |  |

### setTitleTime(RichText value) {#setTitleTime-com.aspose.note.RichText-}
```
public final void setTitleTime(RichText value)
```


Obtiene o establece una representación en cadena del tiempo en el título.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [RichText](../../com.aspose.note/richtext) |  |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public final void setVerticalOffset(float value)
```


Obtiene o establece el desplazamiento vertical.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | float |  |

