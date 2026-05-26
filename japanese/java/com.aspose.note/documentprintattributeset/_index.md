---
title: "DocumentPrintAttributeSet"
second_title: "Aspose.Note for Java API リファレンス"
description: "AttributeSet 用のユーザーフレンドリーなインターフェイスを備えたヘルパークラスを表します。"
type: docs
weight: 21
url: /ja/java/com.aspose.note/documentprintattributeset/
---

**Inheritance:**
java.lang.Object, javax.print.attribute.HashAttributeSet
```
public final class DocumentPrintAttributeSet extends HashAttributeSet
```

AttributeSet 用のユーザーフレンドリーなインターフェイスを備えたヘルパークラスを表します。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [DocumentPrintAttributeSet(int copies)](#DocumentPrintAttributeSet-int-) | `DocumentPrintAttributeSet` の新しいインスタンスを初期化します。 |
| [DocumentPrintAttributeSet(String printerName, int copies)](#DocumentPrintAttributeSet-java.lang.String-int-) | `DocumentPrintAttributeSet` の新しいインスタンスを初期化します。 |
| [DocumentPrintAttributeSet(String printerName)](#DocumentPrintAttributeSet-java.lang.String-) | `DocumentPrintAttributeSet` の新しいインスタンスを初期化します。 |
| [DocumentPrintAttributeSet()](#DocumentPrintAttributeSet--) | `DocumentPrintAttributeSet` の新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getCopies()](#getCopies--) |  |
| [getLandscape()](#getLandscape--) |  |
| [getPrinterName()](#getPrinterName--) |  |
| [setCollate(boolean value)](#setCollate-boolean-) | 文書が段組みされているかどうかを示す値を設定します。 |
| [setCopies(int value)](#setCopies-int-) | 印刷する部数を設定します。 |
| [setDuplex(boolean value)](#setDuplex-boolean-) | 両面印刷のプリンター設定を指定します。 |
| [setLandscape(boolean value)](#setLandscape-boolean-) | ページの向きを設定します。 |
| [setPrintRange(int page)](#setPrintRange-int-) | 印刷する単一ページを設定します。 |
| [setPrintRange(int from, int to)](#setPrintRange-int-int-) | 印刷するページ範囲を設定します。 |
| [setPrinterName(String printerName)](#setPrinterName-java.lang.String-) | 使用するプリンターの名前です。 |
| [setPrinterName(String printerName, Locale locale)](#setPrinterName-java.lang.String-java.util.Locale-) | 使用するプリンターの名前です。 |
### DocumentPrintAttributeSet(int copies) {#DocumentPrintAttributeSet-int-}
```
public DocumentPrintAttributeSet(int copies)
```


`DocumentPrintAttributeSet` の新しいインスタンスを初期化します。デフォルトでは文書のすべてのページが印刷されます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 部数 | int | 印刷する文書の部数です。 |

### DocumentPrintAttributeSet(String printerName, int copies) {#DocumentPrintAttributeSet-java.lang.String-int-}
```
public DocumentPrintAttributeSet(String printerName, int copies)
```


`DocumentPrintAttributeSet` の新しいインスタンスを初期化します。デフォルトでは文書のすべてのページが印刷されます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| printerName | java.lang.String | プリンターの名前です。 |
| 部数 | int | 印刷する文書の部数です。 |

### DocumentPrintAttributeSet(String printerName) {#DocumentPrintAttributeSet-java.lang.String-}
```
public DocumentPrintAttributeSet(String printerName)
```


`DocumentPrintAttributeSet` の新しいインスタンスを初期化します。デフォルトでは各ページは1部のみです。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| printerName | java.lang.String | プリンターの名前です。 |

### DocumentPrintAttributeSet() {#DocumentPrintAttributeSet--}
```
public DocumentPrintAttributeSet()
```


`DocumentPrintAttributeSet` の新しいインスタンスを初期化します。デフォルトでは各ページは1部のみです。

### getCopies() {#getCopies--}
```
public int getCopies()
```




**Returns:**
int
### getLandscape() {#getLandscape--}
```
public boolean getLandscape()
```




**Returns:**
boolean
### getPrinterName() {#getPrinterName--}
```
public String getPrinterName()
```




**Returns:**
java.lang.String
### setCollate(boolean value) {#setCollate-boolean-}
```
public void setCollate(boolean value)
```


文書が段組みされているかどうかを示す値を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | true は SheetCollate.COLLATED の設定に相当し、false は SheetCollate.UNCOLLATED の設定に相当します。 |

### setCopies(int value) {#setCopies-int-}
```
public void setCopies(int value)
```


印刷する部数を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int | 印刷する部数です。 |

### setDuplex(boolean value) {#setDuplex-boolean-}
```
public void setDuplex(boolean value)
```


両面印刷のプリンター設定を指定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | true は Sides.DUPLEX の設定に相当し、false は Sides.ONE\_SIDED の設定に相当します。 |

### setLandscape(boolean value) {#setLandscape-boolean-}
```
public void setLandscape(boolean value)
```


ページの向きを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | boolean | true は OrientationRequested.LANDSCAPE の設定に相当し、false は OrientationRequested.PORTRAIT の設定に相当します。 |

### setPrintRange(int page) {#setPrintRange-int-}
```
public void setPrintRange(int page)
```


印刷する単一ページを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| ページ | int | 印刷するページです。 |

### setPrintRange(int from, int to) {#setPrintRange-int-int-}
```
public void setPrintRange(int from, int to)
```


印刷するページ範囲を設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| から | int | 最初のページです。 |
| まで | int | 最後のページ。 |

### setPrinterName(String printerName) {#setPrinterName-java.lang.String-}
```
public void setPrinterName(String printerName)
```


使用するプリンターの名前です。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| printerName | java.lang.String | プリンターの名前です。 |

### setPrinterName(String printerName, Locale locale) {#setPrinterName-java.lang.String-java.util.Locale-}
```
public void setPrinterName(String printerName, Locale locale)
```


使用するプリンターの名前です。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| printerName | java.lang.String | プリンターの名前です。 |
| ロケール | java.util.Locale | printerName のロケール。 |

