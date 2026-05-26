---
title: "KeepPartAndCloneSolidObjectToNextPageAlgorithm"
second_title: "Aspose.Note for Java API リファレンス"
description: "オブジェクトの上部をページの下部に追加し、元のページに収まらない場合はオブジェクト全体を次のページにクローンします。"
type: docs
weight: 42
url: /ja/java/com.aspose.note/keeppartandclonesolidobjecttonextpagealgorithm/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.PageSplittingAlgorithm](../../com.aspose.note/pagesplittingalgorithm)
```
public class KeepPartAndCloneSolidObjectToNextPageAlgorithm extends PageSplittingAlgorithm
```

オブジェクトの上部をページの下部に追加し、元のページに収まらない場合はオブジェクト全体を次のページにクローンします。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [KeepPartAndCloneSolidObjectToNextPageAlgorithm()](#KeepPartAndCloneSolidObjectToNextPageAlgorithm--) | `KeepPartAndCloneSolidObjectToNextPageAlgorithm` クラスの新しいインスタンスを初期化し、クローン部分のデフォルトの高さ制限を使用します。 |
| [KeepPartAndCloneSolidObjectToNextPageAlgorithm(float heightLimitOfClonedPart)](#KeepPartAndCloneSolidObjectToNextPageAlgorithm-float-) | `KeepPartAndCloneSolidObjectToNextPageAlgorithm` クラスの新しいインスタンスを初期化し、クローン部分の特定の高さ制限を使用します。 |
## フィールド

| フィールド | 説明 |
| --- | --- |
| [DEFAULT_HEIGHT_LIMIT_OF_CLONED_PART](#DEFAULT-HEIGHT-LIMIT-OF-CLONED-PART) | クローン部分のデフォルトの最大サイズです。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getHeightLimitOfClonedPart()](#getHeightLimitOfClonedPart--) | クローン部分の高さ制限を取得します。 |
### KeepPartAndCloneSolidObjectToNextPageAlgorithm() {#KeepPartAndCloneSolidObjectToNextPageAlgorithm--}
```
public KeepPartAndCloneSolidObjectToNextPageAlgorithm()
```


`KeepPartAndCloneSolidObjectToNextPageAlgorithm` クラスの新しいインスタンスを初期化し、クローン部分のデフォルトの高さ制限を使用します。

### KeepPartAndCloneSolidObjectToNextPageAlgorithm(float heightLimitOfClonedPart) {#KeepPartAndCloneSolidObjectToNextPageAlgorithm-float-}
```
public KeepPartAndCloneSolidObjectToNextPageAlgorithm(float heightLimitOfClonedPart)
```


`KeepPartAndCloneSolidObjectToNextPageAlgorithm` クラスの新しいインスタンスを初期化し、クローン部分の特定の高さ制限を使用します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| heightLimitOfClonedPart | float | クローンされた部分の最大高さ。 |

### DEFAULT_HEIGHT_LIMIT_OF_CLONED_PART {#DEFAULT-HEIGHT-LIMIT-OF-CLONED-PART}
```
public static final float DEFAULT_HEIGHT_LIMIT_OF_CLONED_PART
```


クローン部分のデフォルトの最大サイズです。

### getHeightLimitOfClonedPart() {#getHeightLimitOfClonedPart--}
```
public float getHeightLimitOfClonedPart()
```


クローン部分の高さ制限を取得します。

**Returns:**
float
