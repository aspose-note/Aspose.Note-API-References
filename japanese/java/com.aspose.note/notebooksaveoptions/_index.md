---
title: "NotebookSaveOptions"
second_title: "Aspose.Note for Java API リファレンス"
description: "特定の形式向けのノートブック保存オプションを表す抽象基底クラスです。"
type: docs
weight: 61
url: /ja/java/com.aspose.note/notebooksaveoptions/
---

**Inheritance:**
java.lang.Object
```
public abstract class NotebookSaveOptions
```

特定の形式向けのノートブック保存オプションを表す抽象基底クラスです。
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getDeferredSaving()](#getDeferredSaving--) | 子ドキュメントを明示的に保存すべきかどうかを示す値を取得または設定します。 |
| [getDocumentSaveOptionsInternal()](#getDocumentSaveOptionsInternal--) | ノートブックのすべての子ドキュメントの保存オプションを取得します。 |
| [getFlatten()](#getFlatten--) | ノートブックの子階層がフラットに保存されるかどうかを示す値を取得または設定します。 |
| [getSaveFormat()](#getSaveFormat--) | ノートブックが保存される形式を取得します。 |
| [setDeferredSaving(boolean value)](#setDeferredSaving-boolean-) | 子ドキュメントを明示的に保存すべきかどうかを示す値を取得または設定します。 |
| [setFlatten(boolean value)](#setFlatten-boolean-) | ノートブックの子階層がフラットに保存されるかどうかを示す値を取得または設定します。 |
### getDeferredSaving() {#getDeferredSaving--}
```
public boolean getDeferredSaving()
```


子ドキュメントを明示的に保存すべきかどうかを示す値を取得または設定します。

--------------------

デフォルト値は `false` です。そのため子ドキュメントは暗黙的に保存されます。値が `true` の場合、ユーザーは各ノートブックの子ノードを明示的に保存すべきことを示します。ノートブックがストリームに保存される場合、ユーザーが `false` に明示的に設定したかどうかに関わらず、値は常に `true` になります。

**Returns:**
boolean
### getDocumentSaveOptionsInternal() {#getDocumentSaveOptionsInternal--}
```
public abstract SaveOptions getDocumentSaveOptionsInternal()
```


ノートブックのすべての子ドキュメントの保存オプションを取得します。

**Returns:**
[SaveOptions](../../com.aspose.note/saveoptions) - The `SaveOptions`.
### getFlatten() {#getFlatten--}
```
public boolean getFlatten()
```


ノートブックの子階層がフラットに保存されるかどうかを示す値を取得または設定します。

**Returns:**
boolean
### getSaveFormat() {#getSaveFormat--}
```
public abstract int getSaveFormat()
```


ノートブックが保存される形式を取得します。

**Returns:**
int
### setDeferredSaving(boolean value) {#setDeferredSaving-boolean-}
```
public void setDeferredSaving(boolean value)
```


子ドキュメントを明示的に保存すべきかどうかを示す値を取得または設定します。

--------------------

デフォルト値は `false` です。そのため子ドキュメントは暗黙的に保存されます。値が `true` の場合、ユーザーは各ノートブックの子ノードを明示的に保存すべきことを示します。ノートブックがストリームに保存される場合、ユーザーが `false` に明示的に設定したかどうかに関わらず、値は常に `true` になります。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean |  |

### setFlatten(boolean value) {#setFlatten-boolean-}
```
public void setFlatten(boolean value)
```


ノートブックの子階層がフラットに保存されるかどうかを示す値を取得または設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean |  |

