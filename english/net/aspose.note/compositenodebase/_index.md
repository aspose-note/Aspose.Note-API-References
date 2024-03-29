---
title: Class CompositeNodeBase
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.CompositeNodeBase class. The nongeneric class for nodes that can contain other nodes
type: docs
weight: 30
url: /net/aspose.note/compositenodebase/
---
## CompositeNodeBase class

The non-generic class for nodes that can contain other nodes.

```csharp
public abstract class CompositeNodeBase : Node, ICompositeNode
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
| abstract [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenodebase/getchildnodes/#getchildnodes_1)() | Get all child nodes by the node type. |

### See Also

* class [Node](../node/)
* interface [ICompositeNode](../icompositenode/)
* namespace [Aspose.Note](../../aspose.note/)
* assembly [Aspose.Note](../../)


