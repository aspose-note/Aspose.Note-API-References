---
title: "NœudIndenté"
second_title: "Référence d'API Aspose.Note pour Java"
description: "La classe de base pour les nœuds avec une indentation relative pour les nœuds enfants."
type: docs
weight: 37
url: /fr/java/com.aspose.note/indentatednode/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode

**All Implemented Interfaces:**
com.aspose.note.IIndentatedNodeExtended
```
public class IndentatedNode<T,Self> extends CompositeNode<T> implements IIndentatedNodeExtended
```

La classe de base pour les nœuds avec une indentation relative pour les nœuds enfants.

`T`: Le type des éléments dans le nœud composite.

T :
Self :
## Méthodes

| Méthode | Description |
| --- | --- |
| [getIndentPosition()](#getIndentPosition--) | Obtient ou définit la position de l'indentation. |
| [getInternalIndentPosition()](#getInternalIndentPosition--) | Obtient le nombre d'éléments à additionner dans le tableau RgOutlineIndentDistance pour obtenir la taille de l'indentation. |
| [setIndentPosition(byte value)](#setIndentPosition-byte-) | Obtient ou définit la position de l'indentation. |
| [setIndentPosition(int value)](#setIndentPosition-int-) |  |
### getIndentPosition() {#getIndentPosition--}
```
public final byte getIndentPosition()
```


Obtient ou définit la position de l'indentation.

**Returns:**
byte
### getInternalIndentPosition() {#getInternalIndentPosition--}
```
public int getInternalIndentPosition()
```


Obtient le nombre d'éléments à additionner dans le tableau RgOutlineIndentDistance pour obtenir la taille de l'indentation.

**Returns:**
int
### setIndentPosition(byte value) {#setIndentPosition-byte-}
```
public final Self setIndentPosition(byte value)
```


Obtient ou définit la position de l'indentation.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | byte |  |

**Returns:**
Self
### setIndentPosition(int value) {#setIndentPosition-int-}
```
public final Self setIndentPosition(int value)
```




**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int |  |

**Returns:**
Self
