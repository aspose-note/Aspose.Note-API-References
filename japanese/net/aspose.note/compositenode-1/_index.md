---
title: Class CompositeNodeT
second_title: Aspose.Note for .NET API リファレンス
description: Aspose.Note.CompositeNode1T クラス. 他のノードを含むことができるノードの基本ジェネリック クラス
type: docs
weight: 40
url: /ja/net/aspose.note/compositenode-1/
---
## CompositeNode&lt;T&gt; class

他のノードを含むことができるノードの基本ジェネリック クラス。

```csharp
public abstract class CompositeNode<T> : CompositeNodeBase, ICompositeNode<T>
    where T : INode
```

| パラメータ | 説明 |
| --- | --- |
| T | 複合ノード内の要素のタイプ. |

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [Document](../../aspose.note/node/document/) { get; } | ノードのドキュメントを取得します。 |
| [FirstChild](../../aspose.note/compositenode-1/firstchild/) { get; } | このノードの最初の子ノードを取得します。 |
| [IsComposite](../../aspose.note/compositenode-1/iscomposite/) { get; } | ノードが複合かどうかをチェックします。 true の場合、ノードは子ノードを持つことができます。 |
| [LastChild](../../aspose.note/compositenode-1/lastchild/) { get; } | このノードの最後の子ノードを取得します。 |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | 同じノード ツリー レベルの次のノードを取得します。 |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | ノード タイプを取得します。 |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | 親ノードを取得します。 |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | 同じノード ツリー レベルの前のノードを取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| override [Accept](../../aspose.note/compositenode-1/accept/)(DocumentVisitor) | ノードの訪問者を受け入れます。 |
| virtual [AppendChildFirst&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildfirst/)(T1) | このノードの子ノードのリストの先頭にノードを追加します。 |
| virtual [AppendChildLast&lt;T1&gt;](../../aspose.note/compositenode-1/appendchildlast/)(T1) | このノードの子ノードのリストの最後にノードを追加します。 |
| override [GetChildNodes&lt;T1&gt;](../../aspose.note/compositenode-1/getchildnodes/#getchildnodes_1)() | ノード タイプ別にすべての子ノードを取得します。 |
| [GetEnumerator](../../aspose.note/compositenode-1/getenumerator/)() | の子ノードを反復処理する列挙子を返します`CompositeNode`. |
| virtual [InsertChild&lt;T1&gt;](../../aspose.note/compositenode-1/insertchild/)(int, T1) | このノードの子ノードのリスト内の指定された位置にノードを挿入します。 |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/#insertchildrenrange)(int, IEnumerable&lt;T&gt;) | このノードの子ノードのリスト内の指定された位置から始まるノードのシーケンスを挿入します。 |
| [InsertChildrenRange](../../aspose.note/compositenode-1/insertchildrenrange/#insertchildrenrange_1)(int, params T[]) | このノードの子ノードのリスト内の指定された位置から始まるノードのシーケンスを挿入します。 |
| [RemoveChild&lt;T1&gt;](../../aspose.note/compositenode-1/removechild/)(T1) | 子ノードを削除します。 |

### 関連項目

* class [CompositeNodeBase](../compositenodebase/)
* interface [ICompositeNode&lt;T&gt;](../icompositenode-1/)
* interface [INode](../inode/)
* 名前空間 [Aspose.Note](../../aspose.note/)
* 組み立て [Aspose.Note](../../)


