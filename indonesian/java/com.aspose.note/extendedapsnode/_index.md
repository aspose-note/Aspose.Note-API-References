---
title: "ExtendedApsNode"
second_title: "Referensi API Aspose.Note untuk Java"
description: "Mewakili pembungkus untuk ApsNode standar yang memperluas beberapa perilaku menggambar."
type: docs
weight: 26
url: /id/java/com.aspose.note/extendedapsnode/
---

**Inheritance:**
java.lang.Object
```
public abstract class ExtendedApsNode
```

Mewakili pembungkus untuk ApsNode standar, yang memperluas sebagian perilaku menggambar.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [ExtendedApsNode()](#ExtendedApsNode--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | Menambahkan node ini ke `compositeNode` yang diberikan. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | Menerapkan transformasi bidang, memindahkan node pada bidang x dan y. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | Menerapkan skala pada node. |
| [copyAttributes(ApsNode src, ApsNode dst)](#copyAttributes-com.aspose.foundation.rendering.ApsNode-com.aspose.foundation.rendering.ApsNode-) |  |
| [copyAttributes(ApsNodeAttributes src, ApsNodeAttributes dst)](#copyAttributes-com.aspose.foundation.rendering.ApsNodeAttributes-com.aspose.foundation.rendering.ApsNodeAttributes-) |  |
| [getBottom()](#getBottom--) | Mendapatkan atau mengatur koordinat y dari bagian bawah node. |
| [getCopy()](#getCopy--) | Membuat salinan penuh dari node ini. |
| [getOrigin()](#getOrigin--) | Mendapatkan atau mengatur asal node. |
| [getSize()](#getSize--) | Mendapatkan atau mengatur ukuran node. |
| [getTop()](#getTop--) | Mendapatkan atau mengatur koordinat y bagian atas node. |
### ExtendedApsNode() {#ExtendedApsNode--}
```
public ExtendedApsNode()
```


### addToCompositeNode(ApsCompositeNode compositeNode) {#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-}
```
public abstract void addToCompositeNode(ApsCompositeNode compositeNode)
```


Menambahkan node ini ke `compositeNode` yang diberikan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| compositeNode | com.aspose.foundation.rendering.ApsCompositeNode |  |

### applyPlaneTransform(System.Drawing.PointF transformVector) {#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-}
```
public abstract void applyPlaneTransform(System.Drawing.PointF transformVector)
```


Menerapkan transformasi bidang, memindahkan node pada bidang x dan y.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| transformVector | com.aspose.ms.System.Drawing.PointF |  |

### applyScaleTransform(float scaleTransform) {#applyScaleTransform-float-}
```
public abstract void applyScaleTransform(float scaleTransform)
```


Menerapkan skala pada node.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| scaleTransform | float | Faktor skala untuk transformasi. |

### copyAttributes(ApsNode src, ApsNode dst) {#copyAttributes-com.aspose.foundation.rendering.ApsNode-com.aspose.foundation.rendering.ApsNode-}
```
public static void copyAttributes(ApsNode src, ApsNode dst)
```




**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| src | com.aspose.foundation.rendering.ApsNode |  |
| dst | com.aspose.foundation.rendering.ApsNode |  |

### copyAttributes(ApsNodeAttributes src, ApsNodeAttributes dst) {#copyAttributes-com.aspose.foundation.rendering.ApsNodeAttributes-com.aspose.foundation.rendering.ApsNodeAttributes-}
```
public static void copyAttributes(ApsNodeAttributes src, ApsNodeAttributes dst)
```




**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| src | com.aspose.foundation.rendering.ApsNodeAttributes |  |
| dst | com.aspose.foundation.rendering.ApsNodeAttributes |  |

### getBottom() {#getBottom--}
```
public float getBottom()
```


Mendapatkan atau mengatur koordinat y dari bagian bawah node.

**Returns:**
float
### getCopy() {#getCopy--}
```
public abstract ExtendedApsNode getCopy()
```


Membuat salinan penuh dari node ini.

**Returns:**
[ExtendedApsNode](../../com.aspose.note/extendedapsnode) - The `!:ExtendedApsNode`.
### getOrigin() {#getOrigin--}
```
public System.Drawing.PointF getOrigin()
```


Mendapatkan atau mengatur asal node.

**Returns:**
com.aspose.ms.System.Drawing.PointF
### getSize() {#getSize--}
```
public System.Drawing.SizeF getSize()
```


Mendapatkan atau mengatur ukuran node.

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getTop() {#getTop--}
```
public float getTop()
```


Mendapatkan atau mengatur koordinat y bagian atas node.

**Returns:**
float
