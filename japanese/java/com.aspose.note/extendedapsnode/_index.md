---
title: "ExtendedApsNode"
second_title: "Aspose.Note for Java API リファレンス"
description: "標準的な ApsNode のラッパーを表し、描画動作の一部を拡張します。"
type: docs
weight: 26
url: /ja/java/com.aspose.note/extendedapsnode/
---

**Inheritance:**
java.lang.Object
```
public abstract class ExtendedApsNode
```

標準 ApsNode のラッパーを表し、描画動作の一部を拡張します。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [ExtendedApsNode()](#ExtendedApsNode--) |  |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | このノードを指定された `compositeNode` に追加します。 |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | 平面変換を適用し、ノードを x および y 平面で移動させます。 |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | ノードにスケーリングを適用します。 |
| [copyAttributes(ApsNode src, ApsNode dst)](#copyAttributes-com.aspose.foundation.rendering.ApsNode-com.aspose.foundation.rendering.ApsNode-) |  |
| [copyAttributes(ApsNodeAttributes src, ApsNodeAttributes dst)](#copyAttributes-com.aspose.foundation.rendering.ApsNodeAttributes-com.aspose.foundation.rendering.ApsNodeAttributes-) |  |
| [getBottom()](#getBottom--) | ノードの底部の y 座標を取得または設定します。 |
| [getCopy()](#getCopy--) | このノードの完全なコピーを作成します。 |
| [getOrigin()](#getOrigin--) | ノードの原点を取得または設定します。 |
| [getSize()](#getSize--) | ノードのサイズを取得または設定します。 |
| [getTop()](#getTop--) | ノードの上部の y 座標を取得または設定します。 |
### ExtendedApsNode() {#ExtendedApsNode--}
```
public ExtendedApsNode()
```


### addToCompositeNode(ApsCompositeNode compositeNode) {#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-}
```
public abstract void addToCompositeNode(ApsCompositeNode compositeNode)
```


このノードを指定された `compositeNode` に追加します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| compositeNode | com.aspose.foundation.rendering.ApsCompositeNode |  |

### applyPlaneTransform(System.Drawing.PointF transformVector) {#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-}
```
public abstract void applyPlaneTransform(System.Drawing.PointF transformVector)
```


平面変換を適用し、ノードを x および y 平面で移動させます。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| transformVector | com.aspose.ms.System.Drawing.PointF |  |

### applyScaleTransform(float scaleTransform) {#applyScaleTransform-float-}
```
public abstract void applyScaleTransform(float scaleTransform)
```


ノードにスケーリングを適用します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| scaleTransform | float | 変換のスケール係数です。 |

### copyAttributes(ApsNode src, ApsNode dst) {#copyAttributes-com.aspose.foundation.rendering.ApsNode-com.aspose.foundation.rendering.ApsNode-}
```
public static void copyAttributes(ApsNode src, ApsNode dst)
```




**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| src | com.aspose.foundation.rendering.ApsNode |  |
| dst | com.aspose.foundation.rendering.ApsNode |  |

### copyAttributes(ApsNodeAttributes src, ApsNodeAttributes dst) {#copyAttributes-com.aspose.foundation.rendering.ApsNodeAttributes-com.aspose.foundation.rendering.ApsNodeAttributes-}
```
public static void copyAttributes(ApsNodeAttributes src, ApsNodeAttributes dst)
```




**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| src | com.aspose.foundation.rendering.ApsNodeAttributes |  |
| dst | com.aspose.foundation.rendering.ApsNodeAttributes |  |

### getBottom() {#getBottom--}
```
public float getBottom()
```


ノードの底部の y 座標を取得または設定します。

**Returns:**
float
### getCopy() {#getCopy--}
```
public abstract ExtendedApsNode getCopy()
```


このノードの完全なコピーを作成します。

**Returns:**
[ExtendedApsNode](../../com.aspose.note/extendedapsnode) - The `!:ExtendedApsNode`.
### getOrigin() {#getOrigin--}
```
public System.Drawing.PointF getOrigin()
```


ノードの原点を取得または設定します。

**Returns:**
com.aspose.ms.System.Drawing.PointF
### getSize() {#getSize--}
```
public System.Drawing.SizeF getSize()
```


ノードのサイズを取得または設定します。

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getTop() {#getTop--}
```
public float getTop()
```


ノードの上部の y 座標を取得または設定します。

**Returns:**
float
