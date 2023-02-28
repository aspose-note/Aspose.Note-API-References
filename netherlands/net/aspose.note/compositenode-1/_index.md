---
title: Class CompositeNodeT
second_title: Aspose.Note voor .NET API-referentie
description: Aspose.Note.CompositeNode1T klas. De algemene basisklasse voor knooppunten die andere knooppunten kunnen bevatten.
type: docs
weight: 40
url: /nl/net/aspose.note/compositenode-1/
---
## CompositeNode&lt;T&gt; class

De algemene basisklasse voor knooppunten die andere knooppunten kunnen bevatten.

```csharp
public abstract class CompositeNode<T> : CompositeNodeBase, ICompositeNode<T>
    where T : INode
```

| Parameter | Beschrijving |
| --- | --- |
| T | Het type elementen in het samengestelde knooppunt. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Document](../../aspose.note/node/document/) { get; } | Haalt het document van het knooppunt op. |
| [FirstChild](../../aspose.note/compositenode-1/firstchild/) { get; } | Haalt het eerste onderliggende knooppunt van dit knooppunt op. |
| [IsComposite](../../aspose.note/compositenode-1/iscomposite/) { get; } | Controleert of de knoop samengesteld is. Indien waar, kan het knooppunt onderliggende knooppunten hebben. |
| [LastChild](../../aspose.note/compositenode-1/lastchild/) { get; } | Haalt het laatste onderliggende knooppunt van dit knooppunt op. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Haalt het volgende knooppunt op op hetzelfde knooppuntboomniveau. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Haalt het knooppunttype op. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Haalt het bovenliggende knooppunt op. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Haalt het vorige knooppunt op hetzelfde knooppuntboomniveau. |

## methoden

| Naam | Beschrijving |
| --- | --- |
| override [Accept](../../aspose.note/compositenode-1/accept/)(DocumentVisitor) | Accepteert de bezoeker van de node. |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildfirst/)(T1) | Voegt het knooppunt toe aan de voorkant van de lijst met onderliggende knooppunten voor dit knooppunt. |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildlast/)(T1) | Voegt het knooppunt toe aan het einde van de lijst met onderliggende knooppunten voor dit knooppunt. |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode-1/getchildnodes/#getchildnodes_1)() | Alle onderliggende knooppunten ophalen op basis van het knooppunttype. |
| [GetEnumerator](../../aspose.note/compositenode-1/getenumerator/)() | Retourneert een teller die itereert door onderliggende knooppunten van het`CompositeNode` . |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode-1/insertchild/)(int, T1) | Voegt het knooppunt in op de opgegeven positie in de lijst met onderliggende knooppunten voor dit knooppunt. |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/#insertchildrenrange)(int, IEnumerable&lt;T&gt;) | Voegt de reeks van het knooppunt in vanaf de gespecificeerde positie in de lijst met onderliggende knooppunten voor dit knooppunt. |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/#insertchildrenrange_1)(int, params T[]) | Voegt de reeks van het knooppunt in vanaf de gespecificeerde positie in de lijst met onderliggende knooppunten voor dit knooppunt. |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode-1/removechild/)(T1) | Verwijdert het onderliggende knooppunt. |

### Zie ook

* class [CompositeNodeBase](../compositenodebase/)
* interface [ICompositeNode&lt;T&gt;](../icompositenode-1/)
* interface [INode](../inode/)
* naamruimte [Aspose.Note](../../aspose.note/)
* montage [Aspose.Note](../../)


