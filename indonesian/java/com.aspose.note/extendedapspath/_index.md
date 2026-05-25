---
title: "ExtendedApsPath"
second_title: "Referensi API Aspose.Note untuk Java"
description: "Mewakili pembungkus untuk ApsPath standar yang memperluas beberapa perilaku menggambar."
type: docs
weight: 28
url: /id/java/com.aspose.note/extendedapspath/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.ExtendedApsNode](../../com.aspose.note/extendedapsnode)
```
public class ExtendedApsPath extends ExtendedApsNode
```

Mewakili pembungkus untuk ApsPath standar, yang memperluas sebagian perilaku menggambar.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [ExtendedApsPath(ApsPath internalApsPath)](#ExtendedApsPath-com.aspose.foundation.rendering.ApsPath-) | Menginisialisasi instance baru dari kelas `ExtendedApsPath`. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | Menambahkan node ini ke `compositeNode` yang diberikan. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | Menerapkan transformasi bidang, memindahkan node pada bidang x dan y. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | Menerapkan skala pada node. |
| [getBottom()](#getBottom--) | Mendapatkan bagian bawah. |
| [getCopy()](#getCopy--) | Membuat salinan penuh dari node ini. |
| [getTop()](#getTop--) | Mendapatkan bagian atas. |
### ExtendedApsPath(ApsPath internalApsPath) {#ExtendedApsPath-com.aspose.foundation.rendering.ApsPath-}
```
public ExtendedApsPath(ApsPath internalApsPath)
```


Menginisialisasi instance baru dari kelas `ExtendedApsPath`.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| internalApsPath | com.aspose.foundation.rendering.ApsPath | Jalur aps. |

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


Menerapkan skala pada node.

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
### getTop() {#getTop--}
```
public float getTop()
```


Mendapatkan bagian atas.

**Returns:**
float
