---
title: "Document"
second_title: "Aspose.Note for Java API リファレンス"
description: "Aspose.Note ドキュメントを表します。"
type: docs
weight: 20
url: /ja/java/com.aspose.note/document/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode

**All Implemented Interfaces:**
[com.aspose.note.INotebookChildNode](../../com.aspose.note/inotebookchildnode)
```
public class Document extends CompositeNode<Page> implements INotebookChildNode
```

Aspose.Note ドキュメントを表します。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [Document()](#Document--) | `Document` クラスの新しいインスタンスを初期化します。 |
| [Document(String filePath)](#Document-java.lang.String-) | `Document` クラスの新しいインスタンスを初期化します。 |
| [Document(String filePath, LoadOptions loadOptions)](#Document-java.lang.String-com.aspose.note.LoadOptions-) | `Document` クラスの新しいインスタンスを初期化します。 |
| [Document(InputStream inStream)](#Document-java.io.InputStream-) | `Document` クラスの新しいインスタンスを初期化します。 |
| [Document(InputStream inStream, LoadOptions loadOptions)](#Document-java.io.InputStream-com.aspose.note.LoadOptions-) | `Document` クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | ノードのビジターを受け入れます。 |
| [detectLayoutChanges()](#detectLayoutChanges--) | 前回の `DetectLayoutChanges` 呼び出し以降にドキュメントレイアウトに加えられたすべての変更を検出します。 |
| [getAutomaticLayoutChangesDetectionEnabled()](#getAutomaticLayoutChangesDetectionEnabled--) | Aspose.Note がレイアウト変更の検出を自動的に行うかどうかを示す値を取得します。 |
| [getColor()](#getColor--) | 色を取得します。 |
| [getCreationTime()](#getCreationTime--) | 作成時刻を取得します。 |
| [getDisplayName()](#getDisplayName--) | 表示名を取得します。 |
| [getFileFormat()](#getFileFormat--) | ファイル形式を取得します（OneNote 2010、OneNote Online）。 |
| [getGuid()](#getGuid--) | オブジェクトのグローバルに一意な ID を取得します。 |
| [getGuidInternal()](#getGuidInternal--) |  |
| [getPageHistory(Page page)](#getPageHistory-com.aspose.note.Page-) | ドキュメントに表示される各ページの完全な履歴を含む `PageHistory` を取得します（最も古いものがインデックス 0）。 |
| [isEncrypted(InputStream stream, Document[] document)](#isEncrypted-java.io.InputStream-com.aspose.note.Document---) | ストリームからのドキュメントが暗号化されているかどうかをチェックします。 |
| [isEncrypted(InputStream stream, LoadOptions options, Document[] document)](#isEncrypted-java.io.InputStream-com.aspose.note.LoadOptions-com.aspose.note.Document---) | ストリームからのドキュメントが暗号化されているかどうかをチェックします。 |
| [isEncrypted(InputStream stream, String password, Document[] document)](#isEncrypted-java.io.InputStream-java.lang.String-com.aspose.note.Document---) | ストリームからのドキュメントが暗号化されているかどうかをチェックします。 |
| [isEncrypted(String filePath, Document[] document)](#isEncrypted-java.lang.String-com.aspose.note.Document---) | ファイルからのドキュメントが暗号化されているかどうかをチェックします。 |
| [isEncrypted(String filePath, LoadOptions options, Document[] document)](#isEncrypted-java.lang.String-com.aspose.note.LoadOptions-com.aspose.note.Document---) | ファイルからのドキュメントが暗号化されているかどうかをチェックします。 |
| [isEncrypted(String filePath, String password, Document[] document)](#isEncrypted-java.lang.String-java.lang.String-com.aspose.note.Document---) | ファイルからのドキュメントが暗号化されているかどうかをチェックします。 |
| [print()](#print--) | デフォルトのプリンターを使用してドキュメントを印刷します。 |
| [print(PrintOptions options)](#print-com.aspose.note.PrintOptions-) | デフォルトのプリンターを使用してドキュメントを印刷します。 |
| [print(String printerName)](#print-java.lang.String-) | デフォルトのプリンターを使用してドキュメントを印刷します。 |
| [print(AttributeSet printSettings)](#print-javax.print.attribute.AttributeSet-) | デフォルトのプリンターを使用してドキュメントを印刷します。 |
| [save(OutputStream stream)](#save-java.io.OutputStream-) | OneNote ドキュメントをストリームに保存します。 |
| [save(OutputStream stream, SaveOptions options)](#save-java.io.OutputStream-com.aspose.note.SaveOptions-) | 指定された保存オプションを使用して OneNote ドキュメントをストリームに保存します。 |
| [save(OutputStream stream, int format)](#save-java.io.OutputStream-int-) | 指定された形式で OneNote ドキュメントをストリームに保存します。 |
| [save(String fileName)](#save-java.lang.String-) | OneNote ドキュメントをファイルに保存します。 |
| [save(String fileName, SaveOptions options)](#save-java.lang.String-com.aspose.note.SaveOptions-) | 指定された保存オプションを使用して OneNote ドキュメントをファイルに保存します。 |
| [save(String fileName, int format)](#save-java.lang.String-int-) | 指定された形式で OneNote ドキュメントをファイルに保存します。 |
| [setAutomaticLayoutChangesDetectionEnabled(boolean value)](#setAutomaticLayoutChangesDetectionEnabled-boolean-) | Aspose.Note がレイアウト変更の検出を自動的に行うかどうかを示す値を設定します。 |
| [setColor(Color value)](#setColor-java.awt.Color-) | 色を設定します。 |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | 作成時刻を設定します。 |
| [setDisplayName(String value)](#setDisplayName-java.lang.String-) | 表示名を設定します。 |
### Document() {#Document--}
```
public Document()
```


`Document` クラスの新しいインスタンスを初期化します。空白の OneNote ドキュメントを作成します。

### Document(String filePath) {#Document-java.lang.String-}
```
public Document(String filePath)
```


`Document` クラスの新しいインスタンスを初期化します。ファイルから既存の OneNote ドキュメントを開きます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| filePath | java.lang.String | ファイル パスです。 |

### Document(String filePath, LoadOptions loadOptions) {#Document-java.lang.String-com.aspose.note.LoadOptions-}
```
public Document(String filePath, LoadOptions loadOptions)
```


`Document` クラスの新しいインスタンスを初期化します。ファイルから既存の OneNote ドキュメントを開きます。暗号化パスワードなどの追加オプションを指定できます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| filePath | java.lang.String | ファイル パスです。 |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | ドキュメントのロードに使用されるオプションです。null にすることも可能です。 |

### Document(InputStream inStream) {#Document-java.io.InputStream-}
```
public Document(InputStream inStream)
```


`Document` クラスの新しいインスタンスを初期化します。ストリームから既存の OneNote ドキュメントを開きます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| inStream | java.io.InputStream | ストリームです。 |

### Document(InputStream inStream, LoadOptions loadOptions) {#Document-java.io.InputStream-com.aspose.note.LoadOptions-}
```
public Document(InputStream inStream, LoadOptions loadOptions)
```


`Document` クラスの新しいインスタンスを初期化します。ストリームから既存の OneNote ドキュメントを開きます。暗号化パスワードなどの追加オプションを指定できます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| inStream | java.io.InputStream | ストリームです。 |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | ドキュメントのロードに使用されるオプションです。null にすることも可能です。 |

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


ノードのビジターを受け入れます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | `DocumentVisitor` から派生したクラスのオブジェクト。 |

### detectLayoutChanges() {#detectLayoutChanges--}
```
public void detectLayoutChanges()
```


前回の `DetectLayoutChanges` 呼び出し以降にドキュメントのレイアウトに加えられたすべての変更を検出します。`AutomaticLayoutChangesDetectionEnabled` が true に設定されている場合、ドキュメントのエクスポート開始時に自動的に使用されます。

### getAutomaticLayoutChangesDetectionEnabled() {#getAutomaticLayoutChangesDetectionEnabled--}
```
public boolean getAutomaticLayoutChangesDetectionEnabled()
```


Aspose.Note がレイアウト変更の検出を自動的に行うかどうかを示す値を取得します。デフォルト値は `true` です。

**Returns:**
boolean
### getColor() {#getColor--}
```
public Color getColor()
```


色を取得します。

**Returns:**
java.awt.Color
### getCreationTime() {#getCreationTime--}
```
public Date getCreationTime()
```


作成時刻を取得します。

**Returns:**
java.util.Date
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


表示名を取得します。

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

**Returns:**
java.util.UUID
### getGuidInternal() {#getGuidInternal--}
```
public System.Guid getGuidInternal()
```




**Returns:**
com.aspose.ms.System.Guid
### getPageHistory(Page page) {#getPageHistory-com.aspose.note.Page-}
```
public PageHistory getPageHistory(Page page)
```


ドキュメントに表示される各ページの完全な履歴を含む `PageHistory` を取得します（最も古いものがインデックス 0）。現在のページリビジョンは `PageHistory.current` としてアクセスでき、履歴バージョンのコレクションとは別に保持されます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | ページの現在のリビジョンです。 |

**Returns:**
[PageHistory](../../com.aspose.note/pagehistory) - The `PageHistory`.
### isEncrypted(InputStream stream, Document[] document) {#isEncrypted-java.io.InputStream-com.aspose.note.Document---}
```
public static boolean isEncrypted(InputStream stream, Document[] document)
```


ストリームからのドキュメントが暗号化されているかどうかをチェックします。チェックするにはドキュメントを完全にロードする必要があるため、このメソッドはパフォーマンスに影響を与える可能性があります。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| ストリーム | java.io.InputStream | ストリームです。 |
| document | [Document\[\]](../../com.aspose.note/document) | ロードされたドキュメントです。 |

**Returns:**
boolean - ドキュメントが暗号化されている場合は true、そうでない場合は false を返します。
### isEncrypted(InputStream stream, LoadOptions options, Document[] document) {#isEncrypted-java.io.InputStream-com.aspose.note.LoadOptions-com.aspose.note.Document---}
```
public static boolean isEncrypted(InputStream stream, LoadOptions options, Document[] document)
```


ストリームからのドキュメントが暗号化されているかどうかをチェックします。チェックするにはドキュメントを完全にロードする必要があるため、このメソッドはパフォーマンスに影響を与える可能性があります。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| ストリーム | java.io.InputStream | ストリームです。 |
| options | [LoadOptions](../../com.aspose.note/loadoptions) | ロード オプションです。 |
| document | [Document\[\]](../../com.aspose.note/document) | ロードされたドキュメントです。 |

**Returns:**
boolean - ドキュメントが暗号化されている場合は true、そうでない場合は false を返します。
### isEncrypted(InputStream stream, String password, Document[] document) {#isEncrypted-java.io.InputStream-java.lang.String-com.aspose.note.Document---}
```
public static boolean isEncrypted(InputStream stream, String password, Document[] document)
```


ストリームからのドキュメントが暗号化されているかどうかをチェックします。チェックするにはドキュメントを完全にロードする必要があるため、このメソッドはパフォーマンスに影響を与える可能性があります。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| ストリーム | java.io.InputStream | ストリームです。 |
| password | java.lang.String | ドキュメントを復号化するためのパスワードです。 |
| document | [Document\[\]](../../com.aspose.note/document) | ロードされたドキュメントです。 |

**Returns:**
boolean - ドキュメントが暗号化されている場合は true、そうでない場合は false を返します。
### isEncrypted(String filePath, Document[] document) {#isEncrypted-java.lang.String-com.aspose.note.Document---}
```
public static boolean isEncrypted(String filePath, Document[] document)
```


ファイルからのドキュメントが暗号化されているかどうかをチェックします。チェックするにはドキュメントを完全にロードする必要があるため、このメソッドはパフォーマンスに影響を与える可能性があります。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| filePath | java.lang.String | ファイル パスです。 |
| document | [Document\[\]](../../com.aspose.note/document) | ロードされたドキュメントです。 |

**Returns:**
boolean - ドキュメントが暗号化されている場合は true、そうでない場合は false を返します。
### isEncrypted(String filePath, LoadOptions options, Document[] document) {#isEncrypted-java.lang.String-com.aspose.note.LoadOptions-com.aspose.note.Document---}
```
public static boolean isEncrypted(String filePath, LoadOptions options, Document[] document)
```


ファイルからのドキュメントが暗号化されているかどうかをチェックします。チェックするにはドキュメントを完全にロードする必要があるため、このメソッドはパフォーマンスに影響を与える可能性があります。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| filePath | java.lang.String | ファイル パスです。 |
| options | [LoadOptions](../../com.aspose.note/loadoptions) | ロード オプションです。 |
| document | [Document\[\]](../../com.aspose.note/document) | ロードされたドキュメントです。 |

**Returns:**
boolean - ドキュメントが暗号化されている場合は true、そうでない場合は false を返します。
### isEncrypted(String filePath, String password, Document[] document) {#isEncrypted-java.lang.String-java.lang.String-com.aspose.note.Document---}
```
public static boolean isEncrypted(String filePath, String password, Document[] document)
```


ファイルからのドキュメントが暗号化されているかどうかをチェックします。チェックするにはドキュメントを完全にロードする必要があるため、このメソッドはパフォーマンスに影響を与える可能性があります。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| filePath | java.lang.String | ファイル パスです。 |
| password | java.lang.String | ドキュメントを復号化するためのパスワードです。 |
| document | [Document\[\]](../../com.aspose.note/document) | ロードされたドキュメントです。 |

**Returns:**
boolean - ドキュメントが暗号化されている場合は true、そうでない場合は false を返します。
### print() {#print--}
```
public void print()
```


デフォルトのプリンターを使用してドキュメントを印刷します。

### print(PrintOptions options) {#print-com.aspose.note.PrintOptions-}
```
public void print(PrintOptions options)
```


デフォルトのプリンターを使用してドキュメントを印刷します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| options | [PrintOptions](../../com.aspose.note/printoptions) | ドキュメントを印刷するために使用されるオプションです。null にすることができます。 |

### print(String printerName) {#print-java.lang.String-}
```
public void print(String printerName)
```


デフォルトのプリンターを使用してドキュメントを印刷します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| printerName | java.lang.String |  |

### print(AttributeSet printSettings) {#print-javax.print.attribute.AttributeSet-}
```
public void print(AttributeSet printSettings)
```


デフォルトのプリンターを使用してドキュメントを印刷します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| printSettings | javax.print.attribute.AttributeSet |  |

### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public void save(OutputStream stream)
```


OneNote ドキュメントをストリームに保存します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| ストリーム | java.io.OutputStream | ドキュメントが保存される System.iO.stream です。 |

### save(OutputStream stream, SaveOptions options) {#save-java.io.OutputStream-com.aspose.note.SaveOptions-}
```
public void save(OutputStream stream, SaveOptions options)
```


指定された保存オプションを使用して OneNote ドキュメントをストリームに保存します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| ストリーム | java.io.OutputStream | ドキュメントが保存される System.iO.stream です。 |
| options | [SaveOptions](../../com.aspose.note/saveoptions) | ストリームにドキュメントが保存される方法のオプションを指定します。 |

### save(OutputStream stream, int format) {#save-java.io.OutputStream-int-}
```
public void save(OutputStream stream, int format)
```


指定された形式で OneNote ドキュメントをストリームに保存します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| ストリーム | java.io.OutputStream | ドキュメントが保存される System.iO.stream です。 |
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

### save(String fileName, SaveOptions options) {#save-java.lang.String-com.aspose.note.SaveOptions-}
```
public void save(String fileName, SaveOptions options)
```


指定された保存オプションを使用して OneNote ドキュメントをファイルに保存します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| ファイル名 | java.lang.String | ファイルのフルネーム。指定されたフルネームのファイルが既に存在する場合、既存のファイルが上書きされます。 |
| options | [SaveOptions](../../com.aspose.note/saveoptions) | ドキュメントがファイルに保存される方法のオプションを指定します。 |

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

### setAutomaticLayoutChangesDetectionEnabled(boolean value) {#setAutomaticLayoutChangesDetectionEnabled-boolean-}
```
public void setAutomaticLayoutChangesDetectionEnabled(boolean value)
```


Aspose.Note がレイアウト変更の検出を自動的に行うかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | 新しい値です。null にすることができます。 |

### setColor(Color value) {#setColor-java.awt.Color-}
```
public void setColor(Color value)
```


色を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.awt.Color | Color の値です。 |

### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public void setCreationTime(Date value)
```


作成時刻を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.util.Date | DateTime の値です。 |

### setDisplayName(String value) {#setDisplayName-java.lang.String-}
```
public void setDisplayName(String value)
```


表示名を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String | DateTime の値です。 |

