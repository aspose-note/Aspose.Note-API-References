---
title: Class Node
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.Node class. The base class for all nodes of an Aspose.Note document
type: docs
weight: 130
url: /net/aspose.note/node/
---
## Node class

The base class for all nodes of an Aspose.Note document.

```csharp
public abstract class Node : INode
```

## Properties

| Name | Description |
| --- | --- |
| [Document](../../aspose.note/node/document/) { get; } | Gets the document of the node. |
| virtual [IsComposite](../../aspose.note/node/iscomposite/) { get; } | Gets a value indicating whether this node is composite. If true the node can have child nodes. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Gets the next node at the same node tree level. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Gets the node type. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Gets the parent node. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Gets the previous node at the same node tree level. |

## Methods

| Name | Description |
| --- | --- |
| abstract [Accept](../../aspose.note/node/accept/)(DocumentVisitor) | Accepts the visitor of the node. |

### See Also

* interface [INode](../inode/)
* namespace [Aspose.Note](../../aspose.note/)
* assembly [Aspose.Note](../../)


