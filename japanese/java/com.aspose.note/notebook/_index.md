---
title: "ノートブック"
second_title: "Aspose.Note for Java API リファレンス"
description: "Aspose.Note ノートブックを表します。"
type: docs
weight: 56
url: /ja/java/com.aspose.note/notebook/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.note.INotebookChildNode](../../com.aspose.note/inotebookchildnode), com.aspose.ms.System.Collections.Generic.IGenericEnumerable
```
public class Notebook implements INotebookChildNode, System.Collections.Generic.IGenericEnumerable<INotebookChildNode>
```

Aspose.Note ノートブックを表します。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [Notebook()](#Notebook--) | `Notebook` クラスの新しいインスタンスを初期化します。 |
| [Notebook(String filePath)](#Notebook-java.lang.String-) | `Notebook` クラスの新しいインスタンスを初期化します。 |
| [Notebook(String filePath, NotebookLoadOptions loadOptions)](#Notebook-java.lang.String-com.aspose.note.NotebookLoadOptions-) | `Notebook` クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [&lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass)](#-T1-getChildNodes-java.lang.Class-T1--) | ノードのタイプで子ノードをすべて取得します。 |
| [appendChild(INotebookChildNode newChild)](#appendChild-com.aspose.note.INotebookChildNode-) | ノードをリストの末尾に追加します。 |
| [getColor()](#getColor--) | 色を取得または設定します。 |
| [getCount()](#getCount--) | `Notebook` に含まれる要素数を取得します。 |
| [getDisplayName()](#getDisplayName--) | 表示名を取得または設定します。 |
| [getFileFormat()](#getFileFormat--) | ファイル形式を取得します（OneNote 2010、OneNote Online）。 |
| [getGuid()](#getGuid--) | オブジェクトのグローバルに一意な ID を取得します。 |
| [getGuidInternal()](#getGuidInternal--) |  |
| [get_Item(int index)](#get-Item-int-) | 指定されたインデックスでノートブックの子ノードを取得します。 |
| [isHistoryEnabled()](#isHistoryEnabled--) | 履歴が有効かどうかを示す値を取得または設定します。 |
| [iterator()](#iterator--) | `Notebook` の子ノードを列挙する列挙子を返します。 |
| [loadChildDocument(InputStream stream)](#loadChildDocument-java.io.InputStream-) | 子ドキュメントノードを追加します。 |
| [loadChildDocument(InputStream stream, LoadOptions loadOptions)](#loadChildDocument-java.io.InputStream-com.aspose.note.LoadOptions-) | 子ドキュメントノードを追加します。 |
| [loadChildDocument(String filePath)](#loadChildDocument-java.lang.String-) | 子ドキュメントノードを追加します。 |
| [loadChildDocument(String filePath, LoadOptions loadOptions)](#loadChildDocument-java.lang.String-com.aspose.note.LoadOptions-) | 子ドキュメントノードを追加します。 |
| [loadChildNotebook(String filePath)](#loadChildNotebook-java.lang.String-) | 子ノートブックノードを追加します。 |
| [loadChildNotebook(String filePath, NotebookLoadOptions loadOptions)](#loadChildNotebook-java.lang.String-com.aspose.note.NotebookLoadOptions-) | 子ノートブックノードを追加します。 |
| [removeChild(INotebookChildNode oldChild)](#removeChild-com.aspose.note.INotebookChildNode-) | 子ノードを削除します。 |
| [save(OutputStream stream)](#save-java.io.OutputStream-) | OneNote ドキュメントをストリームに保存します。 |
| [save(OutputStream stream, NotebookSaveOptions options)](#save-java.io.OutputStream-com.aspose.note.NotebookSaveOptions-) | 指定された保存オプションを使用して OneNote ドキュメントをストリームに保存します。 |
| [save(OutputStream stream, int format)](#save-java.io.OutputStream-int-) | 指定された形式で OneNote ドキュメントをストリームに保存します。 |
| [save(String fileName)](#save-java.lang.String-) | OneNote ドキュメントをファイルに保存します。 |
| [save(String fileName, NotebookSaveOptions options)](#save-java.lang.String-com.aspose.note.NotebookSaveOptions-) | 指定された保存オプションを使用して OneNote ドキュメントをファイルに保存します。 |
| [save(String fileName, int format)](#save-java.lang.String-int-) | 指定された形式で OneNote ドキュメントをファイルに保存します。 |
| [setColor(Color value)](#setColor-java.awt.Color-) | 色を取得または設定します。 |
| [setDisplayName(String value)](#setDisplayName-java.lang.String-) | 表示名を取得または設定します。 |
| [setHistoryEnabled(boolean value)](#setHistoryEnabled-boolean-) | 履歴が有効かどうかを示す値を取得または設定します。 |
### Notebook() {#Notebook--}
```
public Notebook()
```


`Notebook` クラスの新しいインスタンスを初期化します。

### Notebook(String filePath) {#Notebook-java.lang.String-}
```
public Notebook(String filePath)
```


`Notebook` クラスの新しいインスタンスを初期化します。ファイルから既存の OneNote ノートブックを開きます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| filePath | java.lang.String | ファイル パスです。 |

### Notebook(String filePath, NotebookLoadOptions loadOptions) {#Notebook-java.lang.String-com.aspose.note.NotebookLoadOptions-}
```
public Notebook(String filePath, NotebookLoadOptions loadOptions)
```


新しい `Notebook` クラスのインスタンスを初期化します。ファイルから既存の OneNote ノートブックを開きます。子ノードの読み込み戦略（"lazy"/instant）などの追加オプションを指定できます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| filePath | java.lang.String | ファイル パスです。 |
| loadOptions | [NotebookLoadOptions](../../com.aspose.note/notebookloadoptions) | ロード オプションです。 |

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
### appendChild(INotebookChildNode newChild) {#appendChild-com.aspose.note.INotebookChildNode-}
```
public INotebookChildNode appendChild(INotebookChildNode newChild)
```


ノードをリストの末尾に追加します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| newChild | [INotebookChildNode](../../com.aspose.note/inotebookchildnode) | 追加するノードです。 |

**Returns:**
[INotebookChildNode](../../com.aspose.note/inotebookchildnode) - The added node.
### getColor() {#getColor--}
```
public Color getColor()
```


色を取得または設定します。

**Returns:**
java.awt.Color
### getCount() {#getCount--}
```
public int getCount()
```


`Notebook` に含まれる要素数を取得します。

**Returns:**
int
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


表示名を取得または設定します。

**Returns:**
java.lang.String
### getFileFormat() {#getFileFormat--}
```
public int getFileFormat()
```


ファイル形式を取得します（OneNote 2010、OneNote Online）。

**Returns:**
int
### getGuid() {#getGuid--}
```
public UUID getGuid()
```


オブジェクトのグローバルに一意な ID を取得します。

値: GUIDです。

**Returns:**
java.util.UUID
### getGuidInternal() {#getGuidInternal--}
```
public System.Guid getGuidInternal()
```




**Returns:**
com.aspose.ms.System.Guid
### get_Item(int index) {#get-Item-int-}
```
public INotebookChildNode get_Item(int index)
```


指定されたインデックスでノートブックの子ノードを取得します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| index | int | 子ノードへのインデックスです。 |

**Returns:**
[INotebookChildNode](../../com.aspose.note/inotebookchildnode) - The child node on the `index` position.
### isHistoryEnabled() {#isHistoryEnabled--}
```
public boolean isHistoryEnabled()
```


履歴が有効かどうかを示す値を取得または設定します。

**Returns:**
boolean
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<INotebookChildNode> iterator()
```


`Notebook` の子ノードを列挙する列挙子を返します。

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.note.INotebookChildNode&gt; - `IEnumerator`。
### loadChildDocument(InputStream stream) {#loadChildDocument-java.io.InputStream-}
```
public void loadChildDocument(InputStream stream)
```


子ドキュメントノードを追加します。ストリームから既存の OneNote ドキュメントを開きます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| ストリーム | java.io.InputStream | ストリームです。 |

### loadChildDocument(InputStream stream, LoadOptions loadOptions) {#loadChildDocument-java.io.InputStream-com.aspose.note.LoadOptions-}
```
public void loadChildDocument(InputStream stream, LoadOptions loadOptions)
```


子ドキュメントノードを追加します。ストリームから既存の OneNote ドキュメントを開きます。追加のロード オプションを指定できます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| ストリーム | java.io.InputStream | ストリームです。 |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | ロード オプションです。 |

### loadChildDocument(String filePath) {#loadChildDocument-java.lang.String-}
```
public void loadChildDocument(String filePath)
```


子ドキュメントノードを追加します。ファイルから既存の OneNote ドキュメントを開きます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| filePath | java.lang.String | ファイル パスです。 |

### loadChildDocument(String filePath, LoadOptions loadOptions) {#loadChildDocument-java.lang.String-com.aspose.note.LoadOptions-}
```
public void loadChildDocument(String filePath, LoadOptions loadOptions)
```


子ドキュメントノードを追加します。ファイルから既存の OneNote ドキュメントを開きます。追加のロード オプションを指定できます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| filePath | java.lang.String | ファイル パスです。 |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | ロード オプションです。 |

### loadChildNotebook(String filePath) {#loadChildNotebook-java.lang.String-}
```
public void loadChildNotebook(String filePath)
```


子ノートブックノードを追加します。ファイルから既存の OneNote ノートブックを開きます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| filePath | java.lang.String | ファイル パスです。 |

### loadChildNotebook(String filePath, NotebookLoadOptions loadOptions) {#loadChildNotebook-java.lang.String-com.aspose.note.NotebookLoadOptions-}
```
public void loadChildNotebook(String filePath, NotebookLoadOptions loadOptions)
```


子ノートブックノードを追加します。ファイルから既存の OneNote ノートブックを開きます。追加のロード オプションを指定できます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| filePath | java.lang.String | ファイル パスです。 |
| loadOptions | [NotebookLoadOptions](../../com.aspose.note/notebookloadoptions) | ロード オプションです。 |

### removeChild(INotebookChildNode oldChild) {#removeChild-com.aspose.note.INotebookChildNode-}
```
public INotebookChildNode removeChild(INotebookChildNode oldChild)
```


子ノードを削除します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| oldChild | [INotebookChildNode](../../com.aspose.note/inotebookchildnode) | 削除するノードです。 |

**Returns:**
[INotebookChildNode](../../com.aspose.note/inotebookchildnode) - The removed node.
### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public void save(OutputStream stream)
```


OneNote ドキュメントをストリームに保存します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| ストリーム | java.io.OutputStream | ストリームです。 |

### save(OutputStream stream, NotebookSaveOptions options) {#save-java.io.OutputStream-com.aspose.note.NotebookSaveOptions-}
```
public void save(OutputStream stream, NotebookSaveOptions options)
```


指定された保存オプションを使用して OneNote ドキュメントをストリームに保存します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| ストリーム | java.io.OutputStream | ストリームです。 |
| options | [NotebookSaveOptions](../../com.aspose.note/notebooksaveoptions) | ドキュメントの保存方法に関するオプションを指定します。 |

### save(OutputStream stream, int format) {#save-java.io.OutputStream-int-}
```
public void save(OutputStream stream, int format)
```


指定された形式で OneNote ドキュメントをストリームに保存します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| ストリーム | java.io.OutputStream | ストリームです。 |
| format | int | ドキュメントを保存する形式です。 |

### save(String fileName) {#save-java.lang.String-}
```
public void save(String fileName)
```


OneNote ドキュメントをファイルに保存します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| ファイル名 | java.lang.String | ファイルのフルネーム。指定されたフルネームのファイルが既に存在する場合、既存のファイルが上書きされます。 |

### save(String fileName, NotebookSaveOptions options) {#save-java.lang.String-com.aspose.note.NotebookSaveOptions-}
```
public void save(String fileName, NotebookSaveOptions options)
```


指定された保存オプションを使用して OneNote ドキュメントをファイルに保存します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| ファイル名 | java.lang.String | ファイルのフルネーム。指定されたフルネームのファイルが既に存在する場合、既存のファイルが上書きされます。 |
| options | [NotebookSaveOptions](../../com.aspose.note/notebooksaveoptions) | ドキュメントがファイルに保存される方法のオプションを指定します。 |

### save(String fileName, int format) {#save-java.lang.String-int-}
```
public void save(String fileName, int format)
```


指定された形式で OneNote ドキュメントをファイルに保存します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| ファイル名 | java.lang.String | ファイルのフルネーム。指定されたフルネームのファイルが既に存在する場合、既存のファイルが上書きされます。 |
| format | int | ドキュメントを保存する形式です。 |

### setColor(Color value) {#setColor-java.awt.Color-}
```
public void setColor(Color value)
```


色を取得または設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.awt.Color |  |

### setDisplayName(String value) {#setDisplayName-java.lang.String-}
```
public void setDisplayName(String value)
```


表示名を取得または設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String |  |

### setHistoryEnabled(boolean value) {#setHistoryEnabled-boolean-}
```
public void setHistoryEnabled(boolean value)
```


履歴が有効かどうかを示す値を取得または設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean |  |

