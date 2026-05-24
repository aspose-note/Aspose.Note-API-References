---
title: "OutlineElement"
second_title: "Référence d'API Aspose.Note pour Java"
description: "Représente un OutlineElement."
type: docs
weight: 67
url: /fr/java/com.aspose.note/outlineelement/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode, com.aspose.note.IndentatedNode

**All Implemented Interfaces:**
[com.aspose.note.IOutlineChildNode](../../com.aspose.note/ioutlinechildnode), [com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode)
```
public final class OutlineElement extends IndentatedNode<IOutlineElementChildNode,OutlineElement> implements IOutlineChildNode, IOutlineElementChildNode
```

Représente un OutlineElement.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [OutlineElement()](#OutlineElement--) | Initialise une nouvelle instance de la classe `OutlineElement`. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepte le visiteur du nœud. |
| [getAuthorMostRecent()](#getAuthorMostRecent--) | Obtient l'auteur le plus récent d'un élément de plan. |
| [getAuthorOriginal()](#getAuthorOriginal--) | Obtient l'auteur original d'un élément de plan. |
| [getCreationTime()](#getCreationTime--) | Obtient ou définit l'heure de création. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Obtient ou définit l'heure de la dernière modification. |
| [getNumberList()](#getNumberList--) | Obtient ou définit le style de l'en-tête de liste numérotée. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Obtient ou définit l'heure de création. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Obtient ou définit l'heure de la dernière modification. |
| [setNumberList(NumberList value)](#setNumberList-com.aspose.note.NumberList-) | Obtient ou définit le style de l'en-tête de liste numérotée. |
### OutlineElement() {#OutlineElement--}
```
public OutlineElement()
```


Initialise une nouvelle instance de la classe `OutlineElement`.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Accepte le visiteur du nœud.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | L'objet d'une classe dérivée de `DocumentVisitor`. |

### getAuthorMostRecent() {#getAuthorMostRecent--}
```
public final String getAuthorMostRecent()
```


Obtient l'auteur le plus récent d'un élément de plan.

Valeur : L'auteur le plus récent.

**Returns:**
java.lang.String
### getAuthorOriginal() {#getAuthorOriginal--}
```
public final String getAuthorOriginal()
```


Obtient l'auteur original d'un élément de plan.

Valeur : L'auteur original.

**Returns:**
java.lang.String
### getCreationTime() {#getCreationTime--}
```
public Date getCreationTime()
```


Obtient ou définit l'heure de création.

**Returns:**
java.util.Date
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Obtient ou définit l'heure de la dernière modification.

**Returns:**
java.util.Date
### getNumberList() {#getNumberList--}
```
public NumberList getNumberList()
```


Obtient ou définit le style de l'en-tête de liste numérotée.

**Returns:**
[NumberList](../../com.aspose.note/numberlist)
### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public void setCreationTime(Date value)
```


Obtient ou définit l'heure de création.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.Date |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Obtient ou définit l'heure de la dernière modification.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.Date |  |

### setNumberList(NumberList value) {#setNumberList-com.aspose.note.NumberList-}
```
public void setNumberList(NumberList value)
```


Obtient ou définit le style de l'en-tête de liste numérotée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [NumberList](../../com.aspose.note/numberlist) |  |

