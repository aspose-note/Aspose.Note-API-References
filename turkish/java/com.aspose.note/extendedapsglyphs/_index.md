---
title: "ExtendedApsGlyphs"
second_title: "Aspose.Note for Java API Referansı"
description: "Standart ApsGlyphs için bazı çizim davranışlarını genişleten bir sarmalayıcıyı temsil eder."
type: docs
weight: 24
url: /tr/java/com.aspose.note/extendedapsglyphs/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.ExtendedApsNode](../../com.aspose.note/extendedapsnode)
```
public class ExtendedApsGlyphs extends ExtendedApsNode
```

Çizim davranışının bir kısmını genişleten standart ApsGlyphs için bir sarmalayıcıyı temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [ExtendedApsGlyphs(ApsGlyphs internalGlyphs)](#ExtendedApsGlyphs-com.aspose.foundation.rendering.ApsGlyphs-) | Yeni bir `ExtendedApsGlyphs` sınıfının örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | Bu düğümü verilen `compositeNode` öğesine ekler. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | Düzlem dönüşümünü uygular, düğümü x ve y düzlemlerinde hareket ettirir. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | Gliflere ölçekleme uygular. |
| [getBottom()](#getBottom--) | Gliflerin alt kısmını alır. |
| [getCopy()](#getCopy--) | Gliflerin bir kopyasını alır. |
| [getOrigin()](#getOrigin--) | Orijini alır. |
| [getSize()](#getSize--) | Boyutu alır. |
| [getTop()](#getTop--) | Üst kısmı alır. |
### ExtendedApsGlyphs(ApsGlyphs internalGlyphs) {#ExtendedApsGlyphs-com.aspose.foundation.rendering.ApsGlyphs-}
```
public ExtendedApsGlyphs(ApsGlyphs internalGlyphs)
```


Yeni bir `ExtendedApsGlyphs` sınıfının örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| internalGlyphs | com.aspose.foundation.rendering.ApsGlyphs | Orijinal aps glifleri. |

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


Gliflere ölçekleme uygular.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| scaleTransform | float | Dönüşüm için ölçek faktörü. |

### getBottom() {#getBottom--}
```
public float getBottom()
```


Gliflerin alt kısmını alır.

**Returns:**
float
### getCopy() {#getCopy--}
```
public ExtendedApsNode getCopy()
```


Gliflerin bir kopyasını alır.

**Returns:**
[ExtendedApsNode](../../com.aspose.note/extendedapsnode) - The `IExtendedApsNode`.
### getOrigin() {#getOrigin--}
```
public System.Drawing.PointF getOrigin()
```


Orijini alır.

**Returns:**
com.aspose.ms.System.Drawing.PointF
### getSize() {#getSize--}
```
public System.Drawing.SizeF getSize()
```


Boyutu alır.

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getTop() {#getTop--}
```
public float getTop()
```


Üst kısmı alır.

**Returns:**
float
