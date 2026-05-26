---
title: "NumberList"
second_title: "Aspose.Note for Java API リファレンス"
description: "番号付きまたは箇条書きリストを表します。"
type: docs
weight: 64
url: /ja/java/com.aspose.note/numberlist/
---

**Inheritance:**
java.lang.Object
```
public class NumberList
```

番号付きまたは箇条書きリストを表します。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [NumberList(String bulletedSymbol, String font, int fontSize)](#NumberList-java.lang.String-java.lang.String-int-) | `NumberList` クラスの新しいインスタンスを初期化します。 |
| [NumberList(String format, byte numberFormat, String font, int fontSize)](#NumberList-java.lang.String-byte-java.lang.String-int-) | `NumberList` クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [equals(NumberList other)](#equals-com.aspose.note.NumberList-) | 指定されたオブジェクトが現在のオブジェクトと等しいかどうかを判断します。 |
| [equals(Object obj)](#equals-java.lang.Object-) | 指定されたオブジェクトが現在のオブジェクトと等しいかどうかを判断します。 |
| [getFont()](#getFont--) | フォントの名前を取得または設定します。 |
| [getFontColor()](#getFontColor--) | フォントの色を取得または設定します。 |
| [getFontSize()](#getFontSize--) | フォントサイズを取得または設定します。 |
| [getFormat()](#getFormat--) | 行ヘッダーの形式を取得または設定します。 |
| [getLastModifiedTime()](#getLastModifiedTime--) | 最終更新時刻を取得または設定します。 |
| [getNumberFormat()](#getNumberFormat--) | 自動的に番号付けされたオブジェクトのグループに使用される番号形式を取得または設定します。 |
| [getNumberedListHeader(int sequenceNumber)](#getNumberedListHeader-int-) | 番号付きリストのヘッダーを取得します。 |
| [getRestart()](#getRestart--) | リスト項目の自動番号値を上書きする数値を取得または設定します。 |
| [hashCode()](#hashCode--) | 型のハッシュ関数として機能します。 |
| [isBold()](#isBold--) | テキストスタイルが太字かどうかを示す値を取得または設定します。 |
| [isItalic()](#isItalic--) | テキストスタイルが斜体かどうかを示す値を取得または設定します。 |
| [setBold(boolean value)](#setBold-boolean-) | テキストスタイルが太字かどうかを示す値を取得または設定します。 |
| [setFont(String value)](#setFont-java.lang.String-) | フォントの名前を取得または設定します。 |
| [setFontColor(Color value)](#setFontColor-java.awt.Color-) | フォントの色を取得または設定します。 |
| [setFontSize(int value)](#setFontSize-int-) | フォントサイズを取得または設定します。 |
| [setFormat(String value)](#setFormat-java.lang.String-) | 行ヘッダーの形式を取得または設定します。 |
| [setItalic(boolean value)](#setItalic-boolean-) | テキストスタイルが斜体かどうかを示す値を取得または設定します。 |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | 最終更新時刻を取得または設定します。 |
| [setNumberFormat(Byte value)](#setNumberFormat-java.lang.Byte-) | 自動的に番号付けされたオブジェクトのグループに使用される番号形式を取得または設定します。 |
| [setRestart(int value)](#setRestart-int-) | リスト項目の自動番号値を上書きする数値を取得または設定します。 |
### NumberList(String bulletedSymbol, String font, int fontSize) {#NumberList-java.lang.String-java.lang.String-int-}
```
public NumberList(String bulletedSymbol, String font, int fontSize)
```


`NumberList` クラスの新しいインスタンスを初期化します。このインスタンスは箇条書きリストを表します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 箇条書きシンボル | java.lang.String | 箇条書きを表すシンボルです。 |
| フォント | java.lang.String | 箇条書き用のフォントです。 |
| フォントサイズ | int | 箇条書き用のフォントサイズです。 |

### NumberList(String format, byte numberFormat, String font, int fontSize) {#NumberList-java.lang.String-byte-java.lang.String-int-}
```
public NumberList(String format, byte numberFormat, String font, int fontSize)
```


`NumberList` クラスの新しいインスタンスを初期化します。このインスタンスは番号付きリストを表します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| format | java.lang.String | 番号付きヘッダーの形式です。 |
| 番号形式 | byte | ヘッダーの番号の形式です。 |
| フォント | java.lang.String | 番号付きヘッダー用のフォントです。 |
| フォントサイズ | int | 番号付きヘッダー用のフォントサイズです。 |

### equals(NumberList other) {#equals-com.aspose.note.NumberList-}
```
public boolean equals(NumberList other)
```


指定されたオブジェクトが現在のオブジェクトと等しいかどうかを判断します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| other | [NumberList](../../com.aspose.note/numberlist) | オブジェクトです。 |

**Returns:**
boolean - `bool`です。
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


指定されたオブジェクトが現在のオブジェクトと等しいかどうかを判断します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| obj | java.lang.Object | オブジェクトです。 |

**Returns:**
boolean - `bool`です。
### getFont() {#getFont--}
```
public String getFont()
```


フォントの名前を取得または設定します。

**Returns:**
java.lang.String
### getFontColor() {#getFontColor--}
```
public Color getFontColor()
```


フォントの色を取得または設定します。

**Returns:**
java.awt.Color
### getFontSize() {#getFontSize--}
```
public int getFontSize()
```


フォントサイズを取得または設定します。

**Returns:**
int
### getFormat() {#getFormat--}
```
public String getFormat()
```


行ヘッダーの形式を取得または設定します。箇条書きリストの場合は箇条記号を表します。

**Returns:**
java.lang.String
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


最終更新時刻を取得または設定します。

**Returns:**
java.util.Date
### getNumberFormat() {#getNumberFormat--}
```
public Byte getNumberFormat()
```


自動番号付けオブジェクトのグループに使用される番号形式を取得または設定します。箇条書きリストの場合は null にする必要があります。

**Returns:**
java.lang.Byte
### getNumberedListHeader(int sequenceNumber) {#getNumberedListHeader-int-}
```
public String getNumberedListHeader(int sequenceNumber)
```


番号付きリストのヘッダーを取得します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| sequenceNumber | int | 番号付きリストのシーケンス番号です。 |

**Returns:**
java.lang.String - 指定されたシーケンス番号の文字列表現です。
### getRestart() {#getRestart--}
```
public int getRestart()
```


リスト項目の自動番号値を上書きする数値を取得または設定します。

**Returns:**
int
### hashCode() {#hashCode--}
```
public int hashCode()
```


型のハッシュ関数として機能します。

**Returns:**
int - `int`です。
### isBold() {#isBold--}
```
public boolean isBold()
```


テキストスタイルが太字かどうかを示す値を取得または設定します。

**Returns:**
boolean
### isItalic() {#isItalic--}
```
public boolean isItalic()
```


テキストスタイルが斜体かどうかを示す値を取得または設定します。

**Returns:**
boolean
### setBold(boolean value) {#setBold-boolean-}
```
public void setBold(boolean value)
```


テキストスタイルが太字かどうかを示す値を取得または設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean |  |

### setFont(String value) {#setFont-java.lang.String-}
```
public void setFont(String value)
```


フォントの名前を取得または設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String |  |

### setFontColor(Color value) {#setFontColor-java.awt.Color-}
```
public void setFontColor(Color value)
```


フォントの色を取得または設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.awt.Color |  |

### setFontSize(int value) {#setFontSize-int-}
```
public void setFontSize(int value)
```


フォントサイズを取得または設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int |  |

### setFormat(String value) {#setFormat-java.lang.String-}
```
public void setFormat(String value)
```


行ヘッダーの形式を取得または設定します。箇条書きリストの場合は箇条記号を表します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String |  |

### setItalic(boolean value) {#setItalic-boolean-}
```
public void setItalic(boolean value)
```


テキストスタイルが斜体かどうかを示す値を取得または設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


最終更新時刻を取得または設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.util.Date |  |

### setNumberFormat(Byte value) {#setNumberFormat-java.lang.Byte-}
```
public void setNumberFormat(Byte value)
```


自動番号付けオブジェクトのグループに使用される番号形式を取得または設定します。箇条書きリストの場合は null にする必要があります。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.Byte |  |

### setRestart(int value) {#setRestart-int-}
```
public void setRestart(int value)
```


リスト項目の自動番号値を上書きする数値を取得または設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int |  |

