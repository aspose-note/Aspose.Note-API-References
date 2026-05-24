---
title: "Table"
second_title: "Référence d'API Aspose.Note pour Java"
description: "Représente un tableau."
type: docs
weight: 87
url: /fr/java/com.aspose.note/table/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode

**All Implemented Interfaces:**
[com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode), [com.aspose.note.ITaggable](../../com.aspose.note/itaggable)
```
public final class Table extends CompositeNode<TableRow> implements IOutlineElementChildNode, ITaggable
```

Représente un tableau.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [Table()](#Table--) | Initialise une nouvelle instance de la classe `Table`. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepte le visiteur du nœud. |
| [getColumns()](#getColumns--) | Obtient les colonnes du tableau. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Obtient ou définit l'heure de la dernière modification. |
| [getTags()](#getTags--) | Obtient la liste de toutes les balises d'un tableau. |
| [isBordersVisible()](#isBordersVisible--) | Obtient une valeur indiquant si la bordure du tableau est visible. |
| [setBordersVisible(boolean value)](#setBordersVisible-boolean-) | Définit une valeur indiquant si la bordure du tableau est visible. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Obtient ou définit l'heure de la dernière modification. |
### Table() {#Table--}
```
public Table()
```


Initialise une nouvelle instance de la classe `Table`.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Accepte le visiteur du nœud.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | L'objet d'une classe dérivée de `DocumentVisitor`. |

### getColumns() {#getColumns--}
```
public System.Collections.Generic.IGenericList<TableColumn> getColumns()
```


Obtient les colonnes du tableau.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericList&lt;com.aspose.note.TableColumn&gt;
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Obtient ou définit l'heure de la dernière modification.

**Returns:**
java.util.Date
### getTags() {#getTags--}
```
public final System.Collections.Generic.List<ITag> getTags()
```


Obtient la liste de toutes les balises d'un tableau.

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.note.ITag&gt;
### isBordersVisible() {#isBordersVisible--}
```
public boolean isBordersVisible()
```


Obtient une valeur indiquant si la bordure du tableau est visible.

**Returns:**
boolean
### setBordersVisible(boolean value) {#setBordersVisible-boolean-}
```
public void setBordersVisible(boolean value)
```


Définit une valeur indiquant si la bordure du tableau est visible.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Obtient ou définit l'heure de la dernière modification.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.Date |  |

