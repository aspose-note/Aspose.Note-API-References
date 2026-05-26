---
title: "TableCell"
second_title: "Referencia de API de Aspose.Note para Java"
description: "Representa una celda de tabla."
type: docs
weight: 88
url: /es/java/com.aspose.note/tablecell/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode, com.aspose.note.IndentatedNode
```
public final class TableCell extends IndentatedNode<IOutlineChildNode,TableCell>
```

Representa una celda de tabla.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [TableCell()](#TableCell--) | Inicializa una nueva instancia de la clase `TableCell`. |
## Métodos

| Método | Descripción |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Acepta al visitante del nodo. |
| [getBackgroundColor()](#getBackgroundColor--) | Obtiene el color de fondo. |
| [getInternalIndentPosition()](#getInternalIndentPosition--) |  |
| [getLastModifiedTime()](#getLastModifiedTime--) | Obtiene o establece la hora de la última modificación. |
| [getMaxWidth()](#getMaxWidth--) | Obtiene el ancho máximo. |
| [setBackgroundColor(Color value)](#setBackgroundColor-java.awt.Color-) | Establece el color de fondo. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Obtiene o establece la hora de la última modificación. |
### TableCell() {#TableCell--}
```
public TableCell()
```


Inicializa una nueva instancia de la clase `TableCell`.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Acepta al visitante del nodo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | El objeto de una clase derivada de `DocumentVisitor`. |

### getBackgroundColor() {#getBackgroundColor--}
```
public Color getBackgroundColor()
```


Obtiene el color de fondo.

**Returns:**
java.awt.Color
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
### getMaxWidth() {#getMaxWidth--}
```
public float getMaxWidth()
```


Obtiene el ancho máximo.

**Returns:**
float
### setBackgroundColor(Color value) {#setBackgroundColor-java.awt.Color-}
```
public void setBackgroundColor(Color value)
```


Establece el color de fondo.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.awt.Color |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Obtiene o establece la hora de la última modificación.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.Date |  |

