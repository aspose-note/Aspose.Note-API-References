---
title: Class Node
second_title: Aspose.Note for .NET API リファレンス
description: Aspose.Note.Node クラス. Aspose.Note ドキュメントのすべてのノードの基本クラス
type: docs
weight: 360
url: /ja/net/aspose.note/node/
---
## Node class

Aspose.Note ドキュメントのすべてのノードの基本クラス。

```csharp
public abstract class Node : INode
```

## プロパティ

| 名前 | 説明 |
| --- | --- |
| [Document](../../aspose.note/node/document/) { get; } | ノードのドキュメントを取得します。 |
| virtual [IsComposite](../../aspose.note/node/iscomposite/) { get; } | このノードが複合かどうかを示す値を取得します。 true の場合、ノードは子ノードを持つことができます。 |
| [NextSibling](../../aspose.note/node/nextsibling/) { get; } | 同じノード ツリー レベルの次のノードを取得します。 |
| [NodeType](../../aspose.note/node/nodetype/) { get; } | ノード タイプを取得します。 |
| [ParentNode](../../aspose.note/node/parentnode/) { get; } | 親ノードを取得します。 |
| [PreviousSibling](../../aspose.note/node/previoussibling/) { get; } | 同じノード ツリー レベルの前のノードを取得します。 |

## メソッド

| 名前 | 説明 |
| --- | --- |
| abstract [Accept](../../aspose.note/node/accept/)(DocumentVisitor) | ノードの訪問者を受け入れます。 |

### 関連項目

* interface [INode](../inode/)
* 名前空間 [Aspose.Note](../../aspose.note/)
* 組み立て [Aspose.Note](../../)


