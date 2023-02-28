---
title: Class OutlineGroup
second_title: Aspose.Note for .NET API Referansı
description: Aspose.Note.OutlineGroup sınıf. Bir OutlineGroupu Temsil Eder.
type: docs
weight: 470
url: /tr/net/aspose.note/outlinegroup/
---
## OutlineGroup class

Bir OutlineGroup'u Temsil Eder.

```csharp
public sealed class OutlineGroup : IndentatedNode<IOutlineChildNode>, IOutlineChildNode, 
    IOutlineElementChildNode
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [OutlineGroup](outlinegroup/#constructor)() | Yeni bir örneğini başlatır.`OutlineGroup` sınıf. |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [Document](../../aspose.note/node/document/) { get; } | Düğümün belgesini alır. |
| [FirstChild](../../aspose.note/compositenode-1/firstchild/) { get; } |  |
| [IndentPosition](../../aspose.note/indentatednode-1/indentposition/) { get; set; } |  |
| [IsComposite](../../aspose.note/compositenode-1/iscomposite/) { get; } |  |
| [LastChild](../../aspose.note/compositenode-1/lastchild/) { get; } |  |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Aynı düğüm ağacı seviyesindeki bir sonraki düğümü alır. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Düğüm türünü alır. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Üst düğümü alır. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Aynı düğüm ağacı seviyesindeki önceki düğümü alır. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| override [Accept](../../aspose.note/outlinegroup/accept/)(DocumentVisitor) | Düğümün ziyaretçisini kabul eder. |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildfirst/)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildlast/)(T1) |  |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode-1/getchildnodes/)() |  |
| [GetEnumerator](../../aspose.note/compositenode-1/getenumerator/)() |  |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode-1/insertchild/)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, IEnumerable&lt;IOutlineChildNode&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, params IOutlineChildNode[]) |  |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode-1/removechild/)(T1) |  |

### Ayrıca bakınız

* class [IndentatedNode&lt;T&gt;](../indentatednode-1/)
* interface [IOutlineChildNode](../ioutlinechildnode/)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode/)
* ad alanı [Aspose.Note](../../aspose.note/)
* toplantı [Aspose.Note](../../)


