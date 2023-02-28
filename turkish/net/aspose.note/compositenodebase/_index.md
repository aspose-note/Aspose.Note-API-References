---
title: Class CompositeNodeBase
second_title: Aspose.Note for .NET API Referansı
description: Aspose.Note.CompositeNodeBase sınıf. Diğer düğümleri içerebilen düğümler için genel olmayan sınıf.
type: docs
weight: 30
url: /tr/net/aspose.note/compositenodebase/
---
## CompositeNodeBase class

Diğer düğümleri içerebilen düğümler için genel olmayan sınıf.

```csharp
public abstract class CompositeNodeBase : Node, ICompositeNode
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [Document](../../aspose.note/node/document/) { get; } | Düğümün belgesini alır. |
| virtual [IsComposite](../../aspose.note/node/iscomposite/) { get; } | Bu düğümün bileşik olup olmadığını gösteren bir değer alır. Doğruysa, düğümün alt düğümleri olabilir. |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | Aynı düğüm ağacı seviyesindeki bir sonraki düğümü alır. |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | Düğüm türünü alır. |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | Üst düğümü alır. |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | Aynı düğüm ağacı seviyesindeki önceki düğümü alır. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| abstract [Accept](../../aspose.note/node/accept/)(DocumentVisitor) | Düğümün ziyaretçisini kabul eder. |
| abstract [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenodebase/getchildnodes/#getchildnodes_1)() | Tüm alt düğümleri, düğüm türüne göre alın. |

### Ayrıca bakınız

* class [Node](../node/)
* interface [ICompositeNode](../icompositenode/)
* ad alanı [Aspose.Note](../../aspose.note/)
* toplantı [Aspose.Note](../../)


