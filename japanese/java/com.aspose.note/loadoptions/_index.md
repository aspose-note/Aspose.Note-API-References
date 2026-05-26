---
title: "LoadOptions"
second_title: "Aspose.Note for Java API リファレンス"
description: "ドキュメントの読み込みに使用されるオプションです。"
type: docs
weight: 46
url: /ja/java/com.aspose.note/loadoptions/
---

**Inheritance:**
java.lang.Object
```
public class LoadOptions
```

ドキュメントの読み込みに使用されるオプションです。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [LoadOptions()](#LoadOptions--) | `LoadOptions` クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getDocumentPassword()](#getDocumentPassword--) | 暗号化されたドキュメントコンテンツのパスワードを取得または設定します。 |
| [getLoadHistory()](#getLoadHistory--) | ドキュメントローダーが履歴を無視すべきかどうかを示す値を取得または設定します。 |
| [setDocumentPassword(String value)](#setDocumentPassword-java.lang.String-) | 暗号化されたドキュメントコンテンツのパスワードを取得または設定します。 |
| [setLoadHistory(boolean value)](#setLoadHistory-boolean-) | ドキュメントローダーが履歴を無視すべきかどうかを示す値を取得または設定します。 |
### LoadOptions() {#LoadOptions--}
```
public LoadOptions()
```


`LoadOptions` クラスの新しいインスタンスを初期化します。

### getDocumentPassword() {#getDocumentPassword--}
```
public String getDocumentPassword()
```


暗号化されたドキュメントコンテンツのパスワードを取得または設定します。ドキュメントがパスワードで保護されていない場合、この値は無視されます。

**Returns:**
java.lang.String
### getLoadHistory() {#getLoadHistory--}
```
public boolean getLoadHistory()
```


ドキュメントローダーが履歴を無視すべきかどうかを示す値を取得または設定します。このオプションを使用するとメモリと CPU の使用量を減らすことができます。デフォルト値は `true` です。

**Returns:**
boolean
### setDocumentPassword(String value) {#setDocumentPassword-java.lang.String-}
```
public void setDocumentPassword(String value)
```


暗号化されたドキュメントコンテンツのパスワードを取得または設定します。ドキュメントがパスワードで保護されていない場合、この値は無視されます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String |  |

### setLoadHistory(boolean value) {#setLoadHistory-boolean-}
```
public void setLoadHistory(boolean value)
```


ドキュメントローダーが履歴を無視すべきかどうかを示す値を取得または設定します。このオプションを使用するとメモリと CPU の使用量を減らすことができます。デフォルト値は `true` です。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean |  |

