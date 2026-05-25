---
title: "ExtendedCompositeNode"
second_title: "Referensi API Aspose.Note untuk Java"
description: "Menggabungkan beberapa instance IExtendedApsNode."
type: docs
weight: 29
url: /id/java/com.aspose.note/extendedcompositenode/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.ExtendedApsNode](../../com.aspose.note/extendedapsnode)
```
public class ExtendedCompositeNode extends ExtendedApsNode
```

Menggabungkan beberapa instance `IExtendedApsNode`.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [ExtendedCompositeNode()](#ExtendedCompositeNode--) | Menginisialisasi instance baru dari kelas `ExtendedCompositeNode`. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [add(ExtendedApsNode extendedApsNode)](#add-com.aspose.note.ExtendedApsNode-) | Menambahkan `extendedApsNode` ke daftar internal node. |
| [addToCompositeNode(ApsCompositeNode compositeNode)](#addToCompositeNode-com.aspose.foundation.rendering.ApsCompositeNode-) | Menambahkan node ini ke `compositeNode` yang diberikan. |
| [applyPlaneTransform(System.Drawing.PointF transformVector)](#applyPlaneTransform-com.aspose.ms.System.Drawing.PointF-) | Menerapkan transformasi bidang, memindahkan node pada bidang x dan y. |
| [applyScaleTransform(float scaleTransform)](#applyScaleTransform-float-) | Menerapkan skala pada node. |
| [getApsNodes()](#getApsNodes--) | Mendapatkan semua instance `IExtendedApsNode` yang digabungkan ke dalam `ExtendedCompositeNode` ini. |
| [getCopy()](#getCopy--) | Membuat salinan penuh dari node ini. |
### ExtendedCompositeNode() {#ExtendedCompositeNode--}
```
public ExtendedCompositeNode()
```


Menginisialisasi instance baru dari kelas `ExtendedCompositeNode`.

### add(ExtendedApsNode extendedApsNode) {#add-com.aspose.note.ExtendedApsNode-}
```
public final void add(ExtendedApsNode extendedApsNode)
```


Menambahkan `extendedApsNode` ke daftar internal node.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| extendedApsNode | [ExtendedApsNode](../../com.aspose.note/extendedapsnode) |  |

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

### getApsNodes() {#getApsNodes--}
```
public final System.Collections.Generic.IGenericCollection<ExtendedApsNode> getApsNodes()
```


Mendapatkan semua instance `IExtendedApsNode` yang digabungkan ke dalam `ExtendedCompositeNode` ini.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericCollection&lt;com.aspose.note.ExtendedApsNode&gt;
### getCopy() {#getCopy--}
```
public ExtendedApsNode getCopy()
```


Membuat salinan penuh dari node ini.

**Returns:**
[ExtendedApsNode](../../com.aspose.note/extendedapsnode) - The `IExtendedApsNode`.
