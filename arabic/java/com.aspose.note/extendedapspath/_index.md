---
title: "ExtendedApsPath"
second_title: "مرجع Aspose.Note for Java API"
description: "يمثل غلافًا لمسار ApsPath القياسي الذي يمد بعض سلوك الرسم."
type: docs
weight: 28
url: /ar/java/com.aspose.note/extendedapspath/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.ExtendedApsNode](../../com.aspose.note/extendedapsnode)
```
public class ExtendedApsPath extends ExtendedApsNode
```

يمثل غلافًا لـ ApsPath القياسي، الذي يوسع بعض سلوكيات الرسم.
## المنشئات

| المنشئ | الوصف |
| --- | --- |
| [ExtendedApsPath(ApsPath internalApsPath)](#ExtendedApsPath-com.aspose.foundation.rendering.ApsPath-) | ينشئ مثيلاً جديداً من الفئة `ExtendedApsPath`. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | يضيف هذه العقدة إلى `compositeNode` المعطى. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | يطبق تحويل المستوى، محركًا العقدة في مستويي x و y. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | يطبق التحجيم على العقدة. |
| [getBottom()](#getBottom--) | يحصل على الجزء السفلي. |
| [getCopy()](#getCopy--) | ينشئ نسخة كاملة من هذه العقدة. |
| [getTop()](#getTop--) | يحصل على الجزء العلوي. |
### ExtendedApsPath(ApsPath internalApsPath) {#ExtendedApsPath-com.aspose.foundation.rendering.ApsPath-}
```
public ExtendedApsPath(ApsPath internalApsPath)
```


ينشئ مثيلاً جديداً من الفئة `ExtendedApsPath`.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| internalApsPath | com.aspose.foundation.rendering.ApsPath | مسار aps. |

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


يطبق التحجيم على العقدة.

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
### getTop() {#getTop--}
```
public float getTop()
```


يحصل على الجزء العلوي.

**Returns:**
float
