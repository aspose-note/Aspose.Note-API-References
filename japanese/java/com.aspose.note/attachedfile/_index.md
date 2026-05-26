---
title: "AttachedFile"
second_title: "Aspose.Note for Java API リファレンス"
description: "添付ファイルを表します。"
type: docs
weight: 11
url: /ja/java/com.aspose.note/attachedfile/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node)

**All Implemented Interfaces:**
[com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode), [com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode), [com.aspose.note.ITaggable](../../com.aspose.note/itaggable)
```
public class AttachedFile extends Node implements IPageChildNode, IOutlineElementChildNode, ITaggable
```

添付ファイルを表します。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [AttachedFile(String path)](#AttachedFile-java.lang.String-) | `AttachedFile` クラスの新しいインスタンスを初期化します。 |
| [AttachedFile(String path, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)](#AttachedFile-java.lang.String-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-) | `AttachedFile` クラスの新しいインスタンスを初期化します。 |
| [AttachedFile(String fileName, InputStream attachedFileStream)](#AttachedFile-java.lang.String-java.io.InputStream-) | `AttachedFile` クラスの新しいインスタンスを初期化します。 |
| [AttachedFile(String fileName, InputStream attachedFileStream, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)](#AttachedFile-java.lang.String-java.io.InputStream-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-) | `AttachedFile` クラスの新しいインスタンスを初期化します。 |
| [AttachedFile()](#AttachedFile--) | `AttachedFile` クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | ノードのビジターを受け入れます。 |
| [getAlignment()](#getAlignment--) | 配置を取得します。 |
| [getAlternativeTextDescription()](#getAlternativeTextDescription--) | 添付ファイルのアイコンの代替テキストとしての本文を取得または設定します。 |
| [getAlternativeTextTitle()](#getAlternativeTextTitle--) | 添付ファイルのアイコンの代替テキストのタイトルを取得または設定します。 |
| [getBytes()](#getBytes--) | 埋め込みファイルのバイナリ データを取得します。 |
| [getExtension()](#getExtension--) | 埋め込みファイルの拡張子を取得します。 |
| [getFileName()](#getFileName--) | 埋め込みファイルの名前を取得します。 |
| [getFilePath()](#getFilePath--) | 元ファイルへのパスを取得します。 |
| [getHeight()](#getHeight--) | 埋め込みファイルアイコンの元の高さを取得します。 |
| [getHorizontalOffset()](#getHorizontalOffset--) | 水平オフセットを取得します。 |
| [getIcon()](#getIcon--) | 埋め込みファイルに関連付けられたアイコンのバイナリ データを取得します。 |
| [getIconExtension()](#getIconExtension--) | アイコンの拡張子を取得します。 |
| [getLastModifiedTime()](#getLastModifiedTime--) | 最終更新時刻を取得します。 |
| [getMaxHeight()](#getMaxHeight--) | 埋め込みファイル アイコンを表示するための最大高さを取得します。 |
| [getMaxWidth()](#getMaxWidth--) | 埋め込みファイル アイコンを表示するための最大幅を取得します。 |
| [getParsingErrorInfo()](#getParsingErrorInfo--) | ファイルにアクセス中に発生したエラーに関するデータを取得します。 |
| [getTags()](#getTags--) | 添付ファイルのタグ一覧を取得します。 |
| [getText()](#getText--) | 埋め込みファイルのテキスト表現を取得します。 |
| [getVerticalOffset()](#getVerticalOffset--) | 垂直オフセットを取得します。 |
| [getWidth()](#getWidth--) | 埋め込みファイル アイコンの元の幅を取得します。 |
| [isPrintout()](#isPrintout--) | ファイルのビューが印刷物かどうかを示す値を取得します。 |
| [isSizeSetByUser()](#isSizeSetByUser--) | アイコンのサイズの値がユーザーによって明示的に更新されたかどうかを示す値を取得します。 |
| [setAlignment(int value)](#setAlignment-int-) | 配置を設定します。 |
| [setAlternativeTextDescription(String value)](#setAlternativeTextDescription-java.lang.String-) | 添付ファイルのアイコンの代替テキストとしての本文を取得または設定します。 |
| [setAlternativeTextTitle(String value)](#setAlternativeTextTitle-java.lang.String-) | 添付ファイルのアイコンの代替テキストのタイトルを取得または設定します。 |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | 水平オフセットを設定します。 |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | 最終更新日時を設定します。 |
| [setMaxHeight(float value)](#setMaxHeight-float-) | 埋め込みファイル アイコンを表示するための最大高さを設定します。 |
| [setMaxWidth(float value)](#setMaxWidth-float-) | 埋め込みファイル アイコンを表示するための最大幅を設定します。 |
| [setPrintout(boolean value)](#setPrintout-boolean-) | ファイルのビューが印刷物かどうかを示す値を設定します。 |
| [setSizeSetByUser(boolean value)](#setSizeSetByUser-boolean-) | アイコンのサイズの値がユーザーによって明示的に更新されたかどうかを示す値を設定します。 |
| [setText(String value)](#setText-java.lang.String-) | 埋め込みファイルのテキスト表現を設定します。 |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | 垂直オフセットを設定します。 |
### AttachedFile(String path) {#AttachedFile-java.lang.String-}
```
public AttachedFile(String path)
```


`AttachedFile` クラスの新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| パス | java.lang.String | `AttachedFile` を作成する元となるファイルへのパスを含む文字列です。 |

### AttachedFile(String path, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat) {#AttachedFile-java.lang.String-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-}
```
public AttachedFile(String path, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)
```


`AttachedFile` クラスの新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| パス | java.lang.String | `AttachedFile` を作成する元となるファイルへのパスを含む文字列です。 |
| アイコン | java.io.InputStream | 添付ファイル用のアイコンです。 |
| アイコン形式 | com.aspose.ms.System.Drawing.Imaging.ImageFormat |  |

### AttachedFile(String fileName, InputStream attachedFileStream) {#AttachedFile-java.lang.String-java.io.InputStream-}
```
public AttachedFile(String fileName, InputStream attachedFileStream)
```


`AttachedFile` クラスの新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| ファイル名 | java.lang.String | 添付ファイルの名前。 |
| attachedFileStream | java.io.InputStream | 添付ファイルのバイトを含むストリーム。 |

### AttachedFile(String fileName, InputStream attachedFileStream, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat) {#AttachedFile-java.lang.String-java.io.InputStream-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-}
```
public AttachedFile(String fileName, InputStream attachedFileStream, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)
```


`AttachedFile` クラスの新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| ファイル名 | java.lang.String | 添付ファイルの名前。 |
| attachedFileStream | java.io.InputStream | 添付ファイルのバイトを含むストリーム。 |
| アイコン | java.io.InputStream | 添付ファイル用のアイコンです。 |
| アイコン形式 | com.aspose.ms.System.Drawing.Imaging.ImageFormat | 添付ファイルアイコンの形式。 |

### AttachedFile() {#AttachedFile--}
```
public AttachedFile()
```


`AttachedFile` クラスの新しいインスタンスを初期化します。

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


添付ファイルのアイコンの代替テキストとしての本文を取得または設定します。

**Returns:**
java.lang.String
### getAlternativeTextTitle() {#getAlternativeTextTitle--}
```
public final String getAlternativeTextTitle()
```


添付ファイルのアイコンの代替テキストのタイトルを取得または設定します。

**Returns:**
java.lang.String
### getBytes() {#getBytes--}
```
public byte[] getBytes()
```


埋め込みファイルのバイナリ データを取得します。

**Returns:**
byte[]
### getExtension() {#getExtension--}
```
public String getExtension()
```


埋め込みファイルの拡張子を取得します。

**Returns:**
java.lang.String
### getFileName() {#getFileName--}
```
public String getFileName()
```


埋め込みファイルの名前を取得します。

**Returns:**
java.lang.String
### getFilePath() {#getFilePath--}
```
public String getFilePath()
```


元ファイルへのパスを取得します。

**Returns:**
java.lang.String
### getHeight() {#getHeight--}
```
public float getHeight()
```


埋め込みファイルアイコンの元の高さを取得します。

**Returns:**
float
### getHorizontalOffset() {#getHorizontalOffset--}
```
public float getHorizontalOffset()
```


水平オフセットを取得します。

**Returns:**
float
### getIcon() {#getIcon--}
```
public byte[] getIcon()
```


埋め込みファイルに関連付けられたアイコンのバイナリ データを取得します。

**Returns:**
byte[]
### getIconExtension() {#getIconExtension--}
```
public String getIconExtension()
```


アイコンの拡張子を取得します。

**Returns:**
java.lang.String
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


最終更新時刻を取得します。

**Returns:**
java.util.Date
### getMaxHeight() {#getMaxHeight--}
```
public float getMaxHeight()
```


埋め込みファイル アイコンを表示するための最大高さを取得します。

**Returns:**
float
### getMaxWidth() {#getMaxWidth--}
```
public float getMaxWidth()
```


埋め込みファイル アイコンを表示するための最大幅を取得します。

**Returns:**
float
### getParsingErrorInfo() {#getParsingErrorInfo--}
```
public final ParsingErrorInfo getParsingErrorInfo()
```


ファイルにアクセス中に発生したエラーに関するデータを取得します。

**Returns:**
[ParsingErrorInfo](../../com.aspose.note.infrastructure/parsingerrorinfo)
### getTags() {#getTags--}
```
public final System.Collections.Generic.List<ITag> getTags()
```


添付ファイルのタグ一覧を取得します。

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.note.ITag&gt;
### getText() {#getText--}
```
public String getText()
```


埋め込みファイルのテキスト表現を取得します。文字列は値10（改行）または13（復帰）の文字を含んではいけません。

**Returns:**
java.lang.String
### getVerticalOffset() {#getVerticalOffset--}
```
public float getVerticalOffset()
```


垂直オフセットを取得します。

**Returns:**
float
### getWidth() {#getWidth--}
```
public float getWidth()
```


埋め込みファイル アイコンの元の幅を取得します。

**Returns:**
float
### isPrintout() {#isPrintout--}
```
public boolean isPrintout()
```


ファイルのビューが印刷物かどうかを示す値を取得します。

**Returns:**
boolean
### isSizeSetByUser() {#isSizeSetByUser--}
```
public boolean isSizeSetByUser()
```


アイコンのサイズの値がユーザーによって明示的に更新されたかどうかを示す値を取得します。

**Returns:**
boolean
### setAlignment(int value) {#setAlignment-int-}
```
public void setAlignment(int value)
```


配置を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | Alignment の値。 |

### setAlternativeTextDescription(String value) {#setAlternativeTextDescription-java.lang.String-}
```
public final void setAlternativeTextDescription(String value)
```


添付ファイルのアイコンの代替テキストとしての本文を取得または設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String |  |

### setAlternativeTextTitle(String value) {#setAlternativeTextTitle-java.lang.String-}
```
public final void setAlternativeTextTitle(String value)
```


添付ファイルのアイコンの代替テキストのタイトルを取得または設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String |  |

### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public void setHorizontalOffset(float value)
```


水平オフセットを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | float | Offsets の値。 |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


最終更新日時を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.util.Date | Date の値。 |

### setMaxHeight(float value) {#setMaxHeight-float-}
```
public void setMaxHeight(float value)
```


埋め込みファイル アイコンを表示するための最大高さを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | float | 最大高さの値。 |

### setMaxWidth(float value) {#setMaxWidth-float-}
```
public void setMaxWidth(float value)
```


埋め込みファイル アイコンを表示するための最大幅を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | float | 最大幅の値。 |

### setPrintout(boolean value) {#setPrintout-boolean-}
```
public void setPrintout(boolean value)
```


ファイルのビューが印刷物かどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | 新しい値。 |

### setSizeSetByUser(boolean value) {#setSizeSetByUser-boolean-}
```
public void setSizeSetByUser(boolean value)
```


アイコンのサイズの値がユーザーによって明示的に更新されたかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | 新しい値。 |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


埋め込みファイルのテキスト表現を設定します。文字列は値10（改行）または13（復帰）の文字を含んではいけません。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | Text の値。 |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public void setVerticalOffset(float value)
```


垂直オフセットを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | float | Offset の値。 |

