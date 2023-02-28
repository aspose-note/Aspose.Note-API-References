---
title: Class CompositeNodeT
second_title: Aspose.Note für .NET-API-Referenz
description: Aspose.Note.CompositeNode1T klas. Die generische Basisklasse für Knoten die andere Knoten enthalten können.
type: docs
weight: 40
url: /de/net/aspose.note/compositenode-1/
---
## CompositeNode&lt;T&gt; class

Die generische Basisklasse für Knoten, die andere Knoten enthalten können.

```csharp
public abstract class CompositeNode<T> : CompositeNodeBase, ICompositeNode<T>
    where T : INode
```

| Parameter | Beschreibung |
| --- | --- |
| T | Der Elementtyp im zusammengesetzten Knoten. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Document](../../aspose.note/node/document/) { get; } | Ruft das Dokument des Knotens ab. |
| [FirstChild](../../aspose.note/compositenode-1/firstchild/) { get; } | Ruft den ersten untergeordneten Knoten dieses Knotens ab. |
| [IsComposite](../../aspose.note/compositenode-1/iscomposite/) { get; } | Prüft, ob der Knoten zusammengesetzt ist. Wenn wahr, kann der Knoten untergeordnete Knoten haben. |
| [LastChild](../../aspose.note/compositenode-1/lastchild/) { get; } | Ruft den letzten untergeordneten Knoten dieses Knotens ab. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Ruft den nächsten Knoten auf derselben Knotenbaumebene ab. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Ruft den Knotentyp ab. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Ruft den übergeordneten Knoten ab. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Ruft den vorherigen Knoten auf derselben Knotenbaumebene ab. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| override [Accept](../../aspose.note/compositenode-1/accept/)(DocumentVisitor) | Akzeptiert den Besucher des Knotens. |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildfirst/)(T1) | Fügt den Knoten am Anfang der Liste der untergeordneten Knoten für diesen Knoten hinzu. |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildlast/)(T1) | Fügt den Knoten am Ende der Liste der untergeordneten Knoten für diesen Knoten hinzu. |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode-1/getchildnodes/#getchildnodes_1)() | Alle untergeordneten Knoten nach Knotentyp abrufen. |
| [GetEnumerator](../../aspose.note/compositenode-1/getenumerator/)() | Gibt einen Enumerator zurück, der die untergeordneten Knoten von iteriert`CompositeNode` . |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode-1/insertchild/)(int, T1) | Fügt den Knoten an der angegebenen Position in die Liste der untergeordneten Knoten für diesen Knoten ein. |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/#insertchildrenrange)(int, IEnumerable&lt;T&gt;) | Fügt die Sequenz des Knotens ab der angegebenen Position in die Liste der untergeordneten Knoten für diesen Knoten ein. |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/#insertchildrenrange_1)(int, params T[]) | Fügt die Sequenz des Knotens ab der angegebenen Position in die Liste der untergeordneten Knoten für diesen Knoten ein. |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode-1/removechild/)(T1) | Entfernt den untergeordneten Knoten. |

### Siehe auch

* class [CompositeNodeBase](../compositenodebase/)
* interface [ICompositeNode&lt;T&gt;](../icompositenode-1/)
* interface [INode](../inode/)
* namensraum [Aspose.Note](../../aspose.note/)
* Montage [Aspose.Note](../../)


