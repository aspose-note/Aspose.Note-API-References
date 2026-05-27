---
title: "类 CompositeNodeT"
second_title: "Aspose.Note for .NET API 参考"
description: "Aspose.Note.CompositeNode1T 类。可包含其他节点的节点的基础通用类"
type: docs
weight: 40
url: /zh/net/aspose.note/compositenode-1/
---
## CompositeNode&lt;T&gt; class

可以包含其他节点的节点的基泛型类。

```csharp
public abstract class CompositeNode<T> : CompositeNodeBase, ICompositeNode<T>
    where T : INode
```

| 参数 | 描述 |
| --- | --- |
| T | 复合节点中元素的类型。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [Document](../../aspose.note/node/document/) { get; } | 获取节点的文档。 |
| [FirstChild](../../aspose.note/compositenode-1/firstchild/) { get; } | 获取此节点的第一个子节点。 |
| [IsComposite](../../aspose.note/compositenode-1/iscomposite/) { get; } | 检查节点是否为复合节点。如果为 true，则该节点可以拥有子节点。 |
| [LastChild](../../aspose.note/compositenode-1/lastchild/) { get; } | 获取此节点的最后一个子节点。 |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | 获取同一节点树层级的下一个节点。 |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | 获取节点类型。 |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | 获取父节点。 |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | 获取同一节点树层级的上一个节点。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| override [Accept](../../aspose.note/compositenode-1/accept/)(DocumentVisitor) | 接受节点的访问者。 |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildfirst/)(T1) | 将节点添加到此节点的子节点列表的前端。 |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildlast/)(T1) | 将节点添加到此节点的子节点列表的末尾。 |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode-1/getchildnodes/#getchildnodes_1)() | 按节点类型获取所有子节点。 |
| [GetEnumerator](../../aspose.note/compositenode-1/getenumerator/)() | 返回一个枚举器，用于遍历 `CompositeNode` 的子节点。 |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode-1/insertchild/)(int, T1) | 将节点插入到此节点的子节点列表中的指定位置。 |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/#insertchildrenrange)(int, IEnumerable&lt;T&gt;) | 从指定位置开始，将节点的序列插入到此节点的子节点列表中。 |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/#insertchildrenrange_1)(int, params T[]) | 从指定位置开始，将节点的序列插入到此节点的子节点列表中。 |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode-1/removechild/)(T1) | 移除子节点。 |

### 另请参阅

* class [CompositeNodeBase](../compositenodebase/)
* interface [ICompositeNode&lt;T&gt;](../icompositenode-1/)
* interface [INode](../inode/)
* namespace [Aspose.Note](../../aspose.note/)
* assembly [Aspose.Note](../../)


