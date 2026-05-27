---
title: "ExtendedApsImage"
second_title: "Aspose.Note for Java API Referansı"
description: "Standart ApsImage için bazı çizim davranışlarını genişleten bir sarmalayıcıyı temsil eder."
type: docs
weight: 25
url: /tr/java/com.aspose.note/extendedapsimage/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.ExtendedApsNode](../../com.aspose.note/extendedapsnode)
```
public class ExtendedApsImage extends ExtendedApsNode
```

Çizim davranışının bir kısmını genişleten standart ApsImage için bir sarmalayıcıyı temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [ExtendedApsImage(ApsImage internalImage)](#ExtendedApsImage-com.aspose.foundation.rendering.ApsImage-) | `ExtendedApsImage` sınıfının yeni bir örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | Bu düğümü verilen `compositeNode` öğesine ekler. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | Düzlem dönüşümünü uygular, düğümü x ve y düzlemlerinde hareket ettirir. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | Görüntüye ölçekleme uygular. |
| [getBottom()](#getBottom--) | Alt kısmı alır. |
| [getCopy()](#getCopy--) | Bu düğümün tam bir kopyasını oluşturur. |
| [getOrigin()](#getOrigin--) | Orijini alır. |
| [getSize()](#getSize--) | Boyutu alır. |
| [getTop()](#getTop--) | Üst kısmı alır. |
| [isBackground()](#isBackground--) | Görselin arka plan görseli olup olmadığını alır. |
### ExtendedApsImage(ApsImage internalImage) {#ExtendedApsImage-com.aspose.foundation.rendering.ApsImage-}
```
public ExtendedApsImage(ApsImage internalImage)
```


`ExtendedApsImage` sınıfının yeni bir örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| internalImage | com.aspose.foundation.rendering.ApsImage | Görüntü. |

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


Görüntüye ölçekleme uygular.

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
### isBackground() {#isBackground--}
```
public final boolean isBackground()
```


Görselin arka plan görseli olup olmadığını alır.

**Returns:**
boolean
