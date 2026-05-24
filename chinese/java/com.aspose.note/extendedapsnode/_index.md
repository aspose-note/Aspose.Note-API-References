---
title: "ExtendedApsNode"
second_title: "Aspose.Note for Java API 参考"
description: "表示标准 ApsNode 的包装器，扩展了一些绘图行为。"
type: docs
weight: 26
url: /zh/java/com.aspose.note/extendedapsnode/
---

**Inheritance:**
java.lang.Object
```
public abstract class ExtendedApsNode
```

表示标准 ApsNode 的包装器，扩展了一些绘图行为。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [ExtendedApsNode()](#ExtendedApsNode--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | 将此节点添加到给定的 `compositeNode`。 |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | 应用平面变换，将节点在 x 和 y 平面上移动。 |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | 对节点应用缩放。 |
| [copyAttributes(ApsNode src, ApsNode dst)](#copyAttributes-com.aspose.foundation.rendering.ApsNode-com.aspose.foundation.rendering.ApsNode-) |  |
| [copyAttributes(ApsNodeAttributes src, ApsNodeAttributes dst)](#copyAttributes-com.aspose.foundation.rendering.ApsNodeAttributes-com.aspose.foundation.rendering.ApsNodeAttributes-) |  |
| [getBottom()](#getBottom--) | 获取或设置节点底部的 y 坐标。 |
| [getCopy()](#getCopy--) | 创建此节点的完整副本。 |
| [getOrigin()](#getOrigin--) | 获取或设置节点的原点。 |
| [getSize()](#getSize--) | 获取或设置节点的大小。 |
| [getTop()](#getTop--) | 获取或设置节点顶部的 y 坐标。 |
### ExtendedApsNode() {#ExtendedApsNode--}
```
public ExtendedApsNode()
```


### addToCompositeNode(ApsCompositeNode compositeNode) {#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-}
```
public abstract void addToCompositeNode(ApsCompositeNode compositeNode)
```


将此节点添加到给定的 `compositeNode`。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| compositeNode | com.aspose.foundation.rendering.ApsCompositeNode |  |

### applyPlaneTransform(System.Drawing.PointF transformVector) {#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-}
```
public abstract void applyPlaneTransform(System.Drawing.PointF transformVector)
```


应用平面变换，将节点在 x 和 y 平面上移动。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| transformVector | com.aspose.ms.System.Drawing.PointF |  |

### applyScaleTransform(float scaleTransform) {#applyScaleTransform-float-}
```
public abstract void applyScaleTransform(float scaleTransform)
```


对节点应用缩放。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| scaleTransform | float | 用于转换的比例因子。 |

### copyAttributes(ApsNode src, ApsNode dst) {#copyAttributes-com.aspose.foundation.rendering.ApsNode-com.aspose.foundation.rendering.ApsNode-}
```
public static void copyAttributes(ApsNode src, ApsNode dst)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| src | com.aspose.foundation.rendering.ApsNode |  |
| dst | com.aspose.foundation.rendering.ApsNode |  |

### copyAttributes(ApsNodeAttributes src, ApsNodeAttributes dst) {#copyAttributes-com.aspose.foundation.rendering.ApsNodeAttributes-com.aspose.foundation.rendering.ApsNodeAttributes-}
```
public static void copyAttributes(ApsNodeAttributes src, ApsNodeAttributes dst)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| src | com.aspose.foundation.rendering.ApsNodeAttributes |  |
| dst | com.aspose.foundation.rendering.ApsNodeAttributes |  |

### getBottom() {#getBottom--}
```
public float getBottom()
```


获取或设置节点底部的 y 坐标。

**Returns:**
float
### getCopy() {#getCopy--}
```
public abstract ExtendedApsNode getCopy()
```


创建此节点的完整副本。

**Returns:**
[ExtendedApsNode](../../com.aspose.note/extendedapsnode) - The `!:ExtendedApsNode`.
### getOrigin() {#getOrigin--}
```
public System.Drawing.PointF getOrigin()
```


获取或设置节点的原点。

**Returns:**
com.aspose.ms.System.Drawing.PointF
### getSize() {#getSize--}
```
public System.Drawing.SizeF getSize()
```


获取或设置节点的大小。

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getTop() {#getTop--}
```
public float getTop()
```


获取或设置节点顶部的 y 坐标。

**Returns:**
float
