---
title: "ExtendedApsPath"
second_title: "Aspose.Note for Java API リファレンス"
description: "標準の ApsPath のラッパーを表し、描画動作の一部を拡張します。"
type: docs
weight: 28
url: /ja/java/com.aspose.note/extendedapspath/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.ExtendedApsNode](../../com.aspose.note/extendedapsnode)
```
public class ExtendedApsPath extends ExtendedApsNode
```

標準 ApsPath のラッパーを表し、描画動作の一部を拡張します。
## コンストラクタ

| コンストラクタ | 説明 |
| --- | --- |
| [ExtendedApsPath(ApsPath internalApsPath)](#ExtendedApsPath-com.aspose.foundation.rendering.ApsPath-) | `ExtendedApsPath` クラスの新しいインスタンスを初期化します。 |
## メソッド

| メソッド | 説明 |
| --- | --- |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | このノードを指定された `compositeNode` に追加します。 |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | 平面変換を適用し、ノードを x および y 平面で移動させます。 |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | ノードにスケーリングを適用します。 |
| [getBottom()](#getBottom--) | 下端を取得します。 |
| [getCopy()](#getCopy--) | このノードの完全なコピーを作成します。 |
| [getTop()](#getTop--) | 上端を取得します。 |
### ExtendedApsPath(ApsPath internalApsPath) {#ExtendedApsPath-com.aspose.foundation.rendering.ApsPath-}
```
public ExtendedApsPath(ApsPath internalApsPath)
```


`ExtendedApsPath` クラスの新しいインスタンスを初期化します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| internalApsPath | com.aspose.foundation.rendering.ApsPath | aps パスです。 |

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


ノードにスケーリングを適用します。

**Parameters:**
| パラメーター | 型 | 説明 |
| --- | --- | --- |
| scaleTransform | float | 変換のスケール係数です。 |

### getBottom() {#getBottom--}
```
public float getBottom()
```


下端を取得します。

**Returns:**
float
### getCopy() {#getCopy--}
```
public ExtendedApsNode getCopy()
```


このノードの完全なコピーを作成します。

**Returns:**
[ExtendedApsNode](../../com.aspose.note/extendedapsnode) - The `IExtendedApsNode`.
### getTop() {#getTop--}
```
public float getTop()
```


上端を取得します。

**Returns:**
float
