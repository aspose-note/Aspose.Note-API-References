---
title: "ExtendedCompositeNode"
second_title: "مرجع Aspose.Note for Java API"
description: "يجمع عدة مثيلات IExtendedApsNode."
type: docs
weight: 29
url: /ar/java/com.aspose.note/extendedcompositenode/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.ExtendedApsNode](../../com.aspose.note/extendedapsnode)
```
public class ExtendedCompositeNode extends ExtendedApsNode
```

يجمع عدة مثيلات `IExtendedApsNode`.
## المنشئات

| المنشئ | الوصف |
| --- | --- |
| [ExtendedCompositeNode()](#ExtendedCompositeNode--) | ينشئ مثيلًا جديدًا من الفئة `ExtendedCompositeNode`. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [add(ExtendedApsNode extendedApsNode)](#add-com.aspose.note.ExtendedApsNode-) | يضيف `extendedApsNode` إلى القائمة الداخلية للعناصر. |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | يضيف هذه العقدة إلى `compositeNode` المعطى. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | يطبق تحويل المستوى، محركًا العقدة في مستويي x و y. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | يطبق التحجيم على العقدة. |
| [getApsNodes()](#getApsNodes--) | يحصل على جميع مثيلات `IExtendedApsNode` المدمجة في هذا `ExtendedCompositeNode`. |
| [getCopy()](#getCopy--) | ينشئ نسخة كاملة من هذه العقدة. |
### ExtendedCompositeNode() {#ExtendedCompositeNode--}
```
public ExtendedCompositeNode()
```


ينشئ مثيلًا جديدًا من الفئة `ExtendedCompositeNode`.

### add(ExtendedApsNode extendedApsNode) {#add-com.aspose.note.ExtendedApsNode-}
```
public final void add(ExtendedApsNode extendedApsNode)
```


يضيف `extendedApsNode` إلى القائمة الداخلية للعناصر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| extendedApsNode | [ExtendedApsNode](../../com.aspose.note/extendedapsnode) |  |

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

### getApsNodes() {#getApsNodes--}
```
public final System.Collections.Generic.IGenericCollection<ExtendedApsNode> getApsNodes()
```


يحصل على جميع مثيلات `IExtendedApsNode` المدمجة في هذا `ExtendedCompositeNode`.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericCollection&lt;com.aspose.note.ExtendedApsNode&gt;
### getCopy() {#getCopy--}
```
public ExtendedApsNode getCopy()
```


ينشئ نسخة كاملة من هذه العقدة.

**Returns:**
[ExtendedApsNode](../../com.aspose.note/extendedapsnode) - The `IExtendedApsNode`.
