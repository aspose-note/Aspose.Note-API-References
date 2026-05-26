---
title: "OutlineElement"
second_title: "Aspose.Note for Java API リファレンス"
description: "OutlineElement を表します。"
type: docs
weight: 67
url: /ja/java/com.aspose.note/outlineelement/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode, com.aspose.note.IndentatedNode

**All Implemented Interfaces:**
[com.aspose.note.IOutlineChildNode](../../com.aspose.note/ioutlinechildnode), [com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode)
```
public final class OutlineElement extends IndentatedNode<IOutlineElementChildNode,OutlineElement> implements IOutlineChildNode, IOutlineElementChildNode
```

OutlineElement を表します。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [OutlineElement()](#OutlineElement--) | `OutlineElement` クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | ノードのビジターを受け入れます。 |
| [getAuthorMostRecent()](#getAuthorMostRecent--) | アウトライン要素の最新の作成者を取得します。 |
| [getAuthorOriginal()](#getAuthorOriginal--) | アウトライン要素の元の作成者を取得します。 |
| [getCreationTime()](#getCreationTime--) | 作成時間を取得または設定します。 |
| [getLastModifiedTime()](#getLastModifiedTime--) | 最終更新時刻を取得または設定します。 |
| [getNumberList()](#getNumberList--) | 番号付きリストヘッダーのスタイルを取得または設定します。 |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | 作成時間を取得または設定します。 |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | 最終更新時刻を取得または設定します。 |
| [setNumberList(NumberList value)](#setNumberList-com.aspose.note.NumberList-) | 番号付きリストヘッダーのスタイルを取得または設定します。 |
### OutlineElement() {#OutlineElement--}
```
public OutlineElement()
```


`OutlineElement` クラスの新しいインスタンスを初期化します。

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


ノードのビジターを受け入れます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | `DocumentVisitor` から派生したクラスのオブジェクト。 |

### getAuthorMostRecent() {#getAuthorMostRecent--}
```
public final String getAuthorMostRecent()
```


アウトライン要素の最新の作成者を取得します。

値: 最新の作成者。

**Returns:**
java.lang.String
### getAuthorOriginal() {#getAuthorOriginal--}
```
public final String getAuthorOriginal()
```


アウトライン要素の元の作成者を取得します。

値: 元の作成者。

**Returns:**
java.lang.String
### getCreationTime() {#getCreationTime--}
```
public Date getCreationTime()
```


作成時間を取得または設定します。

**Returns:**
java.util.Date
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


最終更新時刻を取得または設定します。

**Returns:**
java.util.Date
### getNumberList() {#getNumberList--}
```
public NumberList getNumberList()
```


番号付きリストヘッダーのスタイルを取得または設定します。

**Returns:**
[NumberList](../../com.aspose.note/numberlist)
### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public void setCreationTime(Date value)
```


作成時間を取得または設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.util.Date |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


最終更新時刻を取得または設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.util.Date |  |

### setNumberList(NumberList value) {#setNumberList-com.aspose.note.NumberList-}
```
public void setNumberList(NumberList value)
```


番号付きリストヘッダーのスタイルを取得または設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [NumberList](../../com.aspose.note/numberlist) |  |

