---
title: Class Node
second_title: Aspose.Note for .NET API 参考
description: Aspose.Note.Node 班级. Aspose.Note 文档的所有节点的基类
type: docs
weight: 360
url: /zh/net/aspose.note/node/
---
## Node class

Aspose.Note 文档的所有节点的基类。

```csharp
public abstract class Node : INode
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [Document](../../aspose.note/node/document/) { get; } | 获取节点的文档。 |
| virtual [IsComposite](../../aspose.note/node/iscomposite/) { get; } | 获取一个值，指示此节点是否为复合节点。如果为真，节点可以有子节点。 |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | 获取同一节点树级别的下一个节点。 |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | 获取节点类型。 |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | 获取父节点。 |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | 获取同一节点树级别的前一个节点。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| abstract [Accept](../../aspose.note/node/accept/)(DocumentVisitor) | 接受节点的访问者。 |

### 也可以看看

* interface [INode](../inode/)
* 命名空间 [Aspose.Note](../../aspose.note/)
* 部件 [Aspose.Note](../../)


