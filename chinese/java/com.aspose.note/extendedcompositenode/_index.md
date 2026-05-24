---
title: "ExtendedCompositeNode"
second_title: "Aspose.Note for Java API 参考"
description: "合并多个 IExtendedApsNode 实例。"
type: docs
weight: 29
url: /zh/java/com.aspose.note/extendedcompositenode/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.ExtendedApsNode](../../com.aspose.note/extendedapsnode)
```
public class ExtendedCompositeNode extends ExtendedApsNode
```

组合多个 `IExtendedApsNode` 实例。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [ExtendedCompositeNode()](#ExtendedCompositeNode--) | 初始化 `ExtendedCompositeNode` 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [add(ExtendedApsNode extendedApsNode)](#add-com.aspose.note.ExtendedApsNode-) | 将 `extendedApsNode` 添加到内部节点列表中。 |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | 将此节点添加到给定的 `compositeNode`。 |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | 应用平面变换，将节点在 x 和 y 平面上移动。 |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | 对节点应用缩放。 |
| [getApsNodes()](#getApsNodes--) | 获取所有合并到此 `ExtendedCompositeNode` 中的 `IExtendedApsNode` 实例。 |
| [getCopy()](#getCopy--) | 创建此节点的完整副本。 |
### ExtendedCompositeNode() {#ExtendedCompositeNode--}
```
public ExtendedCompositeNode()
```


初始化 `ExtendedCompositeNode` 类的新实例。

### add(ExtendedApsNode extendedApsNode) {#add-com.aspose.note.ExtendedApsNode-}
```
public final void add(ExtendedApsNode extendedApsNode)
```


将 `extendedApsNode` 添加到内部节点列表中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| extendedApsNode | [ExtendedApsNode](../../com.aspose.note/extendedapsnode) |  |

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


对节点应用缩放。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| scaleTransform | float | 用于转换的比例因子。 |

### getApsNodes() {#getApsNodes--}
```
public final System.Collections.Generic.IGenericCollection<ExtendedApsNode> getApsNodes()
```


获取所有合并到此 `ExtendedCompositeNode` 中的 `IExtendedApsNode` 实例。

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericCollection&lt;com.aspose.note.ExtendedApsNode&gt;
### getCopy() {#getCopy--}
```
public ExtendedApsNode getCopy()
```


创建此节点的完整副本。

**Returns:**
[ExtendedApsNode](../../com.aspose.note/extendedapsnode) - The `IExtendedApsNode`.
