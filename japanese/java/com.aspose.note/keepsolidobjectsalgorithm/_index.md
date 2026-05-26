---
title: "KeepSolidObjectsAlgorithm"
second_title: "Aspose.Note for Java API リファレンス"
description: "オブジェクト全体が元のページに収まらない場合、次のページへシフトします。"
type: docs
weight: 43
url: /ja/java/com.aspose.note/keepsolidobjectsalgorithm/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.PageSplittingAlgorithm](../../com.aspose.note/pagesplittingalgorithm)
```
public class KeepSolidObjectsAlgorithm extends PageSplittingAlgorithm
```

元のページに収まらない場合、オブジェクト全体を次のページへ移動します。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [KeepSolidObjectsAlgorithm()](#KeepSolidObjectsAlgorithm--) | `KeepSolidObjectsAlgorithm` クラスの新しいインスタンスを、クローンされた部分のデフォルト高さ制限を使用して初期化します。 |
| [KeepSolidObjectsAlgorithm(float heightLimitOfClonedPart)](#KeepSolidObjectsAlgorithm-float-) | `KeepSolidObjectsAlgorithm` クラスの新しいインスタンスを、クローンされた部分の特定の高さ制限を使用して初期化します。 |
## フィールド

| フィールド | 説明 |
| --- | --- |
| [DEFAULT_HEIGHT_LIMIT_OF_CLONED_PART](#DEFAULT-HEIGHT-LIMIT-OF-CLONED-PART) | クローン部分のデフォルトの最大サイズです。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [getHeightLimitOfClonedPart()](#getHeightLimitOfClonedPart--) | クローン部分の高さ制限を取得します。 |
### KeepSolidObjectsAlgorithm() {#KeepSolidObjectsAlgorithm--}
```
public KeepSolidObjectsAlgorithm()
```


`KeepSolidObjectsAlgorithm` クラスの新しいインスタンスを、クローンされた部分のデフォルト高さ制限を使用して初期化します。

### KeepSolidObjectsAlgorithm(float heightLimitOfClonedPart) {#KeepSolidObjectsAlgorithm-float-}
```
public KeepSolidObjectsAlgorithm(float heightLimitOfClonedPart)
```


`KeepSolidObjectsAlgorithm` クラスの新しいインスタンスを、クローンされた部分の特定の高さ制限を使用して初期化します。

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
