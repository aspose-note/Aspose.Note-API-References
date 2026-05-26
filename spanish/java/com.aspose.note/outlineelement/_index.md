---
title: "OutlineElement"
second_title: "Referencia de API de Aspose.Note para Java"
description: "Representa un OutlineElement."
type: docs
weight: 67
url: /es/java/com.aspose.note/outlineelement/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode, com.aspose.note.IndentatedNode

**All Implemented Interfaces:**
[com.aspose.note.IOutlineChildNode](../../com.aspose.note/ioutlinechildnode), [com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode)
```
public final class OutlineElement extends IndentatedNode<IOutlineElementChildNode,OutlineElement> implements IOutlineChildNode, IOutlineElementChildNode
```

Representa un OutlineElement.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [OutlineElement()](#OutlineElement--) | Inicializa una nueva instancia de la clase `OutlineElement`. |
## Métodos

| Método | Descripción |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Acepta al visitante del nodo. |
| [getAuthorMostRecent()](#getAuthorMostRecent--) | Obtiene el autor más reciente de un elemento de esquema. |
| [getAuthorOriginal()](#getAuthorOriginal--) | Obtiene el autor original de un elemento de esquema. |
| [getCreationTime()](#getCreationTime--) | Obtiene o establece la hora de creación. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Obtiene o establece la hora de la última modificación. |
| [getNumberList()](#getNumberList--) | Obtiene o establece el estilo para el encabezado de la lista numerada. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Obtiene o establece la hora de creación. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Obtiene o establece la hora de la última modificación. |
| [setNumberList(NumberList value)](#setNumberList-com.aspose.note.NumberList-) | Obtiene o establece el estilo para el encabezado de la lista numerada. |
### OutlineElement() {#OutlineElement--}
```
public OutlineElement()
```


Inicializa una nueva instancia de la clase `OutlineElement`.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Acepta al visitante del nodo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | El objeto de una clase derivada de `DocumentVisitor`. |

### getAuthorMostRecent() {#getAuthorMostRecent--}
```
public final String getAuthorMostRecent()
```


Obtiene el autor más reciente de un elemento de esquema.

Valor: El autor más reciente.

**Returns:**
java.lang.String
### getAuthorOriginal() {#getAuthorOriginal--}
```
public final String getAuthorOriginal()
```


Obtiene el autor original de un elemento de esquema.

Valor: El autor original.

**Returns:**
java.lang.String
### getCreationTime() {#getCreationTime--}
```
public Date getCreationTime()
```


Obtiene o establece la hora de creación.

**Returns:**
java.util.Date
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Obtiene o establece la hora de la última modificación.

**Returns:**
java.util.Date
### getNumberList() {#getNumberList--}
```
public NumberList getNumberList()
```


Obtiene o establece el estilo para el encabezado de la lista numerada.

**Returns:**
[NumberList](../../com.aspose.note/numberlist)
### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public void setCreationTime(Date value)
```


Obtiene o establece la hora de creación.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.Date |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Obtiene o establece la hora de la última modificación.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.Date |  |

### setNumberList(NumberList value) {#setNumberList-com.aspose.note.NumberList-}
```
public void setNumberList(NumberList value)
```


Obtiene o establece el estilo para el encabezado de la lista numerada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [NumberList](../../com.aspose.note/numberlist) |  |

