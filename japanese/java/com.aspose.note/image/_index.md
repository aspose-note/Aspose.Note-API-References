---
title: "画像"
second_title: "Aspose.Note for Java API リファレンス"
description: "画像を表します。"
type: docs
weight: 33
url: /ja/java/com.aspose.note/image/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode

**All Implemented Interfaces:**
[com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode), [com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode), [com.aspose.note.ITaggable](../../com.aspose.note/itaggable)
```
public final class Image extends CompositeNode<Loop> implements IPageChildNode, IOutlineElementChildNode, ITaggable
```

画像を表します。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [Image(String path)](#Image-java.lang.String-) | `Image` クラスの新しいインスタンスを初期化します。 |
| [Image(String fileName, InputStream imageStream)](#Image-java.lang.String-java.io.InputStream-) | `Image` クラスの新しいインスタンスを初期化します。 |
| [Image()](#Image--) | `Image` クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | ノードのビジターを受け入れます。 |
| [getAlignment()](#getAlignment--) | 配置を取得します。 |
| [getAlternativeTextDescription()](#getAlternativeTextDescription--) | 画像の代替テキストの本文を取得します。 |
| [getAlternativeTextTitle()](#getAlternativeTextTitle--) | 画像の代替テキストのタイトルを取得します。 |
| [getBytes()](#getBytes--) | 画像データストアを取得します。 |
| [getFileName()](#getFileName--) | ファイル名を取得します。 |
| [getFilePath()](#getFilePath--) | 画像ファイルへのパスを取得します。 |
| [getFormat()](#getFormat--) | 画像の形式を取得します。 |
| [getHeight()](#getHeight--) | 高さを取得します。 |
| [getHorizontalOffset()](#getHorizontalOffset--) | 水平オフセットを取得します。 |
| [getHyperlinkUrl()](#getHyperlinkUrl--) | 画像に関連付けられたハイパーリンクを取得します。 |
| [getLastModifiedTime()](#getLastModifiedTime--) | 最終更新時刻を取得します。 |
| [getOriginalHeight()](#getOriginalHeight--) | 元の高さを取得します。 |
| [getOriginalWidth()](#getOriginalWidth--) | 元の幅を取得します。 |
| [getTags()](#getTags--) | 画像のすべてのタグのリストを取得します。 |
| [getVerticalOffset()](#getVerticalOffset--) | 垂直オフセットを取得します。 |
| [getWidth()](#getWidth--) | 幅を取得します。 |
| [isBackground()](#isBackground--) | 画像が背景画像かどうかを取得します。 |
| [replace(Image newImage)](#replace-com.aspose.note.Image-) | 提供された Image オブジェクトのデータで現在の画像データを置き換えます。 |
| [setAlignment(int value)](#setAlignment-int-) | 配置を設定します。 |
| [setAlternativeTextDescription(String value)](#setAlternativeTextDescription-java.lang.String-) | 画像の代替テキストの本文を設定します。 |
| [setAlternativeTextTitle(String value)](#setAlternativeTextTitle-java.lang.String-) | 画像の代替テキストのタイトルを設定します。 |
| [setBackground(boolean value)](#setBackground-boolean-) | 画像が背景画像かどうかを取得します。 |
| [setHeight(float value)](#setHeight-float-) | 高さを設定します。 |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | 水平オフセットを設定します。 |
| [setHyperlinkUrl(String value)](#setHyperlinkUrl-java.lang.String-) | 画像に関連付けられたハイパーリンクを設定します。 |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | 最終更新時刻を設定します。 |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | 垂直オフセットを設定します。 |
| [setWidth(float value)](#setWidth-float-) | 幅を設定します。 |
### Image(String path) {#Image-java.lang.String-}
```
public Image(String path)
```


`Image` クラスの新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| パス | java.lang.String | `Image` を作成するためのファイルへのパスを含む文字列です。 |

### Image(String fileName, InputStream imageStream) {#Image-java.lang.String-java.io.InputStream-}
```
public Image(String fileName, InputStream imageStream)
```


`Image` クラスの新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| ファイル名 | java.lang.String | 画像の名前です。 |
| imageStream | java.io.InputStream | 画像を含むストリームです。 |

### Image() {#Image--}
```
public Image()
```


`Image` クラスの新しいインスタンスを初期化します。

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


ノードのビジターを受け入れます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | `DocumentVisitor` から派生したクラスのオブジェクト。 |

### getAlignment() {#getAlignment--}
```
public int getAlignment()
```


配置を取得します。

**Returns:**
int
### getAlternativeTextDescription() {#getAlternativeTextDescription--}
```
public final String getAlternativeTextDescription()
```


画像の代替テキストの本文を取得します。

**Returns:**
java.lang.String
### getAlternativeTextTitle() {#getAlternativeTextTitle--}
```
public final String getAlternativeTextTitle()
```


画像の代替テキストのタイトルを取得します。

**Returns:**
java.lang.String
### getBytes() {#getBytes--}
```
public byte[] getBytes()
```


画像データストアを取得します。

**Returns:**
byte[]
### getFileName() {#getFileName--}
```
public String getFileName()
```


ファイル名を取得します。

**Returns:**
java.lang.String
### getFilePath() {#getFilePath--}
```
public String getFilePath()
```


画像ファイルへのパスを取得します。

**Returns:**
java.lang.String
### getFormat() {#getFormat--}
```
public final System.Drawing.Imaging.ImageFormat getFormat()
```


画像の形式を取得します。

**Returns:**
com.aspose.ms.System.Drawing.Imaging.ImageFormat
### getHeight() {#getHeight--}
```
public final float getHeight()
```


高さを取得します。これは MS OneNote ドキュメント内の画像の実際の高さです。

**Returns:**
float
### getHorizontalOffset() {#getHorizontalOffset--}
```
public float getHorizontalOffset()
```


水平オフセットを取得します。

**Returns:**
float
### getHyperlinkUrl() {#getHyperlinkUrl--}
```
public String getHyperlinkUrl()
```


画像に関連付けられたハイパーリンクを取得します。

**Returns:**
java.lang.String
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


最終更新時刻を取得します。

**Returns:**
java.util.Date
### getOriginalHeight() {#getOriginalHeight--}
```
public float getOriginalHeight()
```


元の高さを取得します。これはリサイズ前の画像の元の幅です。

**Returns:**
float
### getOriginalWidth() {#getOriginalWidth--}
```
public float getOriginalWidth()
```


元の幅を取得します。これはリサイズ前の画像の元の幅です。

**Returns:**
float
### getTags() {#getTags--}
```
public final System.Collections.Generic.List<ITag> getTags()
```


画像のすべてのタグのリストを取得します。

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.note.ITag&gt;
### getVerticalOffset() {#getVerticalOffset--}
```
public float getVerticalOffset()
```


垂直オフセットを取得します。

**Returns:**
float
### getWidth() {#getWidth--}
```
public final float getWidth()
```


幅を取得します。これは MS OneNote ドキュメント内の画像の実際の幅です。

**Returns:**
float
### isBackground() {#isBackground--}
```
public final boolean isBackground()
```


画像が背景画像かどうかを取得します。

**Returns:**
boolean
### replace(Image newImage) {#replace-com.aspose.note.Image-}
```
public void replace(Image newImage)
```


提供された Image オブジェクトのデータで現在の画像データを置き換えます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| newImage | [Image](../../com.aspose.note/image) |  |

### setAlignment(int value) {#setAlignment-int-}
```
public void setAlignment(int value)
```


配置を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int |  |

### setAlternativeTextDescription(String value) {#setAlternativeTextDescription-java.lang.String-}
```
public final void setAlternativeTextDescription(String value)
```


画像の代替テキストの本文を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String |  |

### setAlternativeTextTitle(String value) {#setAlternativeTextTitle-java.lang.String-}
```
public final void setAlternativeTextTitle(String value)
```


画像の代替テキストのタイトルを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String |  |

### setBackground(boolean value) {#setBackground-boolean-}
```
public final void setBackground(boolean value)
```


画像が背景画像かどうかを取得します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean |  |

### setHeight(float value) {#setHeight-float-}
```
public final void setHeight(float value)
```


高さを設定します。これは MS OneNote ドキュメント内の画像の実際の高さです。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | float |  |

### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public void setHorizontalOffset(float value)
```


水平オフセットを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | float |  |

### setHyperlinkUrl(String value) {#setHyperlinkUrl-java.lang.String-}
```
public void setHyperlinkUrl(String value)
```


画像に関連付けられたハイパーリンクを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


最終更新時刻を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.util.Date |  |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public void setVerticalOffset(float value)
```


垂直オフセットを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | float |  |

### setWidth(float value) {#setWidth-float-}
```
public final void setWidth(float value)
```


幅を設定します。これは MS OneNote ドキュメント内の画像の実際の幅です。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | float |  |

