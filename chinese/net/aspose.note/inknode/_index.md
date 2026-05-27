---
title: "类 InkNode"
second_title: "Aspose.Note for .NET API 参考"
description: "Aspose.Note.InkNode 类。表示所有墨迹节点的通用接口"
type: docs
weight: 340
url: /zh/net/aspose.note/inknode/
---
## InkNode class

表示所有 ink 节点的通用接口。

```csharp
public abstract class InkNode : Node
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

### 另请参阅

* class [Node](../node/)
* namespace [Aspose.Note](../../aspose.note/)
* assembly [Aspose.Note](../../)


