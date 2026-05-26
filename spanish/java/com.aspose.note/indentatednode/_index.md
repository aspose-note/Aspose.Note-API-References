---
title: "IndentatedNode"
second_title: "Referencia de API de Aspose.Note para Java"
description: "La clase base para nodos con sangría relativa para nodos hijos."
type: docs
weight: 37
url: /es/java/com.aspose.note/indentatednode/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode

**All Implemented Interfaces:**
com.aspose.note.IIndentatedNodeExtended
```
public class IndentatedNode<T,Self> extends CompositeNode<T> implements IIndentatedNodeExtended
```

La clase base para nodos con sangría relativa para nodos hijos.

`T`: El tipo de elementos en el nodo compuesto.

T :
Self :
## Métodos

| Método | Descripción |
| --- | --- |
| [getIndentPosition()](#getIndentPosition--) | Obtiene o establece la posición de sangría. |
| [getInternalIndentPosition()](#getInternalIndentPosition--) | Obtiene la cantidad de elementos a sumar en la matriz RgOutlineIndentDistance para obtener el tamaño de sangría. |
| [setIndentPosition(byte value)](#setIndentPosition-byte-) | Obtiene o establece la posición de sangría. |
| [setIndentPosition(int value)](#setIndentPosition-int-) |  |
### getIndentPosition() {#getIndentPosition--}
```
public final byte getIndentPosition()
```


Obtiene o establece la posición de sangría.

**Returns:**
byte
### getInternalIndentPosition() {#getInternalIndentPosition--}
```
public int getInternalIndentPosition()
```


Obtiene la cantidad de elementos a sumar en la matriz RgOutlineIndentDistance para obtener el tamaño de sangría.

**Returns:**
int
### setIndentPosition(byte value) {#setIndentPosition-byte-}
```
public final Self setIndentPosition(byte value)
```


Obtiene o establece la posición de sangría.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | byte |  |

**Returns:**
Self
### setIndentPosition(int value) {#setIndentPosition-int-}
```
public final Self setIndentPosition(int value)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int |  |

**Returns:**
Self
