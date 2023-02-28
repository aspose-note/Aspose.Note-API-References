---
title: Class CompositeNodeT
second_title: Aspose.Note för .NET API-referens
description: Aspose.Note.CompositeNode1T klass. Den generiska basklassen för noder som kan innehålla andra noder.
type: docs
weight: 40
url: /sv/net/aspose.note/compositenode-1/
---
## CompositeNode&lt;T&gt; class

Den generiska basklassen för noder som kan innehålla andra noder.

```csharp
public abstract class CompositeNode<T> : CompositeNodeBase, ICompositeNode<T>
    where T : INode
```

| Parameter | Beskrivning |
| --- | --- |
| T | Typen av element i den sammansatta noden. |

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [Document](../../aspose.note/node/document/) { get; } | Hämtar dokumentet för noden. |
| [FirstChild](../../aspose.note/compositenode-1/firstchild/) { get; } | Hämtar den första underordnade noden för denna nod. |
| [IsComposite](../../aspose.note/compositenode-1/iscomposite/) { get; } | Kontrollerar om noden är sammansatt. Om sant kan noden ha barnnoder. |
| [LastChild](../../aspose.note/compositenode-1/lastchild/) { get; } | Hämtar den sista underordnade noden för denna nod. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Hämtar nästa nod på samma nodträdsnivå. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Hämtar nodtypen. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Hämtar den överordnade noden. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Hämtar föregående nod på samma nodträdsnivå. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| override [Accept](../../aspose.note/compositenode-1/accept/)(DocumentVisitor) | Accepterar besökaren av noden. |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildfirst/)(T1) | Lägger till noden längst fram i listan över underordnade noder för denna nod. |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildlast/)(T1) | Lägger till noden i slutet av listan över underordnade noder för denna nod. |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode-1/getchildnodes/#getchildnodes_1)() | Hämta alla underordnade noder efter nodtyp. |
| [GetEnumerator](../../aspose.note/compositenode-1/getenumerator/)() | Returnerar en enumerator som itererar genom underordnade noder av`CompositeNode` . |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode-1/insertchild/)(int, T1) | Infogar noden till den angivna positionen i listan över underordnade noder för denna nod. |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/#insertchildrenrange)(int, IEnumerable&lt;T&gt;) | Infogar nodens sekvens med start från angiven position i listan över underordnade noder för denna nod. |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/#insertchildrenrange_1)(int, params T[]) | Infogar nodens sekvens med start från angiven position i listan över underordnade noder för denna nod. |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode-1/removechild/)(T1) | Tar bort den underordnade noden. |

### Se även

* class [CompositeNodeBase](../compositenodebase/)
* interface [ICompositeNode&lt;T&gt;](../icompositenode-1/)
* interface [INode](../inode/)
* namnutrymme [Aspose.Note](../../aspose.note/)
* hopsättning [Aspose.Note](../../)


