---
title: Class CompositeNodeBase
second_title: Aspose.Note voor .NET API-referentie
description: Aspose.Note.CompositeNodeBase klas. De nietgenerieke klasse voor knooppunten die andere knooppunten kunnen bevatten.
type: docs
weight: 30
url: /nl/net/aspose.note/compositenodebase/
---
## CompositeNodeBase class

De niet-generieke klasse voor knooppunten die andere knooppunten kunnen bevatten.

```csharp
public abstract class CompositeNodeBase : Node, ICompositeNode
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Document](../../aspose.note/node/document/) { get; } | Haalt het document van het knooppunt op. |
| virtual [IsComposite](../../aspose.note/node/iscomposite/) { get; } | Krijgt een waarde die aangeeft of dit knooppunt samengesteld is. Indien waar, kan het knooppunt onderliggende knooppunten hebben. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Haalt het volgende knooppunt op op hetzelfde knooppuntboomniveau. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Haalt het knooppunttype op. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Haalt het bovenliggende knooppunt op. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Haalt het vorige knooppunt op hetzelfde knooppuntboomniveau. |

## methoden

| Naam | Beschrijving |
| --- | --- |
| abstract [Accept](../../aspose.note/node/accept/)(DocumentVisitor) | Accepteert de bezoeker van de node. |
| abstract [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenodebase/getchildnodes/#getchildnodes_1)() | Alle onderliggende knooppunten ophalen op basis van het knooppunttype. |

### Zie ook

* class [Node](../node/)
* interface [ICompositeNode](../icompositenode/)
* naamruimte [Aspose.Note](../../aspose.note/)
* montage [Aspose.Note](../../)


