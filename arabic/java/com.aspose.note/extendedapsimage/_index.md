---
title: "ExtendedApsImage"
second_title: "مرجع Aspose.Note for Java API"
description: "يمثل غلافًا لـ ApsImage القياسي الذي يمد بعض سلوكيات الرسم."
type: docs
weight: 25
url: /ar/java/com.aspose.note/extendedapsimage/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.ExtendedApsNode](../../com.aspose.note/extendedapsnode)
```
public class ExtendedApsImage extends ExtendedApsNode
```

يمثل غلافًا لـ ApsImage القياسي، الذي يوسع بعض سلوكيات الرسم.
## المنشئات

| المنشئ | الوصف |
| --- | --- |
| [ExtendedApsImage(ApsImage internalImage)](#ExtendedApsImage-com.aspose.foundation.rendering.ApsImage-) | ينشئ مثيلًا جديدًا للفئة `ExtendedApsImage`. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | يضيف هذه العقدة إلى `compositeNode` المعطى. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | يطبق تحويل المستوى، محركًا العقدة في مستويي x و y. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | يطبق التحجيم على الصورة. |
| [getBottom()](#getBottom--) | يحصل على الجزء السفلي. |
| [getCopy()](#getCopy--) | ينشئ نسخة كاملة من هذه العقدة. |
| [getOrigin()](#getOrigin--) | يحصل على الأصل. |
| [getSize()](#getSize--) | يحصل على الحجم. |
| [getTop()](#getTop--) | يحصل على الجزء العلوي. |
| [isBackground()](#isBackground--) | يحصل على ما إذا كانت الصورة صورة خلفية. |
### ExtendedApsImage(ApsImage internalImage) {#ExtendedApsImage-com.aspose.foundation.rendering.ApsImage-}
```
public ExtendedApsImage(ApsImage internalImage)
```


ينشئ مثيلًا جديدًا للفئة `ExtendedApsImage`.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| internalImage | com.aspose.foundation.rendering.ApsImage | الصورة. |

### addToCompositeNode(ApsCompositeNode compositeNode) {#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-}
```
public void addToCompositeNode(ApsCompositeNode compositeNode)
```


يضيف هذه العقدة إلى `compositeNode` المعطى.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| compositeNode | com.aspose.foundation.rendering.ApsCompositeNode |  |

### applyPlaneTransform(System.Drawing.PointF transformVector) {#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-}
```
public void applyPlaneTransform(System.Drawing.PointF transformVector)
```


يطبق تحويل المستوى، محركًا العقدة في مستويي x و y.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| transformVector | com.aspose.ms.System.Drawing.PointF |  |

### applyScaleTransform(float scaleTransform) {#applyScaleTransform-float-}
```
public void applyScaleTransform(float scaleTransform)
```


يطبق التحجيم على الصورة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| scaleTransform | float | عامل القياس للتحويل. |

### getBottom() {#getBottom--}
```
public float getBottom()
```


يحصل على الجزء السفلي.

**Returns:**
float
### getCopy() {#getCopy--}
```
public ExtendedApsNode getCopy()
```


ينشئ نسخة كاملة من هذه العقدة.

**Returns:**
[ExtendedApsNode](../../com.aspose.note/extendedapsnode) - The `IExtendedApsNode`.
### getOrigin() {#getOrigin--}
```
public System.Drawing.PointF getOrigin()
```


يحصل على الأصل.

**Returns:**
com.aspose.ms.System.Drawing.PointF
### getSize() {#getSize--}
```
public System.Drawing.SizeF getSize()
```


يحصل على الحجم.

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getTop() {#getTop--}
```
public float getTop()
```


يحصل على الجزء العلوي.

**Returns:**
float
### isBackground() {#isBackground--}
```
public final boolean isBackground()
```


يحصل على ما إذا كانت الصورة صورة خلفية.

**Returns:**
boolean
