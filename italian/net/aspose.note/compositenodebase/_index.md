---
title: Class CompositeNodeBase
second_title: Aspose.Note per .NET API Reference
description: Aspose.Note.CompositeNodeBase classe. La classe non generica per i nodi che possono contenere altri nodi.
type: docs
weight: 30
url: /it/net/aspose.note/compositenodebase/
---
## CompositeNodeBase class

La classe non generica per i nodi che possono contenere altri nodi.

```csharp
public abstract class CompositeNodeBase : Node, ICompositeNode
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Document](../../aspose.note/node/document/) { get; } | Ottiene il documento del nodo. |
| virtual [IsComposite](../../aspose.note/node/iscomposite/) { get; } | Ottiene un valore che indica se questo nodo è composto. Se vero il nodo può avere nodi figli. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Ottiene il nodo successivo allo stesso livello di albero dei nodi. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Ottiene il tipo di nodo. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Ottiene il nodo padre. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Ottiene il nodo precedente allo stesso livello dell'albero dei nodi. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| abstract [Accept](../../aspose.note/node/accept/)(DocumentVisitor) | Accetta il visitatore del nodo. |
| abstract [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenodebase/getchildnodes/#getchildnodes_1)() | Ottieni tutti i nodi figli in base al tipo di nodo. |

### Guarda anche

* class [Node](../node/)
* interface [ICompositeNode](../icompositenode/)
* spazio dei nomi [Aspose.Note](../../aspose.note/)
* assemblea [Aspose.Note](../../)


