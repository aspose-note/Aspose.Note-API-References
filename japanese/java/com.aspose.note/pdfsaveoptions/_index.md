---
title: "PdfSaveOptions"
second_title: "Aspose.Note for Java API リファレンス"
description: "ドキュメントページを PDF にレンダリングする際に、追加オプションを指定できるようにします。"
type: docs
weight: 77
url: /ja/java/com.aspose.note/pdfsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.SaveOptions](../../com.aspose.note/saveoptions)
```
public final class PdfSaveOptions extends SaveOptions
```

ドキュメントページを PDF にレンダリングする際に、追加オプションを指定できるようにします。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [PdfSaveOptions()](#PdfSaveOptions--) | `PdfSaveOptions` クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getImageCompression()](#getImageCompression--) | PDF ファイルの画像に適用される圧縮タイプを取得します。 |
| [getJpegQuality()](#getJpegQuality--) | PDF ドキュメント内の JPEG 画像の品質を決定する値を取得します。 |
| [getPageSettings()](#getPageSettings--) | ドキュメント内の各ページのページ設定を取得または設定します。 |
| [getPageSplittingAlgorithm()](#getPageSplittingAlgorithm--) | ページ分割に使用されるアルゴリズムを取得または設定します。 |
| [setImageCompression(int value)](#setImageCompression-int-) | PDF ファイルの画像に適用される圧縮タイプを設定します。 |
| [setJpegQuality(int value)](#setJpegQuality-int-) | PDF ドキュメント内の JPEG 画像の品質を決定する値を設定します。 |
| [setPageSettings(PageSettings value)](#setPageSettings-com.aspose.note.PageSettings-) | ドキュメント内の各ページのページ設定を取得または設定します。 |
| [setPageSplittingAlgorithm(PageSplittingAlgorithm value)](#setPageSplittingAlgorithm-com.aspose.note.PageSplittingAlgorithm-) | ページ分割に使用されるアルゴリズムを取得または設定します。 |
### PdfSaveOptions() {#PdfSaveOptions--}
```
public PdfSaveOptions()
```


`PdfSaveOptions` クラスの新しいインスタンスを初期化します。

### getImageCompression() {#getImageCompression--}
```
public final int getImageCompression()
```


PDF ファイルの画像に適用される圧縮タイプを取得します。

**Returns:**
int
### getJpegQuality() {#getJpegQuality--}
```
public final int getJpegQuality()
```


PDF ドキュメント内の JPEG 画像の品質を決定する値を取得します。値は 0 から 100 の範囲で、0 は最悪の品質だが最大圧縮、100 は最高の品質だが最小圧縮を意味します。

--------------------

デフォルト値は 90 です。

**Returns:**
int
### getPageSettings() {#getPageSettings--}
```
public PageSettings getPageSettings()
```


ドキュメント内の各ページのページ設定を取得または設定します。デフォルトでは CurrentUICulture に依存し、\*US 文化圏はレター設定、その他は A4 設定です。

**Returns:**
[PageSettings](../../com.aspose.note/pagesettings)
### getPageSplittingAlgorithm() {#getPageSplittingAlgorithm--}
```
public PageSplittingAlgorithm getPageSplittingAlgorithm()
```


ページ分割に使用されるアルゴリズムを取得または設定します。

値: `PageSplittingAlgorithm`。

**Returns:**
[PageSplittingAlgorithm](../../com.aspose.note/pagesplittingalgorithm)
### setImageCompression(int value) {#setImageCompression-int-}
```
public final void setImageCompression(int value)
```


PDF ファイルの画像に適用される圧縮タイプを設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int |  |

### setJpegQuality(int value) {#setJpegQuality-int-}
```
public final void setJpegQuality(int value)
```


PDF ドキュメント内の JPEG 画像の品質を決定する値を設定します。値は 0 から 100 の範囲で、0 は最悪の品質だが最大圧縮、100 は最高の品質だが最小圧縮を意味します。

--------------------

デフォルト値は 90 です。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int |  |

### setPageSettings(PageSettings value) {#setPageSettings-com.aspose.note.PageSettings-}
```
public void setPageSettings(PageSettings value)
```


ドキュメント内の各ページのページ設定を取得または設定します。デフォルトでは CurrentUICulture に依存し、\*US 文化圏はレター設定、その他は A4 設定です。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [PageSettings](../../com.aspose.note/pagesettings) |  |

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

