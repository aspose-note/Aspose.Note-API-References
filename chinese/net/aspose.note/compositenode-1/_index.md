---
title: Class CompositeNodeT
second_title: Aspose.Note for .NET API 参考
description: Aspose.Note.CompositeNode1T 班级. 可以包含其他节点的节点的基本泛型类
type: docs
weight: 40
url: /zh/net/aspose.note/compositenode-1/
---
## CompositeNode&lt;T&gt; class

可以包含其他节点的节点的基本泛型类。

```csharp
public abstract class CompositeNode<T> : CompositeNodeBase, ICompositeNode<T>
    where T : INode
```

| 范围 | 描述 |
| --- | --- |
| T | 复合节点中元素的类型。 |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [Document](../../aspose.note/node/document/) { get; } | 获取节点的文档。 |
| [FirstChild](../../aspose.note/compositenode-1/firstchild/) { get; } | 获取该节点的第一个子节点。 |
| [IsComposite](../../aspose.note/compositenode-1/iscomposite/) { get; } | 检查节点是否为复合节点。如果为真，则该节点可以有子节点。 |
| [LastChild](../../aspose.note/compositenode-1/lastchild/) { get; } | 获取该节点的最后一个子节点。 |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | 获取同一节点树级别的下一个节点。 |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | 获取节点类型。 |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | 获取父节点。 |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | 获取同一节点树级别的前一个节点。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| override [Accept](../../aspose.note/compositenode-1/accept/)(DocumentVisitor) | 接受节点的访问者。 |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildfirst/)(T1) | 将节点添加到此节点的子节点列表的前面。 |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildlast/)(T1) | 将节点添加到此节点的子节点列表的末尾。 |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode-1/getchildnodes/#getchildnodes_1)() | 根据节点类型获取所有子节点。 |
| [GetEnumerator](../../aspose.note/compositenode-1/getenumerator/)() | 返回一个遍历子节点的枚举器`CompositeNode`. |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode-1/insertchild/)(int, T1) | 将节点插入到该节点的子节点列表中的指定位置。 |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/#insertchildrenrange)(int, IEnumerable&lt;T&gt;) | 从该节点的子节点列表中的指定位置开始插入节点的序列。 |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/#insertchildrenrange_1)(int, params T[]) | 从该节点的子节点列表中的指定位置开始插入节点的序列。 |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode-1/removechild/)(T1) | 删除子节点。 |

### 也可以看看

* class [CompositeNodeBase](../compositenodebase/)
* interface [ICompositeNode&lt;T&gt;](../icompositenode-1/)
* interface [INode](../inode/)
* 命名空间 [Aspose.Note](../../aspose.note/)
* 部件 [Aspose.Note](../../)


