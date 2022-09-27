---
title: INode
second_title: Aspose.Note for Java API Reference
description: The interface for all nodes of an Aspose.Note document.
type: docs
weight: 85
url: /java/com.aspose.note/inode/
---
```
public interface INode
```

The interface for all nodes of an Aspose.Note document.
## Methods

| Method | Description |
| --- | --- |
| [getPreviousSibling()](#getPreviousSibling--) |  |
| [getNextSibling()](#getNextSibling--) |  |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) |  |
### getPreviousSibling() {#getPreviousSibling--}
```
public abstract INode getPreviousSibling()
```




**Returns:**
[INode](../../com.aspose.note/inode)
### getNextSibling() {#getNextSibling--}
```
public abstract INode getNextSibling()
```




**Returns:**
[INode](../../com.aspose.note/inode)
### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public abstract void accept(DocumentVisitor visitor)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) |  |

