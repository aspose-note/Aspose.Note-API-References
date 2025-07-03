---
title: ExtendedApsImage
second_title: Aspose.Note for Java API Reference
description: Represents a wrapper for the standard ApsImage which extends some of the drawing behavior.
type: docs
weight: 25
url: /java/com.aspose.note/extendedapsimage/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.ExtendedApsNode](../../com.aspose.note/extendedapsnode)
```
public class ExtendedApsImage extends ExtendedApsNode
```

Represents a wrapper for the standard ApsImage, which extends some of the drawing behavior.
## Constructors

| Constructor | Description |
| --- | --- |
| [ExtendedApsImage(ApsImage internalImage)](#ExtendedApsImage-com.aspose.foundation.rendering.ApsImage-) | Initializes a new instance of the `ExtendedApsImage` class. |
## Methods

| Method | Description |
| --- | --- |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | Adds this node to given `compositeNode`. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | Applies plane transform, moving node in x and y planes. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | Applies scaling to the image. |
| [getBottom()](#getBottom--) | Gets the bottom. |
| [getCopy()](#getCopy--) | Creates a full copy of this node. |
| [getOrigin()](#getOrigin--) | Gets the origin. |
| [getSize()](#getSize--) | Gets the size. |
| [getTop()](#getTop--) | Gets the top. |
| [isBackground()](#isBackground--) | Gets whether the image is a background image. |
### ExtendedApsImage(ApsImage internalImage) {#ExtendedApsImage-com.aspose.foundation.rendering.ApsImage-}
```
public ExtendedApsImage(ApsImage internalImage)
```


Initializes a new instance of the `ExtendedApsImage` class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| internalImage | com.aspose.foundation.rendering.ApsImage | The image. |

### addToCompositeNode(ApsCompositeNode compositeNode) {#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-}
```
public void addToCompositeNode(ApsCompositeNode compositeNode)
```


Adds this node to given `compositeNode`.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| compositeNode | com.aspose.foundation.rendering.ApsCompositeNode |  |

### applyPlaneTransform(System.Drawing.PointF transformVector) {#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-}
```
public void applyPlaneTransform(System.Drawing.PointF transformVector)
```


Applies plane transform, moving node in x and y planes.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| transformVector | com.aspose.ms.System.Drawing.PointF |  |

### applyScaleTransform(float scaleTransform) {#applyScaleTransform-float-}
```
public void applyScaleTransform(float scaleTransform)
```


Applies scaling to the image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| scaleTransform | float | The scale factor for the transformation. |

### getBottom() {#getBottom--}
```
public float getBottom()
```


Gets the bottom.

**Returns:**
float
### getCopy() {#getCopy--}
```
public ExtendedApsNode getCopy()
```


Creates a full copy of this node.

**Returns:**
[ExtendedApsNode](../../com.aspose.note/extendedapsnode) - The `IExtendedApsNode`.
### getOrigin() {#getOrigin--}
```
public System.Drawing.PointF getOrigin()
```


Gets the origin.

**Returns:**
com.aspose.ms.System.Drawing.PointF
### getSize() {#getSize--}
```
public System.Drawing.SizeF getSize()
```


Gets the size.

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getTop() {#getTop--}
```
public float getTop()
```


Gets the top.

**Returns:**
float
### isBackground() {#isBackground--}
```
public final boolean isBackground()
```


Gets whether the image is a background image.

**Returns:**
boolean
