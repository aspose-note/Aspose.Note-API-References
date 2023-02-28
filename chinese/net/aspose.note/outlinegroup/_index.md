---
title: Class OutlineGroup
second_title: Aspose.Note for .NET API 参考
description: Aspose.Note.OutlineGroup 班级. 代表一个OutlineGroup
type: docs
weight: 470
url: /zh/net/aspose.note/outlinegroup/
---
## OutlineGroup class

代表一个OutlineGroup。

```csharp
public sealed class OutlineGroup : IndentatedNode<IOutlineChildNode>, IOutlineChildNode, 
    IOutlineElementChildNode
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [OutlineGroup](outlinegroup/#constructor)() | 初始化一个新的实例`OutlineGroup`类. |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [Document](../../aspose.note/node/document/) { get; } | 获取节点的文档。 |
| [FirstChild](../../aspose.note/compositenode-1/firstchild/) { get; } |  |
| [IndentPosition](../../aspose.note/indentatednode-1/indentposition/) { get; set; } |  |
| [IsComposite](../../aspose.note/compositenode-1/iscomposite/) { get; } |  |
| [LastChild](../../aspose.note/compositenode-1/lastchild/) { get; } |  |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | 获取同一节点树级别的下一个节点。 |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | 获取节点类型。 |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | 获取父节点。 |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | 获取同一节点树级别的前一个节点。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| override [Accept](../../aspose.note/outlinegroup/accept/)(DocumentVisitor) | 接受节点的访问者。 |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildfirst/)(T1) |  |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildlast/)(T1) |  |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode-1/getchildnodes/)() |  |
| [GetEnumerator](../../aspose.note/compositenode-1/getenumerator/)() |  |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode-1/insertchild/)(int, T1) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, IEnumerable&lt;IOutlineChildNode&gt;) |  |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/)(int, params IOutlineChildNode[]) |  |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode-1/removechild/)(T1) |  |

### 也可以看看

* class [IndentatedNode&lt;T&gt;](../indentatednode-1/)
* interface [IOutlineChildNode](../ioutlinechildnode/)
* interface [IOutlineElementChildNode](../ioutlineelementchildnode/)
* 命名空间 [Aspose.Note](../../aspose.note/)
* 部件 [Aspose.Note](../../)


