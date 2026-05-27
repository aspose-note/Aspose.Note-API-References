---
title: "类 Node"
second_title: "Aspose.Note for .NET API 参考"
description: "Aspose.Note.Node 类。Aspose.Note 文档中所有节点的基类"
type: docs
weight: 430
url: /zh/net/aspose.note/node/
---
## Node class

Aspose.Note 文档中所有节点的基类。

```csharp
public abstract class Node : INode
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

* interface [INode](../inode/)
* namespace [Aspose.Note](../../aspose.note/)
* assembly [Aspose.Note](../../)


