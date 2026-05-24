---
title: "ExtendedApsGlyphs"
second_title: "مرجع Aspose.Note for Java API"
description: "يمثل غلافًا لـ ApsGlyphs القياسي الذي يوسع بعض سلوكيات الرسم."
type: docs
weight: 24
url: /ar/java/com.aspose.note/extendedapsglyphs/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.ExtendedApsNode](../../com.aspose.note/extendedapsnode)
```
public class ExtendedApsGlyphs extends ExtendedApsNode
```

يمثل غلافًا لـ ApsGlyphs القياسي، الذي يوسع بعض سلوكيات الرسم.
## المنشئات

| المنشئ | الوصف |
| --- | --- |
| [ExtendedApsGlyphs(ApsGlyphs internalGlyphs)](#ExtendedApsGlyphs-com.aspose.foundation.rendering.ApsGlyphs-) | يُنشئ مثيلاً جديدًا من الفئة `ExtendedApsGlyphs`. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | يضيف هذه العقدة إلى `compositeNode` المعطى. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | يطبق تحويل المستوى، محركًا العقدة في مستويي x و y. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | يطبق التحجيم على الرموز. |
| [getBottom()](#getBottom--) | يحصل على الجزء السفلي من الرموز. |
| [getCopy()](#getCopy--) | يحصل على نسخة من الرموز. |
| [getOrigin()](#getOrigin--) | يحصل على الأصل. |
| [getSize()](#getSize--) | يحصل على الحجم. |
| [getTop()](#getTop--) | يحصل على الجزء العلوي. |
### ExtendedApsGlyphs(ApsGlyphs internalGlyphs) {#ExtendedApsGlyphs-com.aspose.foundation.rendering.ApsGlyphs-}
```
public ExtendedApsGlyphs(ApsGlyphs internalGlyphs)
```


يُنشئ مثيلاً جديدًا من الفئة `ExtendedApsGlyphs`.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| internalGlyphs | com.aspose.foundation.rendering.ApsGlyphs | رموز aps الأصلية. |

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


يطبق التحجيم على الرموز.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| scaleTransform | float | عامل القياس للتحويل. |

### getBottom() {#getBottom--}
```
public float getBottom()
```


يحصل على الجزء السفلي من الرموز.

**Returns:**
float
### getCopy() {#getCopy--}
```
public ExtendedApsNode getCopy()
```


يحصل على نسخة من الرموز.

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
