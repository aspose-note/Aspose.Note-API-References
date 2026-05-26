---
title: "Node"
second_title: "Справочник API Aspose.Note for Java"
description: "Базовый класс для всех узлов документа Aspose.Note."
type: docs
weight: 51
url: /ru/java/com.aspose.note/node/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.note.INode](../../com.aspose.note/inode)
```
public abstract class Node implements INode
```

Базовый класс для всех узлов документа Aspose.Note.
## Методы

| Метод | Описание |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Принимает посетителя узла. |
| [getDocument()](#getDocument--) | Получает документ узла. |
| [getNextSibling()](#getNextSibling--) | Получает следующий узел на том же уровне дерева узлов. |
| [getNodeId()](#getNodeId--) | Получает идентификатор узла. |
| [getNodeType()](#getNodeType--) | Получает тип узла. |
| [getParentNode()](#getParentNode--) | Получает родительский узел. |
| [getPreviousSibling()](#getPreviousSibling--) | Получает предыдущий узел на том же уровне дерева узлов. |
| [isComposite()](#isComposite--) | Получает значение, указывающее, является ли этот узел составным. |
### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public abstract void accept(DocumentVisitor visitor)
```


Принимает посетителя узла.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | Объект класса, производного от `DocumentVisitor`. |

### getDocument() {#getDocument--}
```
public Document getDocument()
```


Получает документ узла.

Значение: Документ.

**Returns:**
[Document](../../com.aspose.note/document)
### getNextSibling() {#getNextSibling--}
```
public INode getNextSibling()
```


Получает следующий узел на том же уровне дерева узлов.

Значение: Следующий соседний элемент.

**Returns:**
[INode](../../com.aspose.note/inode)
### getNodeId() {#getNodeId--}
```
public ExtendedGuid getNodeId()
```


Получает идентификатор узла.

**Returns:**
[ExtendedGuid](../../com.aspose.note.revision.types/extendedguid)
### getNodeType() {#getNodeType--}
```
public int getNodeType()
```


Получает тип узла.

**Returns:**
int
### getParentNode() {#getParentNode--}
```
public ICompositeNode getParentNode()
```


Получает родительский узел.

**Returns:**
[ICompositeNode](../../com.aspose.note/icompositenode)
### getPreviousSibling() {#getPreviousSibling--}
```
public INode getPreviousSibling()
```


Получает предыдущий узел на том же уровне дерева узлов.

Значение: Предыдущий соседний элемент.

**Returns:**
[INode](../../com.aspose.note/inode)
### isComposite() {#isComposite--}
```
public boolean isComposite()
```


Получает значение, указывающее, является ли этот узел составным. Если true, узел может иметь дочерние узлы.

**Returns:**
boolean
