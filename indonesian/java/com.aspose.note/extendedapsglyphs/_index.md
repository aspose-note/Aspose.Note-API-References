---
title: "ExtendedApsGlyphs"
second_title: "Referensi API Aspose.Note untuk Java"
description: "Mewakili pembungkus untuk ApsGlyphs standar yang memperluas beberapa perilaku menggambar."
type: docs
weight: 24
url: /id/java/com.aspose.note/extendedapsglyphs/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.ExtendedApsNode](../../com.aspose.note/extendedapsnode)
```
public class ExtendedApsGlyphs extends ExtendedApsNode
```

Mewakili pembungkus untuk ApsGlyphs standar, yang memperluas sebagian perilaku menggambar.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [ExtendedApsGlyphs(ApsGlyphs internalGlyphs)](#ExtendedApsGlyphs-com.aspose.foundation.rendering.ApsGlyphs-) | Menginisialisasi instance baru dari kelas `ExtendedApsGlyphs`. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | Menambahkan node ini ke `compositeNode` yang diberikan. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | Menerapkan transformasi bidang, memindahkan node pada bidang x dan y. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | Menerapkan skala pada glyphs. |
| [getBottom()](#getBottom--) | Mendapatkan bagian bawah glyphs. |
| [getCopy()](#getCopy--) | Mendapatkan salinan glyphs. |
| [getOrigin()](#getOrigin--) | Mendapatkan asal. |
| [getSize()](#getSize--) | Mendapatkan ukuran. |
| [getTop()](#getTop--) | Mendapatkan bagian atas. |
### ExtendedApsGlyphs(ApsGlyphs internalGlyphs) {#ExtendedApsGlyphs-com.aspose.foundation.rendering.ApsGlyphs-}
```
public ExtendedApsGlyphs(ApsGlyphs internalGlyphs)
```


Menginisialisasi instance baru dari kelas `ExtendedApsGlyphs`.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| internalGlyphs | com.aspose.foundation.rendering.ApsGlyphs | Sebuah glyph aps asli. |

### addToCompositeNode(ApsCompositeNode compositeNode) {#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-}
```
public void addToCompositeNode(ApsCompositeNode compositeNode)
```


Menambahkan node ini ke `compositeNode` yang diberikan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| compositeNode | com.aspose.foundation.rendering.ApsCompositeNode |  |

### applyPlaneTransform(System.Drawing.PointF transformVector) {#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-}
```
public void applyPlaneTransform(System.Drawing.PointF transformVector)
```


Menerapkan transformasi bidang, memindahkan node pada bidang x dan y.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| transformVector | com.aspose.ms.System.Drawing.PointF |  |

### applyScaleTransform(float scaleTransform) {#applyScaleTransform-float-}
```
public void applyScaleTransform(float scaleTransform)
```


Menerapkan skala pada glyphs.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| scaleTransform | float | Faktor skala untuk transformasi. |

### getBottom() {#getBottom--}
```
public float getBottom()
```


Mendapatkan bagian bawah glyphs.

**Returns:**
float
### getCopy() {#getCopy--}
```
public ExtendedApsNode getCopy()
```


Mendapatkan salinan glyphs.

**Returns:**
[ExtendedApsNode](../../com.aspose.note/extendedapsnode) - The `IExtendedApsNode`.
### getOrigin() {#getOrigin--}
```
public System.Drawing.PointF getOrigin()
```


Mendapatkan asal.

**Returns:**
com.aspose.ms.System.Drawing.PointF
### getSize() {#getSize--}
```
public System.Drawing.SizeF getSize()
```


Mendapatkan ukuran.

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getTop() {#getTop--}
```
public float getTop()
```


Mendapatkan bagian atas.

**Returns:**
float
