---
title: "ImageSaveOptions"
second_title: "Aspose.Note for Java API リファレンス"
description: "ドキュメントページを画像にレンダリングする際に追加オプションを指定できます。"
type: docs
weight: 35
url: /ja/java/com.aspose.note/imagesaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.SaveOptions](../../com.aspose.note/saveoptions)
```
public class ImageSaveOptions extends SaveOptions
```

ドキュメントページを画像にレンダリングする際に追加オプションを指定できます。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [ImageSaveOptions(int format)](#ImageSaveOptions-int-) | `ImageSaveOptions` クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getBinarizationOptions()](#getBinarizationOptions--) | 画像の二値化オプションを取得または設定します。 |
| [getColorMode()](#getColorMode--) | 出力画像の `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-)) を取得または設定します。 |
| [getQuality()](#getQuality--) | 保存された画像の品質を決定する値を取得します。 |
| [getResolution()](#getResolution--) | 生成された画像の解像度（ドット毎インチ）を取得します。 |
| [getTiffCompression()](#getTiffCompression--) | 生成された画像を TIFF 形式で保存する際に使用する圧縮タイプを取得または設定します。 |
| [setBinarizationOptions(ImageBinarizationOptions value)](#setBinarizationOptions-com.aspose.note.ImageBinarizationOptions-) | 画像の二値化オプションを取得または設定します。 |
| [setColorMode(int value)](#setColorMode-int-) | 出力画像の `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-)) を取得または設定します。 |
| [setQuality(int value)](#setQuality-int-) | 保存された画像の品質を決定する値を設定します。 |
| [setResolution(float value)](#setResolution-float-) | 生成された画像の解像度（dpi）を設定します。 |
| [setTiffCompression(int value)](#setTiffCompression-int-) | 生成された画像を TIFF 形式で保存する際に使用する圧縮タイプを取得または設定します。 |
### ImageSaveOptions(int format) {#ImageSaveOptions-int-}
```
public ImageSaveOptions(int format)
```


`ImageSaveOptions` クラスの新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| format | int | ドキュメントが保存される形式です。 |

### getBinarizationOptions() {#getBinarizationOptions--}
```
public final ImageBinarizationOptions getBinarizationOptions()
```


画像の二値化オプションを取得または設定します。

**Returns:**
[ImageBinarizationOptions](../../com.aspose.note/imagebinarizationoptions)
### getColorMode() {#getColorMode--}
```
public final int getColorMode()
```


出力画像の `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-)) を取得または設定します。

**Returns:**
int
### getQuality() {#getQuality--}
```
public final int getQuality()
```


保存された画像の品質を決定する値を取得します。この値は System.Drawing.Imaging.Encoder.Quality パラメータとしてコーデックに渡されます。

--------------------

品質カテゴリの有用な値の範囲は 0 から 100 です。指定した数値が小さいほど圧縮率が高くなり、画像の品質は低くなります。0 は最低品質の画像、100 は最高品質の画像を表します。デフォルト値は 90 です。

**Returns:**
int
### getResolution() {#getResolution--}
```
public float getResolution()
```


生成された画像の解像度（ドット毎インチ）を取得します。

--------------------

デフォルト値は 96 です。

**Returns:**
float
### getTiffCompression() {#getTiffCompression--}
```
public final int getTiffCompression()
```


生成された画像を TIFF 形式で保存する際に使用する圧縮タイプを取得または設定します。

**Returns:**
int
### setBinarizationOptions(ImageBinarizationOptions value) {#setBinarizationOptions-com.aspose.note.ImageBinarizationOptions-}
```
public final void setBinarizationOptions(ImageBinarizationOptions value)
```


画像の二値化オプションを取得または設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| value | [ImageBinarizationOptions](../../com.aspose.note/imagebinarizationoptions) |  |

### setColorMode(int value) {#setColorMode-int-}
```
public final void setColorMode(int value)
```


出力画像の `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-)) を取得または設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int |  |

### setQuality(int value) {#setQuality-int-}
```
public final void setQuality(int value)
```


保存された画像の品質を決定する値を設定します。この値は System.Drawing.Imaging.Encoder.Quality パラメータとしてコーデックに渡されます。

--------------------

品質カテゴリの有用な値の範囲は 0 から 100 です。指定した数値が小さいほど圧縮率が高くなり、画像の品質は低くなります。0 は最低品質の画像、100 は最高品質の画像を表します。デフォルト値は 90 です。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int |  |

### setResolution(float value) {#setResolution-float-}
```
public void setResolution(float value)
```


生成された画像の解像度（dpi）を設定します。

--------------------

デフォルト値は 90 です。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | float |  |

### setTiffCompression(int value) {#setTiffCompression-int-}
```
public final void setTiffCompression(int value)
```


生成された画像を TIFF 形式で保存する際に使用する圧縮タイプを取得または設定します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| 値 | int |  |

