---
title: "TableCell"
second_title: "Référence d'API Aspose.Note pour Java"
description: "Représente une cellule de tableau."
type: docs
weight: 88
url: /fr/java/com.aspose.note/tablecell/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode, com.aspose.note.IndentatedNode
```
public final class TableCell extends IndentatedNode<IOutlineChildNode,TableCell>
```

Représente une cellule de tableau.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [TableCell()](#TableCell--) | Initialise une nouvelle instance de la classe `TableCell`. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepte le visiteur du nœud. |
| [getBackgroundColor()](#getBackgroundColor--) | Obtient la couleur d'arrière-plan. |
| [getInternalIndentPosition()](#getInternalIndentPosition--) |  |
| [getLastModifiedTime()](#getLastModifiedTime--) | Obtient ou définit l'heure de la dernière modification. |
| [getMaxWidth()](#getMaxWidth--) | Obtient la largeur maximale. |
| [setBackgroundColor(Color value)](#setBackgroundColor-java.awt.Color-) | Définit la couleur d'arrière-plan. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Obtient ou définit l'heure de la dernière modification. |
### TableCell() {#TableCell--}
```
public TableCell()
```


Initialise une nouvelle instance de la classe `TableCell`.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Accepte le visiteur du nœud.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | L'objet d'une classe dérivée de `DocumentVisitor`. |

### getBackgroundColor() {#getBackgroundColor--}
```
public Color getBackgroundColor()
```


Obtient la couleur d'arrière-plan.

**Returns:**
java.awt.Color
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
### getMaxWidth() {#getMaxWidth--}
```
public float getMaxWidth()
```


Obtient la largeur maximale.

**Returns:**
float
### setBackgroundColor(Color value) {#setBackgroundColor-java.awt.Color-}
```
public void setBackgroundColor(Color value)
```


Définit la couleur d'arrière-plan.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.awt.Color |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Obtient ou définit l'heure de la dernière modification.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.Date |  |

