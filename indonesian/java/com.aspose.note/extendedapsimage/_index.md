---
title: "ExtendedApsImage"
second_title: "Referensi API Aspose.Note untuk Java"
description: "Mewakili pembungkus untuk ApsImage standar yang memperluas beberapa perilaku menggambar."
type: docs
weight: 25
url: /id/java/com.aspose.note/extendedapsimage/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.ExtendedApsNode](../../com.aspose.note/extendedapsnode)
```
public class ExtendedApsImage extends ExtendedApsNode
```

Mewakili pembungkus untuk ApsImage standar, yang memperluas sebagian perilaku menggambar.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [ExtendedApsImage(ApsImage internalImage)](#ExtendedApsImage-com.aspose.foundation.rendering.ApsImage-) | Menginisialisasi instance baru dari kelas `ExtendedApsImage`. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | Menambahkan node ini ke `compositeNode` yang diberikan. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | Menerapkan transformasi bidang, memindahkan node pada bidang x dan y. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | Menerapkan skala pada gambar. |
| [getBottom()](#getBottom--) | Mendapatkan bagian bawah. |
| [getCopy()](#getCopy--) | Membuat salinan penuh dari node ini. |
| [getOrigin()](#getOrigin--) | Mendapatkan asal. |
| [getSize()](#getSize--) | Mendapatkan ukuran. |
| [getTop()](#getTop--) | Mendapatkan bagian atas. |
| [isBackground()](#isBackground--) | Mendapatkan apakah gambar merupakan gambar latar belakang. |
### ExtendedApsImage(ApsImage internalImage) {#ExtendedApsImage-com.aspose.foundation.rendering.ApsImage-}
```
public ExtendedApsImage(ApsImage internalImage)
```


Menginisialisasi instance baru dari kelas `ExtendedApsImage`.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| internalImage | com.aspose.foundation.rendering.ApsImage | Gambar tersebut. |

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


Menerapkan skala pada gambar.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| scaleTransform | float | Faktor skala untuk transformasi. |

### getBottom() {#getBottom--}
```
public float getBottom()
```


Mendapatkan bagian bawah.

**Returns:**
float
### getCopy() {#getCopy--}
```
public ExtendedApsNode getCopy()
```


Membuat salinan penuh dari node ini.

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
### isBackground() {#isBackground--}
```
public final boolean isBackground()
```


Mendapatkan apakah gambar merupakan gambar latar belakang.

**Returns:**
boolean
