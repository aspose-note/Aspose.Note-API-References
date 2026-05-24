---
title: "ExtendedApsNode"
second_title: "مرجع Aspose.Note for Java API"
description: "يمثل غلافًا لـ ApsNode القياسي الذي يمد بعض سلوكيات الرسم."
type: docs
weight: 26
url: /ar/java/com.aspose.note/extendedapsnode/
---

**Inheritance:**
java.lang.Object
```
public abstract class ExtendedApsNode
```

يمثل غلافًا لـ ApsNode القياسي، الذي يوسع بعض سلوكيات الرسم.
## المنشئات

| المنشئ | الوصف |
| --- | --- |
| [ExtendedApsNode()](#ExtendedApsNode--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | يضيف هذه العقدة إلى `compositeNode` المعطى. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | يطبق تحويل المستوى، محركًا العقدة في مستويي x و y. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | يطبق التحجيم على العقدة. |
| [copyAttributes(ApsNode src, ApsNode dst)](#copyAttributes-com.aspose.foundation.rendering.ApsNode-com.aspose.foundation.rendering.ApsNode-) |  |
| [copyAttributes(ApsNodeAttributes src, ApsNodeAttributes dst)](#copyAttributes-com.aspose.foundation.rendering.ApsNodeAttributes-com.aspose.foundation.rendering.ApsNodeAttributes-) |  |
| [getBottom()](#getBottom--) | يحصل أو يعيّن إحداثي y لأسفل العقدة. |
| [getCopy()](#getCopy--) | ينشئ نسخة كاملة من هذه العقدة. |
| [getOrigin()](#getOrigin--) | يحصل أو يضبط أصل العقدة. |
| [getSize()](#getSize--) | يحصل أو يضبط حجم العقدة. |
| [getTop()](#getTop--) | يحصل أو يضبط إحداثي y لأعلى العقدة. |
### ExtendedApsNode() {#ExtendedApsNode--}
```
public ExtendedApsNode()
```


### addToCompositeNode(ApsCompositeNode compositeNode) {#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-}
```
public abstract void addToCompositeNode(ApsCompositeNode compositeNode)
```


يضيف هذه العقدة إلى `compositeNode` المعطى.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| compositeNode | com.aspose.foundation.rendering.ApsCompositeNode |  |

### applyPlaneTransform(System.Drawing.PointF transformVector) {#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-}
```
public abstract void applyPlaneTransform(System.Drawing.PointF transformVector)
```


يطبق تحويل المستوى، محركًا العقدة في مستويي x و y.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| transformVector | com.aspose.ms.System.Drawing.PointF |  |

### applyScaleTransform(float scaleTransform) {#applyScaleTransform-float-}
```
public abstract void applyScaleTransform(float scaleTransform)
```


يطبق التحجيم على العقدة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| scaleTransform | float | عامل القياس للتحويل. |

### copyAttributes(ApsNode src, ApsNode dst) {#copyAttributes-com.aspose.foundation.rendering.ApsNode-com.aspose.foundation.rendering.ApsNode-}
```
public static void copyAttributes(ApsNode src, ApsNode dst)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| src | com.aspose.foundation.rendering.ApsNode |  |
| dst | com.aspose.foundation.rendering.ApsNode |  |

### copyAttributes(ApsNodeAttributes src, ApsNodeAttributes dst) {#copyAttributes-com.aspose.foundation.rendering.ApsNodeAttributes-com.aspose.foundation.rendering.ApsNodeAttributes-}
```
public static void copyAttributes(ApsNodeAttributes src, ApsNodeAttributes dst)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| src | com.aspose.foundation.rendering.ApsNodeAttributes |  |
| dst | com.aspose.foundation.rendering.ApsNodeAttributes |  |

### getBottom() {#getBottom--}
```
public float getBottom()
```


يحصل أو يعيّن إحداثي y لأسفل العقدة.

**Returns:**
float
### getCopy() {#getCopy--}
```
public abstract ExtendedApsNode getCopy()
```


ينشئ نسخة كاملة من هذه العقدة.

**Returns:**
[ExtendedApsNode](../../com.aspose.note/extendedapsnode) - The `!:ExtendedApsNode`.
### getOrigin() {#getOrigin--}
```
public System.Drawing.PointF getOrigin()
```


يحصل أو يضبط أصل العقدة.

**Returns:**
com.aspose.ms.System.Drawing.PointF
### getSize() {#getSize--}
```
public System.Drawing.SizeF getSize()
```


يحصل أو يضبط حجم العقدة.

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getTop() {#getTop--}
```
public float getTop()
```


يحصل أو يضبط إحداثي y لأعلى العقدة.

**Returns:**
float
