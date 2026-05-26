---
title: "ExtendedApsGlyphs"
second_title: "Aspose.Note for Java API リファレンス"
description: "標準の ApsGlyphs のラッパーを表し、描画動作のいくつかを拡張します。"
type: docs
weight: 24
url: /ja/java/com.aspose.note/extendedapsglyphs/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.ExtendedApsNode](../../com.aspose.note/extendedapsnode)
```
public class ExtendedApsGlyphs extends ExtendedApsNode
```

標準 ApsGlyphs のラッパーを表し、描画動作の一部を拡張します。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [ExtendedApsGlyphs(ApsGlyphs internalGlyphs)](#ExtendedApsGlyphs-com.aspose.foundation.rendering.ApsGlyphs-) | `ExtendedApsGlyphs` クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | このノードを指定された `compositeNode` に追加します。 |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | 平面変換を適用し、ノードを x および y 平面で移動させます。 |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | グリフにスケーリングを適用します。 |
| [getBottom()](#getBottom--) | グリフの下端を取得します。 |
| [getCopy()](#getCopy--) | グリフのコピーを取得します。 |
| [getOrigin()](#getOrigin--) | 原点を取得します。 |
| [getSize()](#getSize--) | サイズを取得します。 |
| [getTop()](#getTop--) | 上端を取得します。 |
### ExtendedApsGlyphs(ApsGlyphs internalGlyphs) {#ExtendedApsGlyphs-com.aspose.foundation.rendering.ApsGlyphs-}
```
public ExtendedApsGlyphs(ApsGlyphs internalGlyphs)
```


`ExtendedApsGlyphs` クラスの新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| internalGlyphs | com.aspose.foundation.rendering.ApsGlyphs | 元の aps グリフ。 |

### addToCompositeNode(ApsCompositeNode compositeNode) {#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-}
```
public void addToCompositeNode(ApsCompositeNode compositeNode)
```


このノードを指定された `compositeNode` に追加します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| compositeNode | com.aspose.foundation.rendering.ApsCompositeNode |  |

### applyPlaneTransform(System.Drawing.PointF transformVector) {#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-}
```
public void applyPlaneTransform(System.Drawing.PointF transformVector)
```


平面変換を適用し、ノードを x および y 平面で移動させます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| transformVector | com.aspose.ms.System.Drawing.PointF |  |

### applyScaleTransform(float scaleTransform) {#applyScaleTransform-float-}
```
public void applyScaleTransform(float scaleTransform)
```


グリフにスケーリングを適用します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| scaleTransform | float | 変換のスケール係数です。 |

### getBottom() {#getBottom--}
```
public float getBottom()
```


グリフの下端を取得します。

**Returns:**
float
### getCopy() {#getCopy--}
```
public ExtendedApsNode getCopy()
```


グリフのコピーを取得します。

**Returns:**
[ExtendedApsNode](../../com.aspose.note/extendedapsnode) - The `IExtendedApsNode`.
### getOrigin() {#getOrigin--}
```
public System.Drawing.PointF getOrigin()
```


原点を取得します。

**Returns:**
com.aspose.ms.System.Drawing.PointF
### getSize() {#getSize--}
```
public System.Drawing.SizeF getSize()
```


サイズを取得します。

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getTop() {#getTop--}
```
public float getTop()
```


上端を取得します。

**Returns:**
float
