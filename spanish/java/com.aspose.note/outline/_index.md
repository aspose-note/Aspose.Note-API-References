---
title: "Esquema"
second_title: "Referencia de API de Aspose.Note para Java"
description: "Representa un esquema."
type: docs
weight: 66
url: /es/java/com.aspose.note/outline/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode, com.aspose.note.IndentatedNode

**All Implemented Interfaces:**
[com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode)
```
public final class Outline extends IndentatedNode<IOutlineChildNode,Outline> implements IPageChildNode
```

Representa un esquema.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [Outline()](#Outline--) | Inicializa una nueva instancia de la clase [Outline](../../com.aspose.note/outline). |
## Métodos

| Método | Descripción |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Acepta al visitante del nodo. |
| [getDescendantsCannotBeMoved()](#getDescendantsCannotBeMoved--) | Obtiene si los descendientes del esquema pueden moverse. |
| [getHorizontalOffset()](#getHorizontalOffset--) | Obtiene o establece el desplazamiento horizontal. |
| [getInternalIndentPosition()](#getInternalIndentPosition--) |  |
| [getLastModifiedTime()](#getLastModifiedTime--) | Obtiene o establece la hora de la última modificación. |
| [getMaxHeight()](#getMaxHeight--) | Obtiene o establece la altura máxima. |
| [getMaxWidth()](#getMaxWidth--) | Obtiene o establece el ancho máximo. |
| [getMinWidth()](#getMinWidth--) | Obtiene o establece el ancho mínimo. |
| [getReservedWidth()](#getReservedWidth--) | Obtiene o establece el ancho reservado. |
| [getVerticalOffset()](#getVerticalOffset--) | Obtiene o establece el desplazamiento vertical. |
| [setDescendantsCannotBeMoved(boolean value)](#setDescendantsCannotBeMoved-boolean-) | Obtiene si los descendientes del esquema pueden moverse. |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | Obtiene o establece el desplazamiento horizontal. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Obtiene o establece la hora de la última modificación. |
| [setMaxHeight(float value)](#setMaxHeight-float-) | Obtiene o establece la altura máxima. |
| [setMaxWidth(float value)](#setMaxWidth-float-) | Obtiene o establece el ancho máximo. |
| [setMinWidth(float value)](#setMinWidth-float-) | Obtiene o establece el ancho mínimo. |
| [setReservedWidth(float value)](#setReservedWidth-float-) | Obtiene o establece el ancho reservado. |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | Obtiene o establece el desplazamiento vertical. |
### Outline() {#Outline--}
```
public Outline()
```


Inicializa una nueva instancia de la clase [Outline](../../com.aspose.note/outline).

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Acepta al visitante del nodo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | El objeto de una clase derivada de `DocumentVisitor`. |

### getDescendantsCannotBeMoved() {#getDescendantsCannotBeMoved--}
```
public boolean getDescendantsCannotBeMoved()
```


Obtiene si los descendientes del esquema pueden moverse.

**Returns:**
boolean
### getHorizontalOffset() {#getHorizontalOffset--}
```
public float getHorizontalOffset()
```


Obtiene o establece el desplazamiento horizontal.

**Returns:**
float
### getInternalIndentPosition() {#getInternalIndentPosition--}
```
public int getInternalIndentPosition()
```


Obtiene la cantidad de elementos a sumar en la matriz RgOutlineIndentDistance para obtener el tamaño de sangría.

**Returns:**
int
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Obtiene o establece la hora de la última modificación.

**Returns:**
java.util.Date
### getMaxHeight() {#getMaxHeight--}
```
public float getMaxHeight()
```


Obtiene o establece la altura máxima.

**Returns:**
float
### getMaxWidth() {#getMaxWidth--}
```
public float getMaxWidth()
```


Obtiene o establece el ancho máximo.

**Returns:**
float
### getMinWidth() {#getMinWidth--}
```
public float getMinWidth()
```


Obtiene o establece el ancho mínimo.

**Returns:**
float
### getReservedWidth() {#getReservedWidth--}
```
public float getReservedWidth()
```


Obtiene o establece el ancho reservado.

**Returns:**
float
### getVerticalOffset() {#getVerticalOffset--}
```
public float getVerticalOffset()
```


Obtiene o establece el desplazamiento vertical.

**Returns:**
float
### setDescendantsCannotBeMoved(boolean value) {#setDescendantsCannotBeMoved-boolean-}
```
public void setDescendantsCannotBeMoved(boolean value)
```


Obtiene si los descendientes del esquema pueden moverse.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean |  |

### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public void setHorizontalOffset(float value)
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

### setMaxHeight(float value) {#setMaxHeight-float-}
```
public void setMaxHeight(float value)
```


Obtiene o establece la altura máxima.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | float |  |

### setMaxWidth(float value) {#setMaxWidth-float-}
```
public void setMaxWidth(float value)
```


Obtiene o establece el ancho máximo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | float |  |

### setMinWidth(float value) {#setMinWidth-float-}
```
public void setMinWidth(float value)
```


Obtiene o establece el ancho mínimo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | float |  |

### setReservedWidth(float value) {#setReservedWidth-float-}
```
public void setReservedWidth(float value)
```


Obtiene o establece el ancho reservado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | float |  |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public void setVerticalOffset(float value)
```


Obtiene o establece el desplazamiento vertical.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | float |  |

