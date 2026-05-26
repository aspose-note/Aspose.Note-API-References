---
title: "DocumentFontsSubsystem"
second_title: "Aspose.Note for Java API リファレンス"
description: "Aspose.Note.Fonts.FontsSubsystem のシンプルな実装です。"
type: docs
weight: 10
url: /ja/java/com.aspose.note.fonts/documentfontssubsystem/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.fonts.FontsSubsystem](../../com.aspose.note.fonts/fontssubsystem)
```
public class DocumentFontsSubsystem extends FontsSubsystem
```

Aspose.Note.Fonts.FontsSubsystem のシンプルな実装です。OS から FontFamily オブジェクトを取得します。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [DocumentFontsSubsystem(InputStream defaultFontStream, Map&lt;String,String&gt; fontsSubstitutions)](#DocumentFontsSubsystem-java.io.InputStream-java.util.Map-java.lang.String-java.lang.String--) | [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) クラスの新しいインスタンスを初期化します。 |
| [DocumentFontsSubsystem(InputStream defaultFontStream)](#DocumentFontsSubsystem-java.io.InputStream-) | [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) クラスの新しいインスタンスを初期化します。 |
| [DocumentFontsSubsystem(String defaultFontFile, Map&lt;String,String&gt; fontsSubstitutions)](#DocumentFontsSubsystem-java.lang.String-java.util.Map-java.lang.String-java.lang.String--) | [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) クラスの新しいインスタンスを初期化します。 |
| [DocumentFontsSubsystem(String defaultFontFile)](#DocumentFontsSubsystem-java.lang.String-) | [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) クラスの新しいインスタンスを初期化します。 |
| [DocumentFontsSubsystem(Map&lt;String,String&gt; fontsSubstitutions)](#DocumentFontsSubsystem-java.util.Map-java.lang.String-java.lang.String--) | [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) クラスの新しいインスタンスを初期化します。 |
| [DocumentFontsSubsystem()](#DocumentFontsSubsystem--) | [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getDefault()](#getDefault--) | 静的なデフォルトインスタンスを取得または設定します。 |
| [setDefault(DocumentFontsSubsystem value)](#setDefault-com.aspose.note.fonts.DocumentFontsSubsystem-) | 静的なデフォルトインスタンスを取得または設定します。 |
| [usingDefaultFont(String defaultFontName)](#usingDefaultFont-java.lang.String-) | 指定されたデフォルトフォント名を使用して新しい DocumentFontsSubsystem インスタンスを作成します。 |
| [usingDefaultFont(String defaultFontName, Map&lt;String,String&gt; fontsSubstitutions)](#usingDefaultFont-java.lang.String-java.util.Map-java.lang.String-java.lang.String--) | 指定されたデフォルトフォント名を使用して新しい DocumentFontsSubsystem インスタンスを作成します。 |
| [usingDefaultFontFromFile(String filePath)](#usingDefaultFontFromFile-java.lang.String-) | 指定されたデフォルトフォント名を使用して新しい DocumentFontsSubsystem インスタンスを作成します。 |
| [usingDefaultFontFromFile(String filePath, Map&lt;String,String&gt; fontsSubstitutions)](#usingDefaultFontFromFile-java.lang.String-java.util.Map-java.lang.String-java.lang.String--) | 指定されたファイルからフォントをデフォルトとして使用し、新しい DocumentFontsSubsystem インスタンスを作成します。 |
| [usingDefaultFontFromStream(InputStream defaultFontStream)](#usingDefaultFontFromStream-java.io.InputStream-) | 指定されたストリームからフォントをデフォルトとして使用し、新しい DocumentFontsSubsystem インスタンスを作成します。 |
| [usingDefaultFontFromStream(InputStream defaultFontStream, Map&lt;String,String&gt; fontsSubstitutions)](#usingDefaultFontFromStream-java.io.InputStream-java.util.Map-java.lang.String-java.lang.String--) | 指定されたストリームからフォントをデフォルトとして使用し、新しい DocumentFontsSubsystem インスタンスを作成します。 |
### DocumentFontsSubsystem(InputStream defaultFontStream, Map&lt;String,String&gt; fontsSubstitutions) {#DocumentFontsSubsystem-java.io.InputStream-java.util.Map-java.lang.String-java.lang.String--}
```
public DocumentFontsSubsystem(InputStream defaultFontStream, Map<String,String> fontsSubstitutions)
```


[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) クラスの新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| defaultFontStream | java.io.InputStream | デフォルトフォントを含むストリームです。 |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | フォント置換です。 |

### DocumentFontsSubsystem(InputStream defaultFontStream) {#DocumentFontsSubsystem-java.io.InputStream-}
```
public DocumentFontsSubsystem(InputStream defaultFontStream)
```


[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) クラスの新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| defaultFontStream | java.io.InputStream | デフォルトフォントを含むストリームです。 |

### DocumentFontsSubsystem(String defaultFontFile, Map&lt;String,String&gt; fontsSubstitutions) {#DocumentFontsSubsystem-java.lang.String-java.util.Map-java.lang.String-java.lang.String--}
```
public DocumentFontsSubsystem(String defaultFontFile, Map<String,String> fontsSubstitutions)
```


[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) クラスの新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| defaultFontFile | java.lang.String | デフォルトフォントを含むファイルへのパスです。 |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | フォント置換です。 |

### DocumentFontsSubsystem(String defaultFontFile) {#DocumentFontsSubsystem-java.lang.String-}
```
public DocumentFontsSubsystem(String defaultFontFile)
```


[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) クラスの新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| defaultFontFile | java.lang.String | デフォルトフォントを含むファイルへのパスです。 |

### DocumentFontsSubsystem(Map&lt;String,String&gt; fontsSubstitutions) {#DocumentFontsSubsystem-java.util.Map-java.lang.String-java.lang.String--}
```
public DocumentFontsSubsystem(Map<String,String> fontsSubstitutions)
```


[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) クラスの新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | フォント置換です。 |

### DocumentFontsSubsystem() {#DocumentFontsSubsystem--}
```
public DocumentFontsSubsystem()
```


[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) クラスの新しいインスタンスを初期化します。

### getDefault() {#getDefault--}
```
public static DocumentFontsSubsystem getDefault()
```


静的なデフォルトインスタンスを取得または設定します。

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem)
### setDefault(DocumentFontsSubsystem value) {#setDefault-com.aspose.note.fonts.DocumentFontsSubsystem-}
```
public static void setDefault(DocumentFontsSubsystem value)
```


静的なデフォルトインスタンスを取得または設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) |  |

### usingDefaultFont(String defaultFontName) {#usingDefaultFont-java.lang.String-}
```
public static DocumentFontsSubsystem usingDefaultFont(String defaultFontName)
```


指定されたデフォルトフォント名を使用して新しい DocumentFontsSubsystem インスタンスを作成します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| defaultFontName | java.lang.String | デフォルトフォント名です。 |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFont(String defaultFontName, Map&lt;String,String&gt; fontsSubstitutions) {#usingDefaultFont-java.lang.String-java.util.Map-java.lang.String-java.lang.String--}
```
public static DocumentFontsSubsystem usingDefaultFont(String defaultFontName, Map<String,String> fontsSubstitutions)
```


指定されたデフォルトフォント名を使用して新しい DocumentFontsSubsystem インスタンスを作成します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| defaultFontName | java.lang.String | デフォルトフォント名です。 |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | フォント置換です。 |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFontFromFile(String filePath) {#usingDefaultFontFromFile-java.lang.String-}
```
public static DocumentFontsSubsystem usingDefaultFontFromFile(String filePath)
```


指定されたデフォルトフォント名を使用して新しい DocumentFontsSubsystem インスタンスを作成します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| filePath | java.lang.String | デフォルトフォント名を含むファイルです。 |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFontFromFile(String filePath, Map&lt;String,String&gt; fontsSubstitutions) {#usingDefaultFontFromFile-java.lang.String-java.util.Map-java.lang.String-java.lang.String--}
```
public static DocumentFontsSubsystem usingDefaultFontFromFile(String filePath, Map<String,String> fontsSubstitutions)
```


指定されたファイルからフォントをデフォルトとして使用し、新しい DocumentFontsSubsystem インスタンスを作成します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| filePath | java.lang.String | デフォルトフォント名を含むファイルです。 |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | フォント置換です。 |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFontFromStream(InputStream defaultFontStream) {#usingDefaultFontFromStream-java.io.InputStream-}
```
public static DocumentFontsSubsystem usingDefaultFontFromStream(InputStream defaultFontStream)
```


指定されたストリームからフォントをデフォルトとして使用し、新しい DocumentFontsSubsystem インスタンスを作成します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| defaultFontStream | java.io.InputStream | デフォルトフォント名を含むストリームです。 |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFontFromStream(InputStream defaultFontStream, Map&lt;String,String&gt; fontsSubstitutions) {#usingDefaultFontFromStream-java.io.InputStream-java.util.Map-java.lang.String-java.lang.String--}
```
public static DocumentFontsSubsystem usingDefaultFontFromStream(InputStream defaultFontStream, Map<String,String> fontsSubstitutions)
```


指定されたストリームからフォントをデフォルトとして使用し、新しい DocumentFontsSubsystem インスタンスを作成します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| defaultFontStream | java.io.InputStream | デフォルトフォント名を含むストリームです。 |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | フォント置換です。 |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
