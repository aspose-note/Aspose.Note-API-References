---
title: "アウトライン"
second_title: "Aspose.Note for Java API リファレンス"
description: "アウトラインを表します。"
type: docs
weight: 66
url: /ja/java/com.aspose.note/outline/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode, com.aspose.note.IndentatedNode

**All Implemented Interfaces:**
[com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode)
```
public final class Outline extends IndentatedNode<IOutlineChildNode,Outline> implements IPageChildNode
```

アウトラインを表します。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [Outline()](#Outline--) | 新しい [Outline](../../com.aspose.note/outline) クラスのインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | ノードのビジターを受け入れます。 |
| [getDescendantsCannotBeMoved()](#getDescendantsCannotBeMoved--) | アウトラインの子孫が移動可能かどうかを取得します。 |
| [getHorizontalOffset()](#getHorizontalOffset--) | 水平オフセットを取得または設定します。 |
| [getInternalIndentPosition()](#getInternalIndentPosition--) |  |
| [getLastModifiedTime()](#getLastModifiedTime--) | 最終更新時刻を取得または設定します。 |
| [getMaxHeight()](#getMaxHeight--) | 最大高さを取得または設定します。 |
| [getMaxWidth()](#getMaxWidth--) | 最大幅を取得または設定します。 |
| [getMinWidth()](#getMinWidth--) | 最小幅を取得または設定します。 |
| [getReservedWidth()](#getReservedWidth--) | 予約幅を取得または設定します。 |
| [getVerticalOffset()](#getVerticalOffset--) | 垂直オフセットを取得または設定します。 |
| [setDescendantsCannotBeMoved(boolean value)](#setDescendantsCannotBeMoved-boolean-) | アウトラインの子孫が移動可能かどうかを取得します。 |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | 水平オフセットを取得または設定します。 |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | 最終更新時刻を取得または設定します。 |
| [setMaxHeight(float value)](#setMaxHeight-float-) | 最大高さを取得または設定します。 |
| [setMaxWidth(float value)](#setMaxWidth-float-) | 最大幅を取得または設定します。 |
| [setMinWidth(float value)](#setMinWidth-float-) | 最小幅を取得または設定します。 |
| [setReservedWidth(float value)](#setReservedWidth-float-) | 予約幅を取得または設定します。 |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | 垂直オフセットを取得または設定します。 |
### Outline() {#Outline--}
```
public Outline()
```


新しい [Outline](../../com.aspose.note/outline) クラスのインスタンスを初期化します。

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


ノードのビジターを受け入れます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | `DocumentVisitor` から派生したクラスのオブジェクト。 |

### getDescendantsCannotBeMoved() {#getDescendantsCannotBeMoved--}
```
public boolean getDescendantsCannotBeMoved()
```


アウトラインの子孫が移動可能かどうかを取得します。

**Returns:**
boolean
### getHorizontalOffset() {#getHorizontalOffset--}
```
public float getHorizontalOffset()
```


水平オフセットを取得または設定します。

**Returns:**
float
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
### getMaxHeight() {#getMaxHeight--}
```
public float getMaxHeight()
```


最大高さを取得または設定します。

**Returns:**
float
### getMaxWidth() {#getMaxWidth--}
```
public float getMaxWidth()
```


最大幅を取得または設定します。

**Returns:**
float
### getMinWidth() {#getMinWidth--}
```
public float getMinWidth()
```


最小幅を取得または設定します。

**Returns:**
float
### getReservedWidth() {#getReservedWidth--}
```
public float getReservedWidth()
```


予約幅を取得または設定します。

**Returns:**
float
### getVerticalOffset() {#getVerticalOffset--}
```
public float getVerticalOffset()
```


垂直オフセットを取得または設定します。

**Returns:**
float
### setDescendantsCannotBeMoved(boolean value) {#setDescendantsCannotBeMoved-boolean-}
```
public void setDescendantsCannotBeMoved(boolean value)
```


アウトラインの子孫が移動可能かどうかを取得します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean |  |

### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public void setHorizontalOffset(float value)
```


水平オフセットを取得または設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | float |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


最終更新時刻を取得または設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.util.Date |  |

### setMaxHeight(float value) {#setMaxHeight-float-}
```
public void setMaxHeight(float value)
```


最大高さを取得または設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | float |  |

### setMaxWidth(float value) {#setMaxWidth-float-}
```
public void setMaxWidth(float value)
```


最大幅を取得または設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | float |  |

### setMinWidth(float value) {#setMinWidth-float-}
```
public void setMinWidth(float value)
```


最小幅を取得または設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | float |  |

### setReservedWidth(float value) {#setReservedWidth-float-}
```
public void setReservedWidth(float value)
```


予約幅を取得または設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | float |  |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public void setVerticalOffset(float value)
```


垂直オフセットを取得または設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | float |  |

