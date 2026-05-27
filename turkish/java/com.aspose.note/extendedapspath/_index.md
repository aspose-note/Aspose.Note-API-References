---
title: "ExtendedApsPath"
second_title: "Aspose.Note for Java API Referansı"
description: "Standart ApsPath için, bazı çizim davranışlarını genişleten bir sarmalayıcıyı temsil eder."
type: docs
weight: 28
url: /tr/java/com.aspose.note/extendedapspath/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.ExtendedApsNode](../../com.aspose.note/extendedapsnode)
```
public class ExtendedApsPath extends ExtendedApsNode
```

Çizim davranışının bir kısmını genişleten standart ApsPath için bir sarmalayıcıyı temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [ExtendedApsPath(ApsPath internalApsPath)](#ExtendedApsPath-com.aspose.foundation.rendering.ApsPath-) | `ExtendedApsPath` sınıfının yeni bir örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | Bu düğümü verilen `compositeNode` öğesine ekler. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | Düzlem dönüşümünü uygular, düğümü x ve y düzlemlerinde hareket ettirir. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | Düğüm üzerine ölçeklendirme uygular. |
| [getBottom()](#getBottom--) | Alt kısmı alır. |
| [getCopy()](#getCopy--) | Bu düğümün tam bir kopyasını oluşturur. |
| [getTop()](#getTop--) | Üst kısmı alır. |
### ExtendedApsPath(ApsPath internalApsPath) {#ExtendedApsPath-com.aspose.foundation.rendering.ApsPath-}
```
public ExtendedApsPath(ApsPath internalApsPath)
```


`ExtendedApsPath` sınıfının yeni bir örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| internalApsPath | com.aspose.foundation.rendering.ApsPath | Aps yolu. |

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

### getBottom() {#getBottom--}
```
public float getBottom()
```


Alt kısmı alır.

**Returns:**
float
### getCopy() {#getCopy--}
```
public ExtendedApsNode getCopy()
```


Bu düğümün tam bir kopyasını oluşturur.

**Returns:**
[ExtendedApsNode](../../com.aspose.note/extendedapsnode) - The `IExtendedApsNode`.
### getTop() {#getTop--}
```
public float getTop()
```


Üst kısmı alır.

**Returns:**
float
