---
title: Class CompositeNodeT
second_title: Aspose.Note for .NET API Reference
description: Aspose.Note.CompositeNode1T class. The base generic class for nodes that can contain other nodes
type: docs
weight: 40
url: /net/aspose.note/compositenode-1/
---
## CompositeNode&lt;T&gt; class

The base generic class for nodes that can contain other nodes.

```csharp
public abstract class CompositeNode<T> : CompositeNodeBase, ICompositeNode<T>
    where T : INode
```

| Parameter | Description |
| --- | --- |
| T | The type of elements in the composite node. |

## Properties

| Name | Description |
| --- | --- |
| [Document](../../aspose.note/node/document/) { get; } | Gets the document of the node. |
| [FirstChild](../../aspose.note/compositenode-1/firstchild/) { get; } | Gets the first child node of this node. |
| [IsComposite](../../aspose.note/compositenode-1/iscomposite/) { get; } | Checks whether the node is composite. If true then the node can have child nodes. |
| [LastChild](../../aspose.note/compositenode-1/lastchild/) { get; } | Gets the last child node of this node. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Gets the next node at the same node tree level. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Gets the node type. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Gets the parent node. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Gets the previous node at the same node tree level. |

## Methods

| Name | Description |
| --- | --- |
| override [Accept](../../aspose.note/compositenode-1/accept/)(DocumentVisitor) | Accepts the visitor of the node. |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildfirst/)(T1) | Adds the node to the front of the list of child nodes for this node. |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildlast/)(T1) | Adds the node to the end of the list of child nodes for this node. |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode-1/getchildnodes/#getchildnodes_1)() | Get all child nodes by the node type. |
| [GetEnumerator](../../aspose.note/compositenode-1/getenumerator/)() | Returns an enumerator that iterates through child nodes of the `CompositeNode`. |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode-1/insertchild/)(int, T1) | Inserts the node to the specified position in the list of child nodes for this node. |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/#insertchildrenrange)(int, IEnumerable&lt;T&gt;) | Inserts the node's sequence starting from specified position in the list of child nodes for this node. |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/#insertchildrenrange_1)(int, params T[]) | Inserts the node's sequence starting from specified position in the list of child nodes for this node. |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode-1/removechild/)(T1) | Removes the child node. |

### See Also

* class [CompositeNodeBase](../compositenodebase/)
* interface [ICompositeNode&lt;T&gt;](../icompositenode-1/)
* interface [INode](../inode/)
* namespace [Aspose.Note](../../aspose.note/)
* assembly [Aspose.Note](../../)


