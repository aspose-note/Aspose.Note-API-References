---
title: "Title"
second_title: "Aspose.Note for Java API リファレンス"
description: "タイトルを表します。"
type: docs
weight: 95
url: /ja/java/com.aspose.note/title/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase)

**All Implemented Interfaces:**
com.aspose.note.ICompositeNodeT, [com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode)
```
public final class Title extends CompositeNodeBase implements ICompositeNodeT<RichText>, IPageChildNode
```

タイトルを表します。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [Title()](#Title--) | `Title` クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [&lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass)](#-T1-getChildNodes-java.lang.Class-T1--) | ノードのタイプで子ノードをすべて取得します。 |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | ノードのビジターを受け入れます。 |
| [getChildNodes(int type)](#getChildNodes-int-) |  |
| [getHorizontalOffset()](#getHorizontalOffset--) | 水平オフセットを取得または設定します。 |
| [getLastModifiedTime()](#getLastModifiedTime--) | 最終更新時刻を取得または設定します。 |
| [getTitleDate()](#getTitleDate--) | タイトルの日付の文字列表現を取得または設定します。 |
| [getTitleText()](#getTitleText--) | タイトルのテキストを取得または設定します。 |
| [getTitleTime()](#getTitleTime--) | タイトルの時刻の文字列表現を取得または設定します。 |
| [getVerticalOffset()](#getVerticalOffset--) | 垂直オフセットを取得または設定します。 |
| [isComposite()](#isComposite--) | このノードが複合ノードかどうかを示す値を取得します。 |
| [iterator()](#iterator--) | [Title](../../com.aspose.note/title) の子ノードを反復処理する列挙子を返します。 |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | 水平オフセットを取得または設定します。 |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | 最終更新時刻を取得または設定します。 |
| [setTitleDate(RichText value)](#setTitleDate-com.aspose.note.RichText-) | タイトルの日付の文字列表現を取得または設定します。 |
| [setTitleText(RichText value)](#setTitleText-com.aspose.note.RichText-) | タイトルのテキストを取得または設定します。 |
| [setTitleTime(RichText value)](#setTitleTime-com.aspose.note.RichText-) | タイトルの時刻の文字列表現を取得または設定します。 |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | 垂直オフセットを取得または設定します。 |
### Title() {#Title--}
```
public Title()
```


`Title` クラスの新しいインスタンスを初期化します。

### &lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass) {#-T1-getChildNodes-java.lang.Class-T1--}
```
public List<T1> <T1>getChildNodes(Class<T1> typeParameterClass)
```


ノードのタイプで子ノードをすべて取得します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| typeParameterClass | java.lang.Class&lt;T1&gt; |  |

**Returns:**
java.util.List&lt;T1&gt; - 子ノードのリスト。

`T1`: 返されたリスト内の要素の型です。
### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


ノードのビジターを受け入れます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | `DocumentVisitor` から派生したクラスのオブジェクト。 |

### getChildNodes(int type) {#getChildNodes-int-}
```
public List<INode> getChildNodes(int type)
```




**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| タイプ | int |  |

**Returns:**
java.util.List&lt;com.aspose.note.INode&gt;
### getHorizontalOffset() {#getHorizontalOffset--}
```
public final float getHorizontalOffset()
```


水平オフセットを取得または設定します。

**Returns:**
float
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


最終更新時刻を取得または設定します。

**Returns:**
java.util.Date
### getTitleDate() {#getTitleDate--}
```
public final RichText getTitleDate()
```


タイトルの日付の文字列表現を取得または設定します。

**Returns:**
[RichText](../../com.aspose.note/richtext)
### getTitleText() {#getTitleText--}
```
public RichText getTitleText()
```


タイトルのテキストを取得または設定します。

**Returns:**
[RichText](../../com.aspose.note/richtext)
### getTitleTime() {#getTitleTime--}
```
public final RichText getTitleTime()
```


タイトルの時刻の文字列表現を取得または設定します。

**Returns:**
[RichText](../../com.aspose.note/richtext)
### getVerticalOffset() {#getVerticalOffset--}
```
public final float getVerticalOffset()
```


垂直オフセットを取得または設定します。

**Returns:**
float
### isComposite() {#isComposite--}
```
public boolean isComposite()
```


このノードが複合ノードかどうかを示す値を取得します。true の場合、ノードは子ノードを持つことができます。

**Returns:**
boolean
### iterator() {#iterator--}
```
public final System.Collections.Generic.IGenericEnumerator<RichText> iterator()
```


[Title](../../com.aspose.note/title) の子ノードを反復処理する列挙子を返します。

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.note.RichText&gt; - IEnumerator。
### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public final void setHorizontalOffset(float value)
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

### setTitleDate(RichText value) {#setTitleDate-com.aspose.note.RichText-}
```
public final void setTitleDate(RichText value)
```


タイトルの日付の文字列表現を取得または設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [RichText](../../com.aspose.note/richtext) |  |

### setTitleText(RichText value) {#setTitleText-com.aspose.note.RichText-}
```
public final void setTitleText(RichText value)
```


タイトルのテキストを取得または設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [RichText](../../com.aspose.note/richtext) |  |

### setTitleTime(RichText value) {#setTitleTime-com.aspose.note.RichText-}
```
public final void setTitleTime(RichText value)
```


タイトルの時刻の文字列表現を取得または設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [RichText](../../com.aspose.note/richtext) |  |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public final void setVerticalOffset(float value)
```


垂直オフセットを取得または設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | float |  |

