---
title: "Plan"
second_title: "Référence d'API Aspose.Note pour Java"
description: "Représente un plan."
type: docs
weight: 66
url: /fr/java/com.aspose.note/outline/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode, com.aspose.note.IndentatedNode

**All Implemented Interfaces:**
[com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode)
```
public final class Outline extends IndentatedNode<IOutlineChildNode,Outline> implements IPageChildNode
```

Représente un plan.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [Outline()](#Outline--) | Initialise une nouvelle instance de la classe [Outline](../../com.aspose.note/outline). |
## Méthodes

| Méthode | Description |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepte le visiteur du nœud. |
| [getDescendantsCannotBeMoved()](#getDescendantsCannotBeMoved--) | Obtient si les descendants du plan peuvent être déplacés. |
| [getHorizontalOffset()](#getHorizontalOffset--) | Obtient ou définit le décalage horizontal. |
| [getInternalIndentPosition()](#getInternalIndentPosition--) |  |
| [getLastModifiedTime()](#getLastModifiedTime--) | Obtient ou définit l'heure de la dernière modification. |
| [getMaxHeight()](#getMaxHeight--) | Obtient ou définit la hauteur maximale. |
| [getMaxWidth()](#getMaxWidth--) | Obtient ou définit la largeur maximale. |
| [getMinWidth()](#getMinWidth--) | Obtient ou définit la largeur minimale. |
| [getReservedWidth()](#getReservedWidth--) | Obtient ou définit la largeur réservée. |
| [getVerticalOffset()](#getVerticalOffset--) | Obtient ou définit le décalage vertical. |
| [setDescendantsCannotBeMoved(boolean value)](#setDescendantsCannotBeMoved-boolean-) | Obtient si les descendants du plan peuvent être déplacés. |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | Obtient ou définit le décalage horizontal. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Obtient ou définit l'heure de la dernière modification. |
| [setMaxHeight(float value)](#setMaxHeight-float-) | Obtient ou définit la hauteur maximale. |
| [setMaxWidth(float value)](#setMaxWidth-float-) | Obtient ou définit la largeur maximale. |
| [setMinWidth(float value)](#setMinWidth-float-) | Obtient ou définit la largeur minimale. |
| [setReservedWidth(float value)](#setReservedWidth-float-) | Obtient ou définit la largeur réservée. |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | Obtient ou définit le décalage vertical. |
### Outline() {#Outline--}
```
public Outline()
```


Initialise une nouvelle instance de la classe [Outline](../../com.aspose.note/outline).

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Accepte le visiteur du nœud.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | L'objet d'une classe dérivée de `DocumentVisitor`. |

### getDescendantsCannotBeMoved() {#getDescendantsCannotBeMoved--}
```
public boolean getDescendantsCannotBeMoved()
```


Obtient si les descendants du plan peuvent être déplacés.

**Returns:**
boolean
### getHorizontalOffset() {#getHorizontalOffset--}
```
public float getHorizontalOffset()
```


Obtient ou définit le décalage horizontal.

**Returns:**
float
### getInternalIndentPosition() {#getInternalIndentPosition--}
```
public int getInternalIndentPosition()
```


Obtient le nombre d'éléments à additionner dans le tableau RgOutlineIndentDistance pour obtenir la taille de l'indentation.

**Returns:**
int
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Obtient ou définit l'heure de la dernière modification.

**Returns:**
java.util.Date
### getMaxHeight() {#getMaxHeight--}
```
public float getMaxHeight()
```


Obtient ou définit la hauteur maximale.

**Returns:**
float
### getMaxWidth() {#getMaxWidth--}
```
public float getMaxWidth()
```


Obtient ou définit la largeur maximale.

**Returns:**
float
### getMinWidth() {#getMinWidth--}
```
public float getMinWidth()
```


Obtient ou définit la largeur minimale.

**Returns:**
float
### getReservedWidth() {#getReservedWidth--}
```
public float getReservedWidth()
```


Obtient ou définit la largeur réservée.

**Returns:**
float
### getVerticalOffset() {#getVerticalOffset--}
```
public float getVerticalOffset()
```


Obtient ou définit le décalage vertical.

**Returns:**
float
### setDescendantsCannotBeMoved(boolean value) {#setDescendantsCannotBeMoved-boolean-}
```
public void setDescendantsCannotBeMoved(boolean value)
```


Obtient si les descendants du plan peuvent être déplacés.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public void setHorizontalOffset(float value)
```


Obtient ou définit le décalage horizontal.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | float |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Obtient ou définit l'heure de la dernière modification.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.Date |  |

### setMaxHeight(float value) {#setMaxHeight-float-}
```
public void setMaxHeight(float value)
```


Obtient ou définit la hauteur maximale.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | float |  |

### setMaxWidth(float value) {#setMaxWidth-float-}
```
public void setMaxWidth(float value)
```


Obtient ou définit la largeur maximale.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | float |  |

### setMinWidth(float value) {#setMinWidth-float-}
```
public void setMinWidth(float value)
```


Obtient ou définit la largeur minimale.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | float |  |

### setReservedWidth(float value) {#setReservedWidth-float-}
```
public void setReservedWidth(float value)
```


Obtient ou définit la largeur réservée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | float |  |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public void setVerticalOffset(float value)
```


Obtient ou définit le décalage vertical.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | float |  |

