---
title: "IndentatedNode"
second_title: "Aspose.Note for Java API リファレンス"
description: "子ノードの相対インデントを持つノードの基本クラスです。"
type: docs
weight: 37
url: /ja/java/com.aspose.note/indentatednode/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode

**All Implemented Interfaces:**
com.aspose.note.IIndentatedNodeExtended
```
public class IndentatedNode<T,Self> extends CompositeNode<T> implements IIndentatedNodeExtended
```

子ノードの相対インデントを持つノードの基本クラスです。

`T`: 複合ノード内の要素の型です。

T :
Self :
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getIndentPosition()](#getIndentPosition--) | インデント位置を取得または設定します。 |
| [getInternalIndentPosition()](#getInternalIndentPosition--) | インデントサイズを取得するために RgOutlineIndentDistance 配列で合計する項目数を取得します。 |
| [setIndentPosition(byte value)](#setIndentPosition-byte-) | インデント位置を取得または設定します。 |
| [setIndentPosition(int value)](#setIndentPosition-int-) |  |
### getIndentPosition() {#getIndentPosition--}
```
public final byte getIndentPosition()
```


インデント位置を取得または設定します。

**Returns:**
byte
### getInternalIndentPosition() {#getInternalIndentPosition--}
```
public int getInternalIndentPosition()
```


インデントサイズを取得するために RgOutlineIndentDistance 配列で合計する項目数を取得します。

**Returns:**
int
### setIndentPosition(byte value) {#setIndentPosition-byte-}
```
public final Self setIndentPosition(byte value)
```


インデント位置を取得または設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | byte |  |

**Returns:**
Self
### setIndentPosition(int value) {#setIndentPosition-int-}
```
public final Self setIndentPosition(int value)
```




**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int |  |

**Returns:**
Self
