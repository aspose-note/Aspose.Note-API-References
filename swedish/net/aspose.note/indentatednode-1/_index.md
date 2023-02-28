---
title: Class IndentatedNodeT
second_title: Aspose.Note för .NET API-referens
description: Aspose.Note.IndentatedNode1T klass. Basklassen för noder med relativ indrag för undernoder.
type: docs
weight: 300
url: /sv/net/aspose.note/indentatednode-1/
---
## IndentatedNode&lt;T&gt; class

Basklassen för noder med relativ indrag för undernoder.

```csharp
public class IndentatedNode<T> : CompositeNode<T>, IIndentatedNode
    where T : INode
```

| Parameter | Beskrivning |
| --- | --- |
| T | Typen av element i den sammansatta noden. |

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [Document](../../aspose.note/node/document/) { get; } | Hämtar dokumentet för noden. |
| [FirstChild](../../aspose.note/compositenode-1/firstchild/) { get; } |  |
| [IndentPosition](../../aspose.note/indentatednode-1/indentposition/) { get; set; } | Hämtar eller ställer in indragspositionen. |
| [IsComposite](../../aspose.note/compositenode-1/iscomposite/) { get; } |  |
| [LastChild](../../aspose.note/compositenode-1/lastchild/) { get; } |  |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Hämtar nästa nod på samma nodträdsnivå. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Hämtar nodtypen. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Hämtar den överordnade noden. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Hämtar föregående nod på samma nodträdsnivå. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| override [Accept](../../aspose.note/compositenode-1/accept/)(DocumentVisitor) |  |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildfirst/)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildlast/)(T1) |  |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode-1/getchildnodes/)() |  |
| [GetEnumerator](../../aspose.note/compositenode-1/getenumerator/)() |  |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode-1/insertchild/)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, IEnumerable&lt;T&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, params T[]) |  |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode-1/removechild/)(T1) |  |

### Se även

* class [CompositeNode&lt;T&gt;](../compositenode-1/)
* interface [IIndentatedNode](../iindentatednode/)
* interface [INode](../inode/)
* namnutrymme [Aspose.Note](../../aspose.note/)
* hopsättning [Aspose.Note](../../)


