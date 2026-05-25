---
title: "ExtendedApsPage"
second_title: "Referensi API Aspose.Note untuk Java"
description: "Mewakili pembungkus untuk ApsGlyphs standar yang memperluas beberapa perilaku menggambar."
type: docs
weight: 27
url: /id/java/com.aspose.note/extendedapspage/
---

**Inheritance:**
java.lang.Object, com.aspose.foundation.rendering.ApsNode, com.aspose.foundation.rendering.ApsCompositeNode, com.aspose.foundation.rendering.ApsPage

**All Implemented Interfaces:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerable
```
public class ExtendedApsPage extends ApsPage implements System.Collections.Generic.IGenericEnumerable<ApsNode>
```

Mewakili pembungkus untuk ApsGlyphs standar, yang memperluas sebagian perilaku menggambar.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [ExtendedApsPage(System.Drawing.SizeF pageSize, float pageStartInNotePage, Margin margin)](#ExtendedApsPage-com.aspose.ms.System.Drawing.SizeF-float-com.aspose.foundation.layout.Margin-) | Menginisialisasi sebuah instance baru dari kelas `ExtendedApsPage`. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getContentSize()](#getContentSize--) | Mendapatkan ukuran halaman tanpa margin. |
| [getMargin()](#getMargin--) | Mendapatkan margin halaman ini. |
| [getPageEndInNotePage()](#getPageEndInNotePage--) | Mendapatkan posisi akhir halaman, dalam halaman MS OneNote, ketika satu halaman MS OneNote dibagi menjadi beberapa halaman aps. |
| [getPageSize()](#getPageSize--) | Mendapatkan ukuran halaman akhir. |
| [getPageStartInNotePage()](#getPageStartInNotePage--) | Mendapatkan posisi awal halaman dalam halaman MS OneNote, ketika satu halaman MS OneNote dibagi menjadi beberapa halaman aps. |
| [iterator()](#iterator--) | Mengembalikan enumerator yang mengiterasi semua node dari halaman ini. |
| [iterator_Rename_Namesake()](#iterator-Rename-Namesake--) | Enumerator get. |
### ExtendedApsPage(System.Drawing.SizeF pageSize, float pageStartInNotePage, Margin margin) {#ExtendedApsPage-com.aspose.ms.System.Drawing.SizeF-float-com.aspose.foundation.layout.Margin-}
```
public ExtendedApsPage(System.Drawing.SizeF pageSize, float pageStartInNotePage, Margin margin)
```


Menginisialisasi sebuah instance baru dari kelas `ExtendedApsPage`.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| pageSize | com.aspose.ms.System.Drawing.SizeF | Ukuran halaman. |
| pageStartInNotePage | float | Awal halaman dalam halaman MS OneNote asli. |
| margin | com.aspose.foundation.layout.Margin | Margin halaman yang diperluas. |

### getContentSize() {#getContentSize--}
```
public System.Drawing.SizeF getContentSize()
```


Mendapatkan ukuran halaman tanpa margin.

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getMargin() {#getMargin--}
```
public Margin getMargin()
```


Mendapatkan margin halaman ini.

**Returns:**
com.aspose.foundation.layout.Margin
### getPageEndInNotePage() {#getPageEndInNotePage--}
```
public float getPageEndInNotePage()
```


Mendapatkan posisi akhir halaman, dalam halaman MS OneNote, ketika satu halaman MS OneNote dibagi menjadi beberapa halaman aps.

**Returns:**
float
### getPageSize() {#getPageSize--}
```
public System.Drawing.SizeF getPageSize()
```


Mendapatkan ukuran halaman akhir.

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getPageStartInNotePage() {#getPageStartInNotePage--}
```
public float getPageStartInNotePage()
```


Mendapatkan posisi awal halaman dalam halaman MS OneNote, ketika satu halaman MS OneNote dibagi menjadi beberapa halaman aps.

**Returns:**
float
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<ApsNode> iterator()
```


Mengembalikan enumerator yang mengiterasi semua node dari halaman ini.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.foundation.rendering.ApsNode&gt; - `IEnumerator`.
### iterator_Rename_Namesake() {#iterator-Rename-Namesake--}
```
public System.Collections.IEnumerator iterator_Rename_Namesake()
```


Enumerator get.

**Returns:**
com.aspose.ms.System.Collections.IEnumerator - `IEnumerator`.
