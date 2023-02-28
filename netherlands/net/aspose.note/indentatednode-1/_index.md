---
title: Class IndentatedNodeT
second_title: Aspose.Note voor .NET API-referentie
description: Aspose.Note.IndentatedNode1T klas. De basisklasse voor knooppunten met relatieve inspringing voor onderliggende knooppunten.
type: docs
weight: 300
url: /nl/net/aspose.note/indentatednode-1/
---
## IndentatedNode&lt;T&gt; class

De basisklasse voor knooppunten met relatieve inspringing voor onderliggende knooppunten.

```csharp
public class IndentatedNode<T> : CompositeNode<T>, IIndentatedNode
    where T : INode
```

| Parameter | Beschrijving |
| --- | --- |
| T | Het type elementen in het samengestelde knooppunt. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Document](../../aspose.note/node/document/) { get; } | Haalt het document van het knooppunt op. |
| [FirstChild](../../aspose.note/compositenode-1/firstchild/) { get; } |  |
| [IndentPosition](../../aspose.note/indentatednode-1/indentposition/) { get; set; } | Haalt of stelt de inspringpositie in. |
| [IsComposite](../../aspose.note/compositenode-1/iscomposite/) { get; } |  |
| [LastChild](../../aspose.note/compositenode-1/lastchild/) { get; } |  |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Haalt het volgende knooppunt op op hetzelfde knooppuntboomniveau. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Haalt het knooppunttype op. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Haalt het bovenliggende knooppunt op. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Haalt het vorige knooppunt op hetzelfde knooppuntboomniveau. |

## methoden

| Naam | Beschrijving |
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

### Zie ook

* class [CompositeNode&lt;T&gt;](../compositenode-1/)
* interface [IIndentatedNode](../iindentatednode/)
* interface [INode](../inode/)
* naamruimte [Aspose.Note](../../aspose.note/)
* montage [Aspose.Note](../../)


