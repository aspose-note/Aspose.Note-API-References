---
title: "TableCell"
second_title: "Aspose.Note for Java API リファレンス"
description: "テーブルセルを表します。"
type: docs
weight: 88
url: /ja/java/com.aspose.note/tablecell/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode, com.aspose.note.IndentatedNode
```
public final class TableCell extends IndentatedNode<IOutlineChildNode,TableCell>
```

テーブルセルを表します。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [TableCell()](#TableCell--) | `TableCell` クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | ノードのビジターを受け入れます。 |
| [getBackgroundColor()](#getBackgroundColor--) | 背景色を取得します。 |
| [getInternalIndentPosition()](#getInternalIndentPosition--) |  |
| [getLastModifiedTime()](#getLastModifiedTime--) | 最終更新時刻を取得または設定します。 |
| [getMaxWidth()](#getMaxWidth--) | 最大幅を取得します。 |
| [setBackgroundColor(Color value)](#setBackgroundColor-java.awt.Color-) | 背景色を設定します。 |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | 最終更新時刻を取得または設定します。 |
### TableCell() {#TableCell--}
```
public TableCell()
```


`TableCell` クラスの新しいインスタンスを初期化します。

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


ノードのビジターを受け入れます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | `DocumentVisitor` から派生したクラスのオブジェクト。 |

### getBackgroundColor() {#getBackgroundColor--}
```
public Color getBackgroundColor()
```


背景色を取得します。

**Returns:**
java.awt.Color
### getInternalIndentPosition() {#getInternalIndentPosition--}
```
public int getInternalIndentPosition()
```


インデントサイズを取得するために RgOutlineIndentDistance 配列で合計する項目数を取得します。

**Returns:**
int
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


最終更新時刻を取得または設定します。

**Returns:**
java.util.Date
### getMaxWidth() {#getMaxWidth--}
```
public float getMaxWidth()
```


最大幅を取得します。

**Returns:**
float
### setBackgroundColor(Color value) {#setBackgroundColor-java.awt.Color-}
```
public void setBackgroundColor(Color value)
```


背景色を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.awt.Color |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


最終更新時刻を取得または設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.util.Date |  |

