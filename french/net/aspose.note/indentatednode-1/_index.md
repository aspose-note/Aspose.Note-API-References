---
title: Class IndentatedNodeT
second_title: Référence de l'API Aspose.Note pour .NET
description: Aspose.Note.IndentatedNode1T classe. La classe de base pour les nœuds avec une indentation relative pour les nœuds enfants.
type: docs
weight: 300
url: /fr/net/aspose.note/indentatednode-1/
---
## IndentatedNode&lt;T&gt; class

La classe de base pour les nœuds avec une indentation relative pour les nœuds enfants.

```csharp
public class IndentatedNode<T> : CompositeNode<T>, IIndentatedNode
    where T : INode
```

| Paramètre | La description |
| --- | --- |
| T | Le type d'éléments dans le nœud composite. |

## Propriétés

| Nom | La description |
| --- | --- |
| [Document](../../aspose.note/node/document/) { get; } | Obtient le document du nœud. |
| [FirstChild](../../aspose.note/compositenode-1/firstchild/) { get; } |  |
| [IndentPosition](../../aspose.note/indentatednode-1/indentposition/) { get; set; } | Obtient ou définit la position du retrait. |
| [IsComposite](../../aspose.note/compositenode-1/iscomposite/) { get; } |  |
| [LastChild](../../aspose.note/compositenode-1/lastchild/) { get; } |  |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Obtient le nœud suivant au même niveau d'arborescence de nœuds. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Obtient le type de nœud. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Obtient le nœud parent. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Obtient le nœud précédent au même niveau d'arborescence de nœuds. |

## Méthodes

| Nom | La description |
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

### Voir également

* class [CompositeNode&lt;T&gt;](../compositenode-1/)
* interface [IIndentatedNode](../iindentatednode/)
* interface [INode](../inode/)
* espace de noms [Aspose.Note](../../aspose.note/)
* Assemblée [Aspose.Note](../../)


