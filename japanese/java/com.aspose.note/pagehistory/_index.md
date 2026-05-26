---
title: "PageHistory"
second_title: "Aspose.Note for Java API リファレンス"
description: "ページ履歴を表します。"
type: docs
weight: 70
url: /ja/java/com.aspose.note/pagehistory/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.ms.System.Collections.Generic.IGenericList
```
public class PageHistory implements System.Collections.Generic.IGenericList<Page>
```

ページ履歴を表します。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [PageHistory(Page page)](#PageHistory-com.aspose.note.Page-) | `PageHistory` クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [addItem(Page item)](#addItem-com.aspose.note.Page-) | `PageHistory` の末尾にページバージョンを追加します。 |
| [addRange(System.Collections.Generic.IGenericEnumerable&lt;Page&gt; items)](#addRange-com.aspose.ms.System.Collections.Generic.IGenericEnumerable-com.aspose.note.Page--) | `PageHistory` の末尾にページバージョンを追加します。 |
| [clear()](#clear--) | ページ履歴をクリアします。 |
| [containsItem(Page item)](#containsItem-com.aspose.note.Page-) | ページ履歴にページバージョンが含まれているかどうかを判断します。 |
| [copyToTArray(Page[] array, int arrayIndex)](#copyToTArray-com.aspose.note.Page---int-) | ページ バージョンを配列にコピーし、特定のインデックスから開始します.. |
| [getCurrent()](#getCurrent--) | 現在のページ バージョンを取得します。 |
| [get_Item(int index)](#get-Item-int-) | 指定されたインデックスの `PageHistory` のページ バージョンを取得または設定します。 |
| [indexOfItem(Page item)](#indexOfItem-com.aspose.note.Page-) | ページ履歴内の特定のページ バージョンのインデックスを決定します。 |
| [insertItem(int index, Page item)](#insertItem-int-com.aspose.note.Page-) | ページ履歴にページ バージョンを挿入します。 |
| [isReadOnly()](#isReadOnly--) | ページ履歴が読み取り専用かどうかを示す値を取得します。 |
| [iterator()](#iterator--) | `PageHistory` の子ノードを列挙する列挙子を返します。 |
| [removeAt(int index)](#removeAt-int-) | `PageHistory` の指定インデックスにあるページ バージョンを削除します。 |
| [removeItem(Page item)](#removeItem-com.aspose.note.Page-) | `PageHistory` からページ バージョンを削除します。 |
| [removeRange(int index, int count)](#removeRange-int-int-) | `PageHistory` からページ バージョンの範囲を削除します。 |
| [set_Item(int index, Page value)](#set-Item-int-com.aspose.note.Page-) | 指定されたインデックスの `PageHistory` のページ バージョンを取得または設定します。 |
| [size()](#size--) | ページ履歴内のページ バージョンの数を取得します。 |
### PageHistory(Page page) {#PageHistory-com.aspose.note.Page-}
```
public PageHistory(Page page)
```


`PageHistory` クラスの新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | 現在のページ バージョン。 |

### addItem(Page item) {#addItem-com.aspose.note.Page-}
```
public void addItem(Page item)
```


`PageHistory` の末尾にページバージョンを追加します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | ページ バージョン。 |

### addRange(System.Collections.Generic.IGenericEnumerable&lt;Page&gt; items) {#addRange-com.aspose.ms.System.Collections.Generic.IGenericEnumerable-com.aspose.note.Page--}
```
public void addRange(System.Collections.Generic.IGenericEnumerable<Page> items)
```


`PageHistory` の末尾にページバージョンを追加します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 項目 | com.aspose.ms.System.Collections.Generic.IGenericEnumerable&lt;com.aspose.note.Page&gt; | ページ バージョンの `IEnumerable\{Page\}` コレクションです。 |

### clear() {#clear--}
```
public void clear()
```


ページ履歴をクリアします。

### containsItem(Page item) {#containsItem-com.aspose.note.Page-}
```
public boolean containsItem(Page item)
```


ページ履歴にページバージョンが含まれているかどうかを判断します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | ページ バージョン。 |

**Returns:**
boolean - `bool`です。
### copyToTArray(Page[] array, int arrayIndex) {#copyToTArray-com.aspose.note.Page---int-}
```
public void copyToTArray(Page[] array, int arrayIndex)
```


ページ バージョンを配列にコピーし、特定のインデックスから開始します..

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| array | [Page\[\]](../../com.aspose.note/page) | 対象の配列です。 |
| arrayIndex | int | 配列インデックスです。 |

### getCurrent() {#getCurrent--}
```
public Page getCurrent()
```


現在のページ バージョンを取得します。

**Returns:**
[Page](../../com.aspose.note/page)
### get_Item(int index) {#get-Item-int-}
```
public Page get_Item(int index)
```


指定されたインデックスの `PageHistory` のページ バージョンを取得または設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| index | int | インデックスです。 |

**Returns:**
[Page](../../com.aspose.note/page) - The page version.
### indexOfItem(Page item) {#indexOfItem-com.aspose.note.Page-}
```
public int indexOfItem(Page item)
```


ページ履歴内の特定のページ バージョンのインデックスを決定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | ページ バージョン。 |

**Returns:**
int - `int`です。
### insertItem(int index, Page item) {#insertItem-int-com.aspose.note.Page-}
```
public void insertItem(int index, Page item)
```


ページ履歴にページ バージョンを挿入します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| index | int | インデックスです。 |
| item | [Page](../../com.aspose.note/page) | ページ バージョン。 |

### isReadOnly() {#isReadOnly--}
```
public boolean isReadOnly()
```


ページ履歴が読み取り専用かどうかを示す値を取得します。

**Returns:**
boolean
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<Page> iterator()
```


`PageHistory` の子ノードを列挙する列挙子を返します。

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.note.Page&gt; - `IEnumerator`。
### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


`PageHistory` の指定インデックスにあるページ バージョンを削除します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| index | int | インデックスです。 |

### removeItem(Page item) {#removeItem-com.aspose.note.Page-}
```
public boolean removeItem(Page item)
```


`PageHistory` からページ バージョンを削除します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | ページ バージョン。 |

**Returns:**
boolean - `bool`です。
### removeRange(int index, int count) {#removeRange-int-int-}
```
public void removeRange(int index, int count)
```


`PageHistory` からページ バージョンの範囲を削除します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| index | int | インデックスです。 |
| count | int | カウントです。 |

### set_Item(int index, Page value) {#set-Item-int-com.aspose.note.Page-}
```
public void set_Item(int index, Page value)
```


指定されたインデックスの `PageHistory` のページ バージョンを取得または設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| index | int | インデックスです。 |
| value | [Page](../../com.aspose.note/page) |  |

### size() {#size--}
```
public int size()
```


ページ履歴内のページ バージョンの数を取得します。

**Returns:**
int
