---
title: Class IndentatedNodeT
second_title: Aspose.Note for .NET API Referansı
description: Aspose.Note.IndentatedNode1T sınıf. Alt düğümler için göreli girintili düğümler için temel sınıf.
type: docs
weight: 300
url: /tr/net/aspose.note/indentatednode-1/
---
## IndentatedNode&lt;T&gt; class

Alt düğümler için göreli girintili düğümler için temel sınıf.

```csharp
public class IndentatedNode<T> : CompositeNode<T>, IIndentatedNode
    where T : INode
```

| Parametre | Tanım |
| --- | --- |
| T | Bileşik düğümdeki öğelerin türü. |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [Document](../../aspose.note/node/document/) { get; } | Düğümün belgesini alır. |
| [FirstChild](../../aspose.note/compositenode-1/firstchild/) { get; } |  |
| [IndentPosition](../../aspose.note/indentatednode-1/indentposition/) { get; set; } | Girinti konumunu alır veya ayarlar. |
| [IsComposite](../../aspose.note/compositenode-1/iscomposite/) { get; } |  |
| [LastChild](../../aspose.note/compositenode-1/lastchild/) { get; } |  |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Aynı düğüm ağacı seviyesindeki bir sonraki düğümü alır. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Düğüm türünü alır. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Üst düğümü alır. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Aynı düğüm ağacı seviyesindeki önceki düğümü alır. |

## yöntemler

| İsim | Tanım |
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

### Ayrıca bakınız

* class [CompositeNode&lt;T&gt;](../compositenode-1/)
* interface [IIndentatedNode](../iindentatednode/)
* interface [INode](../inode/)
* ad alanı [Aspose.Note](../../aspose.note/)
* toplantı [Aspose.Note](../../)


