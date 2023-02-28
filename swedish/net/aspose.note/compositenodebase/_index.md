---
title: Class CompositeNodeBase
second_title: Aspose.Note för .NET API-referens
description: Aspose.Note.CompositeNodeBase klass. Den ickegeneriska klassen för noder som kan innehålla andra noder.
type: docs
weight: 30
url: /sv/net/aspose.note/compositenodebase/
---
## CompositeNodeBase class

Den icke-generiska klassen för noder som kan innehålla andra noder.

```csharp
public abstract class CompositeNodeBase : Node, ICompositeNode
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [Document](../../aspose.note/node/document/) { get; } | Hämtar dokumentet för noden. |
| virtual [IsComposite](../../aspose.note/node/iscomposite/) { get; } | Får ett värde som indikerar om denna nod är sammansatt. Om sant kan noden ha underordnade noder. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Hämtar nästa nod på samma nodträdsnivå. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Hämtar nodtypen. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Hämtar den överordnade noden. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Hämtar föregående nod på samma nodträdsnivå. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| abstract [Accept](../../aspose.note/node/accept/)(DocumentVisitor) | Accepterar besökaren av noden. |
| abstract [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenodebase/getchildnodes/#getchildnodes_1)() | Hämta alla underordnade noder efter nodtyp. |

### Se även

* class [Node](../node/)
* interface [ICompositeNode](../icompositenode/)
* namnutrymme [Aspose.Note](../../aspose.note/)
* hopsättning [Aspose.Note](../../)


