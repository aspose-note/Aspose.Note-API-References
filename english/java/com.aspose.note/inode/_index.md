---
title: INode
second_title: Aspose.Note for Java API Reference
description: The interface for all nodes of an Aspose.Note document.
type: docs
weight: 102
url: /java/com.aspose.note/inode/
---
```
public interface INode
```

The interface for all nodes of an Aspose.Note document.
## Methods

| Method | Description |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) |  |
| [getNextSibling()](#getNextSibling--) |  |
| [getPreviousSibling()](#getPreviousSibling--) |  |
### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public abstract void accept(DocumentVisitor visitor)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) |  |

### getNextSibling() {#getNextSibling--}
```
public abstract INode getNextSibling()
```




**Returns:**
[INode](../../com.aspose.note/inode)
### getPreviousSibling() {#getPreviousSibling--}
```
public abstract INode getPreviousSibling()
```




**Returns:**
[INode](../../com.aspose.note/inode)
