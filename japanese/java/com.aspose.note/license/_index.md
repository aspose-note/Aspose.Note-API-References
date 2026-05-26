---
title: "License"
second_title: "Aspose.Note for Java API リファレンス"
description: "コンポーネントをライセンスするためのメソッドを提供します。"
type: docs
weight: 44
url: /ja/java/com.aspose.note/license/
---

**Inheritance:**
java.lang.Object
```
public class License
```

コンポーネントをライセンスするためのメソッドを提供します。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [License()](#License--) | このクラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [resetThreadContext()](#resetThreadContext--) | 現在のスレッドのライセンス コンテキストをリセットします。 |
| [setLicense(File licenseFile)](#setLicense-java.io.File-) | コンポーネントにライセンスを付与します。 |
| [setLicense(InputStream stream)](#setLicense-java.io.InputStream-) | コンポーネントにライセンスを付与します。 |
| [setLicense(String licenseName)](#setLicense-java.lang.String-) | コンポーネントにライセンスを付与します。 |
| [setThreadContext(InputStream stream)](#setThreadContext-java.io.InputStream-) | 現在のスレッドのライセンス コンテキストを設定します。 |
### License() {#License--}
```
public License()
```


このクラスの新しいインスタンスを初期化します。

### resetThreadContext() {#resetThreadContext--}
```
public static void resetThreadContext()
```


現在のスレッドのライセンス コンテキストをリセットします。

### setLicense(File licenseFile) {#setLicense-java.io.File-}
```
public void setLicense(File licenseFile)
```


コンポーネントにライセンスを付与します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| licenseFile | java.io.File | ライセンスのファイル`System.IO.FileInfo`。 |

### setLicense(InputStream stream) {#setLicense-java.io.InputStream-}
```
public final void setLicense(InputStream stream)
```


コンポーネントにライセンスを付与します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
|  | ストリーム | java.io.InputStream | ライセンスを含むストリームです。 |

--------------------

`

このメソッドを使用して、ストリームからライセンスをロードします。

`

`void setLicense(java.io.InputStream stream)` |

### setLicense(String licenseName) {#setLicense-java.lang.String-}
```
public final void setLicense(String licenseName)
```


コンポーネントにライセンスを付与します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
|  | licenseName | java.lang.String | 完全または短いファイル名`または埋め込みリソースの名前`にすることができます。空文字列を使用すると評価モードに切り替わります。 |

--------------------

`

次の場所でライセンスを検索します:

` `

1. 明示的なパス。

` `

2. Aspose コンポーネント アセンブリを含むフォルダー。

3. クライアントの呼び出しアセンブリを含むフォルダー。

4. エントリ（スタートアップ）アセンブリを含むフォルダー。

5. クライアントの呼び出しアセンブリ内の埋め込みリソース。

**Note:**On the .NET Compact Framework, tries to find the license only in these locations:

1. 明示的なパス。

2. クライアントの呼び出しアセンブリ内の埋め込みリソース。

` `

2. Aspose コンポーネント JAR ファイルを含むフォルダー。

3. クライアントの呼び出し JAR ファイルを含むフォルダー。

` |

### setThreadContext(InputStream stream) {#setThreadContext-java.io.InputStream-}
```
public static void setThreadContext(InputStream stream)
```


現在のスレッドのライセンス コンテキストを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| ストリーム | java.io.InputStream | ライセンスを含むストリームです。 |

