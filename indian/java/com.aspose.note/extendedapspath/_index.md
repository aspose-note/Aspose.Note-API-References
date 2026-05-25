---
title: "ExtendedApsPath"
second_title: "Aspose.Note for Java API Reference"
description: "मानक ApsPath के लिए एक रैपर का प्रतिनिधित्व करता है जो कुछ ड्रॉइंग व्यवहार को विस्तारित करता है।"
type: docs
weight: 28
url: /hi/java/com.aspose.note/extendedapspath/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.ExtendedApsNode](../../com.aspose.note/extendedapsnode)
```
public class ExtendedApsPath extends ExtendedApsNode
```

Represents a wrapper for the standard ApsPath, which extends some of the drawing behavior.
## Constructors

| Constructor | Description |
| --- | --- |
| [ExtendedApsPath(ApsPath internalApsPath)](#ExtendedApsPath-com.aspose.foundation.rendering.ApsPath-) | `ExtendedApsPath` क्लास का एक नया उदाहरण प्रारंभ करता है। |
## Methods

| Method | Description |
| --- | --- |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | Adds this node to given `compositeNode`. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | Applies plane transform, moving node in x and y planes. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | Applies scaling to the node. |
| [getBottom()](#getBottom--) | नीचे प्राप्त करता है। |
| [getCopy()](#getCopy--) | Creates a full copy of this node. |
| [getTop()](#getTop--) | Gets the top. |
### ExtendedApsPath(ApsPath internalApsPath) {#ExtendedApsPath-com.aspose.foundation.rendering.ApsPath-}
```
public ExtendedApsPath(ApsPath internalApsPath)
```


`ExtendedApsPath` क्लास का एक नया उदाहरण प्रारंभ करता है।

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| internalApsPath | com.aspose.foundation.rendering.ApsPath | aps पथ। |

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


Applies scaling to the node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| scaleTransform | float | The scale factor for the transformation. |

### getBottom() {#getBottom--}
```
public float getBottom()
```


नीचे प्राप्त करता है।

**Returns:**
float
### getCopy() {#getCopy--}
```
public ExtendedApsNode getCopy()
```


Creates a full copy of this node.

**Returns:**
[ExtendedApsNode](../../com.aspose.note/extendedapsnode) - The `IExtendedApsNode`.
### getTop() {#getTop--}
```
public float getTop()
```


Gets the top.

**Returns:**
float
