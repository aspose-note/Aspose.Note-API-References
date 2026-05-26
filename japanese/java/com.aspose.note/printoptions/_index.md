---
title: "PrintOptions"
second_title: "Aspose.Note for Java API リファレンス"
description: "ドキュメントの印刷に使用されるオプションです。"
type: docs
weight: 78
url: /ja/java/com.aspose.note/printoptions/
---

**Inheritance:**
java.lang.Object
```
public class PrintOptions
```

ドキュメントの印刷に使用されるオプションです。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [PrintOptions()](#PrintOptions--) | `PrintOptions` クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getDocumentName()](#getDocumentName--) | ドキュメントを印刷中に表示する文書名を取得または設定します（例: 印刷ステータス ダイアログ ボックスやプリンター キュー）。 |
| [getPageSplittingAlgorithm()](#getPageSplittingAlgorithm--) | ページ分割に使用されるアルゴリズムを取得または設定します。 |
| [getPrinterSettings()](#getPrinterSettings--) | プリンター設定を取得または設定します。 |
| [getResolution()](#getResolution--) | 生成された画像の解像度（dpi）を取得または設定します。 |
| [setDocumentName(String value)](#setDocumentName-java.lang.String-) | ドキュメントを印刷中に表示する文書名を取得または設定します（例: 印刷ステータス ダイアログ ボックスやプリンター キュー）。 |
| [setPageSplittingAlgorithm(PageSplittingAlgorithm value)](#setPageSplittingAlgorithm-com.aspose.note.PageSplittingAlgorithm-) | ページ分割に使用されるアルゴリズムを取得または設定します。 |
| [setPrinterSettings(AttributeSet value)](#setPrinterSettings-javax.print.attribute.AttributeSet-) | プリンター設定を取得または設定します。 |
| [setResolution(float value)](#setResolution-float-) | 生成された画像の解像度（dpi）を取得または設定します。 |
### PrintOptions() {#PrintOptions--}
```
public PrintOptions()
```


`PrintOptions` クラスの新しいインスタンスを初期化します。

### getDocumentName() {#getDocumentName--}
```
public String getDocumentName()
```


ドキュメントを印刷中に表示する文書名を取得または設定します（例: 印刷ステータス ダイアログ ボックスやプリンター キュー）。

**Returns:**
java.lang.String
### getPageSplittingAlgorithm() {#getPageSplittingAlgorithm--}
```
public PageSplittingAlgorithm getPageSplittingAlgorithm()
```


ページ分割に使用されるアルゴリズムを取得または設定します。

値: `PageSplittingAlgorithm`。

**Returns:**
[PageSplittingAlgorithm](../../com.aspose.note/pagesplittingalgorithm)
### getPrinterSettings() {#getPrinterSettings--}
```
public AttributeSet getPrinterSettings()
```


プリンター設定を取得または設定します。

**Returns:**
javax.print.attribute.AttributeSet
### getResolution() {#getResolution--}
```
public float getResolution()
```


生成された画像の解像度（dpi）を取得または設定します。

--------------------

デフォルト値は 96 です。

**Returns:**
float
### setDocumentName(String value) {#setDocumentName-java.lang.String-}
```
public void setDocumentName(String value)
```


ドキュメントを印刷中に表示する文書名を取得または設定します（例: 印刷ステータス ダイアログ ボックスやプリンター キュー）。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | java.lang.String |  |

### setPageSplittingAlgorithm(PageSplittingAlgorithm value) {#setPageSplittingAlgorithm-com.aspose.note.PageSplittingAlgorithm-}
```
public void setPageSplittingAlgorithm(PageSplittingAlgorithm value)
```


ページ分割に使用されるアルゴリズムを取得または設定します。

値: `PageSplittingAlgorithm`。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [PageSplittingAlgorithm](../../com.aspose.note/pagesplittingalgorithm) |  |

### setPrinterSettings(AttributeSet value) {#setPrinterSettings-javax.print.attribute.AttributeSet-}
```
public void setPrinterSettings(AttributeSet value)
```


プリンター設定を取得または設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | javax.print.attribute.AttributeSet |  |

### setResolution(float value) {#setResolution-float-}
```
public void setResolution(float value)
```


生成された画像の解像度（dpi）を取得または設定します。

--------------------

デフォルト値は 96 です。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | float |  |

