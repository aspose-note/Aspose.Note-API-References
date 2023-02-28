---
title: Class CompositeNodeBase
second_title: Référence de l'API Aspose.Note pour .NET
description: Aspose.Note.CompositeNodeBase classe. La classe non générique pour les nœuds pouvant contenir dautres nœuds.
type: docs
weight: 30
url: /fr/net/aspose.note/compositenodebase/
---
## CompositeNodeBase class

La classe non générique pour les nœuds pouvant contenir d'autres nœuds.

```csharp
public abstract class CompositeNodeBase : Node, ICompositeNode
```

## Propriétés

| Nom | La description |
| --- | --- |
| [Document](../../aspose.note/node/document/) { get; } | Obtient le document du nœud. |
| virtual [IsComposite](../../aspose.note/node/iscomposite/) { get; } | Obtient une valeur indiquant si ce nœud est composite. Si vrai, le nœud peut avoir des nœuds enfants. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Obtient le nœud suivant au même niveau d'arborescence de nœuds. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Obtient le type de nœud. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Obtient le nœud parent. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Obtient le nœud précédent au même niveau d'arborescence de nœuds. |

## Méthodes

| Nom | La description |
| --- | --- |
| abstract [Accept](../../aspose.note/node/accept/)(DocumentVisitor) | Accepte le visiteur du nœud. |
| abstract [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenodebase/getchildnodes/#getchildnodes_1)() | Obtenir tous les nœuds enfants par le type de nœud. |

### Voir également

* class [Node](../node/)
* interface [ICompositeNode](../icompositenode/)
* espace de noms [Aspose.Note](../../aspose.note/)
* Assemblée [Aspose.Note](../../)


