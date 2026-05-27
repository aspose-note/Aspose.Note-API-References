---
title: "ExtendedCompositeNode"
second_title: "Aspose.Note for Java API Referansı"
description: "Birçok IExtendedApsNode örneğini birleştirir."
type: docs
weight: 29
url: /tr/java/com.aspose.note/extendedcompositenode/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.ExtendedApsNode](../../com.aspose.note/extendedapsnode)
```
public class ExtendedCompositeNode extends ExtendedApsNode
```

Birçok `IExtendedApsNode` örneğini birleştirir.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [ExtendedCompositeNode()](#ExtendedCompositeNode--) | `ExtendedCompositeNode` sınıfının yeni bir örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [add(ExtendedApsNode extendedApsNode)](#add-com.aspose.note.ExtendedApsNode-) | `extendedApsNode` öğesini iç düğüm listesine ekler. |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | Bu düğümü verilen `compositeNode` öğesine ekler. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | Düzlem dönüşümünü uygular, düğümü x ve y düzlemlerinde hareket ettirir. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | Düğüm üzerine ölçeklendirme uygular. |
| [getApsNodes()](#getApsNodes--) | Bu `ExtendedCompositeNode` içinde birleştirilen tüm `IExtendedApsNode` örneklerini alır. |
| [getCopy()](#getCopy--) | Bu düğümün tam bir kopyasını oluşturur. |
### ExtendedCompositeNode() {#ExtendedCompositeNode--}
```
public ExtendedCompositeNode()
```


`ExtendedCompositeNode` sınıfının yeni bir örneğini başlatır.

### add(ExtendedApsNode extendedApsNode) {#add-com.aspose.note.ExtendedApsNode-}
```
public final void add(ExtendedApsNode extendedApsNode)
```


`extendedApsNode` öğesini iç düğüm listesine ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| extendedApsNode | [ExtendedApsNode](../../com.aspose.note/extendedapsnode) |  |

### addToCompositeNode(ApsCompositeNode compositeNode) {#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-}
```
public void addToCompositeNode(ApsCompositeNode compositeNode)
```


Bu düğümü verilen `compositeNode` öğesine ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| compositeNode | com.aspose.foundation.rendering.ApsCompositeNode |  |

### applyPlaneTransform(System.Drawing.PointF transformVector) {#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-}
```
public void applyPlaneTransform(System.Drawing.PointF transformVector)
```


Düzlem dönüşümünü uygular, düğümü x ve y düzlemlerinde hareket ettirir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| transformVector | com.aspose.ms.System.Drawing.PointF |  |

### applyScaleTransform(float scaleTransform) {#applyScaleTransform-float-}
```
public void applyScaleTransform(float scaleTransform)
```


Düğüm üzerine ölçeklendirme uygular.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| scaleTransform | float | Dönüşüm için ölçek faktörü. |

### getApsNodes() {#getApsNodes--}
```
public final System.Collections.Generic.IGenericCollection<ExtendedApsNode> getApsNodes()
```


Bu `ExtendedCompositeNode` içinde birleştirilen tüm `IExtendedApsNode` örneklerini alır.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericCollection&lt;com.aspose.note.ExtendedApsNode&gt;
### getCopy() {#getCopy--}
```
public ExtendedApsNode getCopy()
```


Bu düğümün tam bir kopyasını oluşturur.

**Returns:**
[ExtendedApsNode](../../com.aspose.note/extendedapsnode) - The `IExtendedApsNode`.
