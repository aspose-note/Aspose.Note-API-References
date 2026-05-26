---
title: "NotebookLoadOptions"
second_title: "Aspose.Note for Java API リファレンス"
description: "ノートブックの読み込みに使用されるオプションです。"
type: docs
weight: 58
url: /ja/java/com.aspose.note/notebookloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class NotebookLoadOptions
```

ノートブックの読み込みに使用されるオプションです。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [NotebookLoadOptions()](#NotebookLoadOptions--) | 新しい `NotebookLoadOptions` クラスのインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getDeferredLoading()](#getDeferredLoading--) | 子ドキュメントを後で明示的にロードするかどうかを示す値を取得または設定します。 |
| [getInstantLoading()](#getInstantLoading--) | 親ドキュメントのロード中に子ドキュメントをロードするかどうかを示す値を取得または設定します。 |
| [setDeferredLoading(boolean value)](#setDeferredLoading-boolean-) | 子ドキュメントを後で明示的にロードするかどうかを示す値を取得または設定します。 |
| [setInstantLoading(boolean value)](#setInstantLoading-boolean-) | 親ドキュメントのロード中に子ドキュメントをロードするかどうかを示す値を取得または設定します。 |
### NotebookLoadOptions() {#NotebookLoadOptions--}
```
public NotebookLoadOptions()
```


新しい `NotebookLoadOptions` クラスのインスタンスを初期化します。

### getDeferredLoading() {#getDeferredLoading--}
```
public final boolean getDeferredLoading()
```


子ドキュメントを後で明示的にロードするかどうかを示す値を取得または設定します。

--------------------

デフォルト値は `false` です。そのため子ドキュメントは暗黙的にロードされます。値が `true` の場合、ユーザーは `Notebook.loadChildDocument` を呼び出すか、ノートブック自体がロードされた後に各ノートブックの子ノードを呼び出す必要があります。値が `true` の場合、`NotebookLoadOptions.instantLoading` オプションは無視されます。ノートブックがストリームからロードされる場合、ユーザーが `false` に明示的に設定していても、値は常に `true` です。

**Returns:**
boolean
### getInstantLoading() {#getInstantLoading--}
```
public boolean getInstantLoading()
```


親ドキュメントのロード中に子ドキュメントをロードするかどうかを示す値を取得または設定します。

--------------------

デフォルト値は `false` です。そのため子ドキュメントは「遅延」ロードされ、つまり特定の子への直接アクセスが行われるまでロードが延期されます。値が `true` の場合、ロードは即座に実行されることを示します。

**Returns:**
boolean
### setDeferredLoading(boolean value) {#setDeferredLoading-boolean-}
```
public final void setDeferredLoading(boolean value)
```


子ドキュメントを後で明示的にロードするかどうかを示す値を取得または設定します。

--------------------

デフォルト値は `false` です。そのため子ドキュメントは暗黙的にロードされます。値が `true` の場合、ユーザーは `Notebook.loadChildDocument` を呼び出すか、ノートブック自体がロードされた後に各ノートブックの子ノードを呼び出す必要があります。値が `true` の場合、`NotebookLoadOptions.instantLoading` オプションは無視されます。ノートブックがストリームからロードされる場合、ユーザーが `false` に明示的に設定していても、値は常に `true` です。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean |  |

### setInstantLoading(boolean value) {#setInstantLoading-boolean-}
```
public void setInstantLoading(boolean value)
```


親ドキュメントのロード中に子ドキュメントをロードするかどうかを示す値を取得または設定します。

--------------------

デフォルト値は `false` です。そのため子ドキュメントは「遅延」ロードされ、つまり特定の子への直接アクセスが行われるまでロードが延期されます。値が `true` の場合、ロードは即座に実行されることを示します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean |  |

