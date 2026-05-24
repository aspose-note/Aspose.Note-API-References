---
title: "ExtendedApsImage"
second_title: "Aspose.Note for Java API 参考"
description: "表示标准 ApsImage 的包装器，扩展了一些绘图行为。"
type: docs
weight: 25
url: /zh/java/com.aspose.note/extendedapsimage/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.ExtendedApsNode](../../com.aspose.note/extendedapsnode)
```
public class ExtendedApsImage extends ExtendedApsNode
```

表示标准 ApsImage 的包装器，扩展了一些绘图行为。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [ExtendedApsImage(ApsImage internalImage)](#ExtendedApsImage-com.aspose.foundation.rendering.ApsImage-) | 初始化 `ExtendedApsImage` 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | 将此节点添加到给定的 `compositeNode`。 |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | 应用平面变换，将节点在 x 和 y 平面上移动。 |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | 对图像应用缩放。 |
| [getBottom()](#getBottom--) | 获取底部。 |
| [getCopy()](#getCopy--) | 创建此节点的完整副本。 |
| [getOrigin()](#getOrigin--) | 获取原点。 |
| [getSize()](#getSize--) | 获取大小。 |
| [getTop()](#getTop--) | 获取顶部。 |
| [isBackground()](#isBackground--) | 获取图像是否为背景图像。 |
### ExtendedApsImage(ApsImage internalImage) {#ExtendedApsImage-com.aspose.foundation.rendering.ApsImage-}
```
public ExtendedApsImage(ApsImage internalImage)
```


初始化 `ExtendedApsImage` 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| internalImage | com.aspose.foundation.rendering.ApsImage | 图像。 |

### addToCompositeNode(ApsCompositeNode compositeNode) {#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-}
```
public void addToCompositeNode(ApsCompositeNode compositeNode)
```


将此节点添加到给定的 `compositeNode`。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| compositeNode | com.aspose.foundation.rendering.ApsCompositeNode |  |

### applyPlaneTransform(System.Drawing.PointF transformVector) {#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-}
```
public void applyPlaneTransform(System.Drawing.PointF transformVector)
```


应用平面变换，将节点在 x 和 y 平面上移动。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| transformVector | com.aspose.ms.System.Drawing.PointF |  |

### applyScaleTransform(float scaleTransform) {#applyScaleTransform-float-}
```
public void applyScaleTransform(float scaleTransform)
```


对图像应用缩放。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| scaleTransform | float | 用于转换的比例因子。 |

### getBottom() {#getBottom--}
```
public float getBottom()
```


获取底部。

**Returns:**
float
### getCopy() {#getCopy--}
```
public ExtendedApsNode getCopy()
```


创建此节点的完整副本。

**Returns:**
[ExtendedApsNode](../../com.aspose.note/extendedapsnode) - The `IExtendedApsNode`.
### getOrigin() {#getOrigin--}
```
public System.Drawing.PointF getOrigin()
```


获取原点。

**Returns:**
com.aspose.ms.System.Drawing.PointF
### getSize() {#getSize--}
```
public System.Drawing.SizeF getSize()
```


获取大小。

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getTop() {#getTop--}
```
public float getTop()
```


获取顶部。

**Returns:**
float
### isBackground() {#isBackground--}
```
public final boolean isBackground()
```


获取图像是否为背景图像。

**Returns:**
boolean
