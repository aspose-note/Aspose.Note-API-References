---
title: "类 CompositeNodeBase"
second_title: "Aspose.Note for .NET API 参考"
description: "Aspose.Note.CompositeNodeBase 类。用于可以包含其他节点的非泛型节点类"
type: docs
weight: 30
url: /zh/net/aspose.note/compositenodebase/
---
## CompositeNodeBase class

可以包含其他节点的节点的非泛型类。

```csharp
public abstract class CompositeNodeBase : Node, ICompositeNode
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [Document](../../aspose.note/node/document/) { get; } | 获取节点的文档。 |
| virtual [IsComposite](../../aspose.note/node/iscomposite/) { get; } | 获取一个值，指示此节点是否为复合节点。如果为 true，则该节点可以拥有子节点。 |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | 获取同一节点树层级的下一个节点。 |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | 获取节点类型。 |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | 获取父节点。 |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | 获取同一节点树层级的上一个节点。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| abstract [Accept](../../aspose.note/node/accept/)(DocumentVisitor) | 接受节点的访问者。 |
| abstract [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenodebase/getchildnodes/#getchildnodes_1)() | 按节点类型获取所有子节点。 |

### 另请参阅

* class [Node](../node/)
* interface [ICompositeNode](../icompositenode/)
* namespace [Aspose.Note](../../aspose.note/)
* assembly [Aspose.Note](../../)


