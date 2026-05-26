---
title: "Page"
second_title: "Aspose.Note for Java API リファレンス"
description: "ページを表します。"
type: docs
weight: 69
url: /ja/java/com.aspose.note/page/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode
```
public final class Page extends CompositeNode<IPageChildNode>
```

ページを表します。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [Page()](#Page--) | `Page` クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | ノードのビジターを受け入れます。 |
| [deepClone()](#deepClone--) | ページをクローンします。 |
| [deepClone(boolean cloneHistory)](#deepClone-boolean-) | ページをクローンします。 |
| [getAuthor()](#getAuthor--) | 作者を取得または設定します。 |
| [getBackgroundColor()](#getBackgroundColor--) | ページの背景色を取得または設定します。 |
| [getCreationTime()](#getCreationTime--) | 作成時間を取得または設定します。 |
| [getLastModifiedTime()](#getLastModifiedTime--) | 最終更新時刻を取得または設定します。 |
| [getLevel()](#getLevel--) | レベルを取得または設定します。 |
| [getMargin()](#getMargin--) | 余白を取得または設定します。 |
| [getPageContentRevisionSummary()](#getPageContentRevisionSummary--) | ページとその子ノードのリビジョンサマリーを取得または設定します。 |
| [getPageLayoutSize()](#getPageLayoutSize--) | エディタに表示されるページのレイアウトサイズを取得します。 |
| [getSizeType()](#getSizeType--) | ページのサイズタイプを取得または設定します。 |
| [getTitle()](#getTitle--) | タイトルを取得または設定します。 |
| [isConflictPage()](#isConflictPage--) | このページが競合ページかどうかを示す値を取得または設定します。 |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | 作者を取得または設定します。 |
| [setBackgroundColor(Color value)](#setBackgroundColor-java.awt.Color-) | ページの背景色を取得または設定します。 |
| [setConflictPage(boolean value)](#setConflictPage-boolean-) | このページが競合ページかどうかを示す値を取得または設定します。 |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | 作成時間を取得または設定します。 |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | 最終更新時刻を取得または設定します。 |
| [setLevel(byte value)](#setLevel-byte-) | レベルを取得または設定します。 |
| [setMargin(Margins value)](#setMargin-com.aspose.note.Margins-) | 余白を取得または設定します。 |
| [setPageContentRevisionSummary(RevisionSummary value)](#setPageContentRevisionSummary-com.aspose.note.RevisionSummary-) | ページとその子ノードのリビジョンサマリーを取得または設定します。 |
| [setPageLayoutSize(Dimension2D value)](#setPageLayoutSize-java.awt.geom.Dimension2D-) | エディターに表示されるページのレイアウトサイズを設定します。 |
| [setSizeType(int value)](#setSizeType-int-) | ページのサイズタイプを取得または設定します。 |
| [setTitle(Title value)](#setTitle-com.aspose.note.Title-) | タイトルを取得または設定します。 |
### Page() {#Page--}
```
public Page()
```


`Page` クラスの新しいインスタンスを初期化します。

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


ノードのビジターを受け入れます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | `DocumentVisitor` から派生したクラスのオブジェクト。 |

### deepClone() {#deepClone--}
```
public final Page deepClone()
```


ページをクローンします。

**Returns:**
[Page](../../com.aspose.note/page) - A clone of the page.
### deepClone(boolean cloneHistory) {#deepClone-boolean-}
```
public final Page deepClone(boolean cloneHistory)
```


ページをクローンします。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| cloneHistory | boolean | ページの履歴をクローンするかどうかを指定します。 |

**Returns:**
[Page](../../com.aspose.note/page) - A clone of the page.
### getAuthor() {#getAuthor--}
```
public String getAuthor()
```


作者を取得または設定します。

**Returns:**
java.lang.String
### getBackgroundColor() {#getBackgroundColor--}
```
public final Color getBackgroundColor()
```


ページの背景色を取得または設定します。

**Returns:**
java.awt.Color
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
### getLevel() {#getLevel--}
```
public byte getLevel()
```


レベルを取得または設定します。

**Returns:**
byte
### getMargin() {#getMargin--}
```
public Margins getMargin()
```


余白を取得または設定します。

**Returns:**
[Margins](../../com.aspose.note/margins)
### getPageContentRevisionSummary() {#getPageContentRevisionSummary--}
```
public RevisionSummary getPageContentRevisionSummary()
```


ページとその子ノードのリビジョンサマリーを取得または設定します。

**Returns:**
[RevisionSummary](../../com.aspose.note/revisionsummary)
### getPageLayoutSize() {#getPageLayoutSize--}
```
public final Dimension2D getPageLayoutSize()
```


エディタに表示されるページのレイアウトサイズを取得します。

--------------------

この値は Microsoft OneNote アプリケーションによって、ドキュメントが開かれたときに基になるページレイアウトを表示するために使用されます。印刷やドキュメントの保存には影響しません。Page.SizeType プロパティが PageSizeType.SizeByContent に設定されている場合、このプロパティはコンテンツの実際のサイズを返します。

**Returns:**
java.awt.geom.Dimension2D
### getSizeType() {#getSizeType--}
```
public final int getSizeType()
```


ページのサイズタイプを取得または設定します。

--------------------

デフォルトでは、ページは自動的にサイズ変更されます。デフォルト値は [PageSizeType.SizeByContent](../../com.aspose.note/pagesizetype\#SizeByContent) です。

**Returns:**
int
### getTitle() {#getTitle--}
```
public Title getTitle()
```


タイトルを取得または設定します。

値: `Title`。

**Returns:**
[Title](../../com.aspose.note/title)
### isConflictPage() {#isConflictPage--}
```
public final boolean isConflictPage()
```


このページが競合ページかどうかを示す値を取得または設定します。

--------------------

競合ページは、2 人のユーザーが同じコンテンツを更新しようとしたときに発生します。この場合、最初のユーザーの変更は通常どおり書き込まれますが、別のユーザーの変更はマージできません。そのため、ページのコピーが作成され、競合としてマークされます。

このバージョンでは、競合は最初のユーザーの変更を優先して解決されます。そのため、ドキュメントに競合ページがある場合、履歴には表示されますが、保存時にはスキップされます。このフラグをリセットすれば、これらのページを通常のページと同様に履歴に保存することが可能です。

競合ページの操作に関する詳細なサンプルはオンラインドキュメントで確認できます。

**Returns:**
boolean
### setAuthor(String value) {#setAuthor-java.lang.String-}
```
public void setAuthor(String value)
```


作者を取得または設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String |  |

### setBackgroundColor(Color value) {#setBackgroundColor-java.awt.Color-}
```
public final void setBackgroundColor(Color value)
```


ページの背景色を取得または設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.awt.Color |  |

### setConflictPage(boolean value) {#setConflictPage-boolean-}
```
public final void setConflictPage(boolean value)
```


このページが競合ページかどうかを示す値を取得または設定します。

--------------------

競合ページは、2 人のユーザーが同じコンテンツを更新しようとしたときに発生します。この場合、最初のユーザーの変更は通常どおり書き込まれますが、別のユーザーの変更はマージできません。そのため、ページのコピーが作成され、競合としてマークされます。

このバージョンでは、競合は最初のユーザーの変更を優先して解決されます。そのため、ドキュメントに競合ページがある場合、履歴には表示されますが、保存時にはスキップされます。このフラグをリセットすれば、これらのページを通常のページと同様に履歴に保存することが可能です。

競合ページの操作に関する詳細なサンプルはオンラインドキュメントで確認できます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean |  |

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

### setLevel(byte value) {#setLevel-byte-}
```
public void setLevel(byte value)
```


レベルを取得または設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | byte |  |

### setMargin(Margins value) {#setMargin-com.aspose.note.Margins-}
```
public void setMargin(Margins value)
```


余白を取得または設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [Margins](../../com.aspose.note/margins) |  |

### setPageContentRevisionSummary(RevisionSummary value) {#setPageContentRevisionSummary-com.aspose.note.RevisionSummary-}
```
public void setPageContentRevisionSummary(RevisionSummary value)
```


ページとその子ノードのリビジョンサマリーを取得または設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [RevisionSummary](../../com.aspose.note/revisionsummary) |  |

### setPageLayoutSize(Dimension2D value) {#setPageLayoutSize-java.awt.geom.Dimension2D-}
```
public final void setPageLayoutSize(Dimension2D value)
```


エディターに表示されるページのレイアウトサイズを設定します。

--------------------

この値は Microsoft OneNote アプリケーションによって、ドキュメントが開かれたときに基になるページレイアウトを表示するために使用されます。印刷やドキュメントの保存には影響しません。Page.SizeType プロパティが PageSizeType.SizeByContent に設定されている場合、このプロパティはコンテンツの実際のサイズを返します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.awt.geom.Dimension2D |  |

### setSizeType(int value) {#setSizeType-int-}
```
public final void setSizeType(int value)
```


ページのサイズタイプを取得または設定します。

--------------------

デフォルトでは、ページは自動的にサイズ変更されます。デフォルト値は [PageSizeType.SizeByContent](../../com.aspose.note/pagesizetype\#SizeByContent) です。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int |  |

### setTitle(Title value) {#setTitle-com.aspose.note.Title-}
```
public void setTitle(Title value)
```


タイトルを取得または設定します。

値: `Title`。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [Title](../../com.aspose.note/title) |  |

