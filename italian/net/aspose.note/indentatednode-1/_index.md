---
title: Class IndentatedNodeT
second_title: Aspose.Note per .NET API Reference
description: Aspose.Note.IndentatedNode1T classe. La classe base per i nodi con indentazione relativa per i nodi figli.
type: docs
weight: 300
url: /it/net/aspose.note/indentatednode-1/
---
## IndentatedNode&lt;T&gt; class

La classe base per i nodi con indentazione relativa per i nodi figli.

```csharp
public class IndentatedNode<T> : CompositeNode<T>, IIndentatedNode
    where T : INode
```

| Parametro | Descrizione |
| --- | --- |
| T | Il tipo di elementi nel nodo composito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Document](../../aspose.note/node/document/) { get; } | Ottiene il documento del nodo. |
| [FirstChild](../../aspose.note/compositenode-1/firstchild/) { get; } |  |
| [IndentPosition](../../aspose.note/indentatednode-1/indentposition/) { get; set; } | Ottiene o imposta la posizione del rientro. |
| [IsComposite](../../aspose.note/compositenode-1/iscomposite/) { get; } |  |
| [LastChild](../../aspose.note/compositenode-1/lastchild/) { get; } |  |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Ottiene il nodo successivo allo stesso livello di albero dei nodi. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Ottiene il tipo di nodo. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Ottiene il nodo padre. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Ottiene il nodo precedente allo stesso livello dell'albero dei nodi. |

## Metodi

| Nome | Descrizione |
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

### Guarda anche

* class [CompositeNode&lt;T&gt;](../compositenode-1/)
* interface [IIndentatedNode](../iindentatednode/)
* interface [INode](../inode/)
* spazio dei nomi [Aspose.Note](../../aspose.note/)
* assemblea [Aspose.Note](../../)


