---
title: "ExtendedApsNode"
second_title: "Aspose.Note for Java API Referansı"
description: "Standart bir ApsNode için sarmalayıcıyı temsil eder ve bazı çizim davranışlarını genişletir."
type: docs
weight: 26
url: /tr/java/com.aspose.note/extendedapsnode/
---

**Inheritance:**
java.lang.Object
```
public abstract class ExtendedApsNode
```

Çizim davranışının bir kısmını genişleten standart ApsNode için bir sarmalayıcıyı temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [ExtendedApsNode()](#ExtendedApsNode--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | Bu düğümü verilen `compositeNode` öğesine ekler. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | Düzlem dönüşümünü uygular, düğümü x ve y düzlemlerinde hareket ettirir. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | Düğüm üzerine ölçeklendirme uygular. |
| [copyAttributes(ApsNode src, ApsNode dst)](#copyAttributes-com.aspose.foundation.rendering.ApsNode-com.aspose.foundation.rendering.ApsNode-) |  |
| [copyAttributes(ApsNodeAttributes src, ApsNodeAttributes dst)](#copyAttributes-com.aspose.foundation.rendering.ApsNodeAttributes-com.aspose.foundation.rendering.ApsNodeAttributes-) |  |
| [getBottom()](#getBottom--) | Düğümün alt kısmının y koordinatını alır veya ayarlar. |
| [getCopy()](#getCopy--) | Bu düğümün tam bir kopyasını oluşturur. |
| [getOrigin()](#getOrigin--) | Düğümün kökenini alır veya ayarlar. |
| [getSize()](#getSize--) | Düğümün boyutunu alır veya ayarlar. |
| [getTop()](#getTop--) | Düğümün üst kısmının y koordinatını alır veya ayarlar. |
### ExtendedApsNode() {#ExtendedApsNode--}
```
public ExtendedApsNode()
```


### addToCompositeNode(ApsCompositeNode compositeNode) {#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-}
```
public abstract void addToCompositeNode(ApsCompositeNode compositeNode)
```


Bu düğümü verilen `compositeNode` öğesine ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| compositeNode | com.aspose.foundation.rendering.ApsCompositeNode |  |

### applyPlaneTransform(System.Drawing.PointF transformVector) {#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-}
```
public abstract void applyPlaneTransform(System.Drawing.PointF transformVector)
```


Düzlem dönüşümünü uygular, düğümü x ve y düzlemlerinde hareket ettirir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| transformVector | com.aspose.ms.System.Drawing.PointF |  |

### applyScaleTransform(float scaleTransform) {#applyScaleTransform-float-}
```
public abstract void applyScaleTransform(float scaleTransform)
```


Düğüm üzerine ölçeklendirme uygular.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| scaleTransform | float | Dönüşüm için ölçek faktörü. |

### copyAttributes(ApsNode src, ApsNode dst) {#copyAttributes-com.aspose.foundation.rendering.ApsNode-com.aspose.foundation.rendering.ApsNode-}
```
public static void copyAttributes(ApsNode src, ApsNode dst)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| src | com.aspose.foundation.rendering.ApsNode |  |
| dst | com.aspose.foundation.rendering.ApsNode |  |

### copyAttributes(ApsNodeAttributes src, ApsNodeAttributes dst) {#copyAttributes-com.aspose.foundation.rendering.ApsNodeAttributes-com.aspose.foundation.rendering.ApsNodeAttributes-}
```
public static void copyAttributes(ApsNodeAttributes src, ApsNodeAttributes dst)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| src | com.aspose.foundation.rendering.ApsNodeAttributes |  |
| dst | com.aspose.foundation.rendering.ApsNodeAttributes |  |

### getBottom() {#getBottom--}
```
public float getBottom()
```


Düğümün alt kısmının y koordinatını alır veya ayarlar.

**Returns:**
float
### getCopy() {#getCopy--}
```
public abstract ExtendedApsNode getCopy()
```


Bu düğümün tam bir kopyasını oluşturur.

**Returns:**
[ExtendedApsNode](../../com.aspose.note/extendedapsnode) - The `!:ExtendedApsNode`.
### getOrigin() {#getOrigin--}
```
public System.Drawing.PointF getOrigin()
```


Düğümün kökenini alır veya ayarlar.

**Returns:**
com.aspose.ms.System.Drawing.PointF
### getSize() {#getSize--}
```
public System.Drawing.SizeF getSize()
```


Düğümün boyutunu alır veya ayarlar.

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getTop() {#getTop--}
```
public float getTop()
```


Düğümün üst kısmının y koordinatını alır veya ayarlar.

**Returns:**
float
