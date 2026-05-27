---
title: "ExtendedApsPage"
second_title: "Aspose.Note for Java API Referansı"
description: "Standart ApsGlyphs için bir sarmalayıcı temsil eder ve bazı çizim davranışlarını genişletir."
type: docs
weight: 27
url: /tr/java/com.aspose.note/extendedapspage/
---

**Inheritance:**
java.lang.Object, com.aspose.foundation.rendering.ApsNode, com.aspose.foundation.rendering.ApsCompositeNode, com.aspose.foundation.rendering.ApsPage

**All Implemented Interfaces:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerable
```
public class ExtendedApsPage extends ApsPage implements System.Collections.Generic.IGenericEnumerable<ApsNode>
```

Çizim davranışının bir kısmını genişleten standart ApsGlyphs için bir sarmalayıcıyı temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [ExtendedApsPage(System.Drawing.SizeF pageSize, float pageStartInNotePage, Margin margin)](#ExtendedApsPage-com.aspose.ms.System.Drawing.SizeF-float-com.aspose.foundation.layout.Margin-) | `ExtendedApsPage` sınıfının yeni bir örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getContentSize()](#getContentSize--) | Kenar boşlukları hariç sayfa boyutunu alır. |
| [getMargin()](#getMargin--) | Bu sayfanın kenar boşluğunu alır. |
| [getPageEndInNotePage()](#getPageEndInNotePage--) | Bir MS OneNote sayfası birden fazla aps Sayfasına bölündüğünde, MS OneNote sayfasındaki sayfa sonunun konumunu alır. |
| [getPageSize()](#getPageSize--) | Son sayfa boyutunu alır. |
| [getPageStartInNotePage()](#getPageStartInNotePage--) | Bir MS OneNote sayfası birden fazla aps Sayfasına bölündüğünde, MS OneNote sayfasındaki sayfa başlangıcının konumunu alır. |
| [iterator()](#iterator--) | Bu sayfadaki tüm düğümler üzerinde yineleme yapan enumeratörü döndürür. |
| [iterator_Rename_Namesake()](#iterator-Rename-Namesake--) | Enumeratörü al. |
### ExtendedApsPage(System.Drawing.SizeF pageSize, float pageStartInNotePage, Margin margin) {#ExtendedApsPage-com.aspose.ms.System.Drawing.SizeF-float-com.aspose.foundation.layout.Margin-}
```
public ExtendedApsPage(System.Drawing.SizeF pageSize, float pageStartInNotePage, Margin margin)
```


`ExtendedApsPage` sınıfının yeni bir örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pageSize | com.aspose.ms.System.Drawing.SizeF | Sayfa boyutu. |
| pageStartInNotePage | float | Orijinal MS OneNote sayfasındaki sayfa başlangıcı. |
| margin | com.aspose.foundation.layout.Margin | Genişletilmiş sayfa kenarı. |

### getContentSize() {#getContentSize--}
```
public System.Drawing.SizeF getContentSize()
```


Kenar boşlukları hariç sayfa boyutunu alır.

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getMargin() {#getMargin--}
```
public Margin getMargin()
```


Bu sayfanın kenar boşluğunu alır.

**Returns:**
com.aspose.foundation.layout.Margin
### getPageEndInNotePage() {#getPageEndInNotePage--}
```
public float getPageEndInNotePage()
```


Bir MS OneNote sayfası birden fazla aps Sayfasına bölündüğünde, MS OneNote sayfasındaki sayfa sonunun konumunu alır.

**Returns:**
float
### getPageSize() {#getPageSize--}
```
public System.Drawing.SizeF getPageSize()
```


Son sayfa boyutunu alır.

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getPageStartInNotePage() {#getPageStartInNotePage--}
```
public float getPageStartInNotePage()
```


Bir MS OneNote sayfası birden fazla aps Sayfasına bölündüğünde, MS OneNote sayfasındaki sayfa başlangıcının konumunu alır.

**Returns:**
float
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<ApsNode> iterator()
```


Bu sayfadaki tüm düğümler üzerinde yineleme yapan enumeratörü döndürür.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.foundation.rendering.ApsNode&gt; - Bu `IEnumerator`.
### iterator_Rename_Namesake() {#iterator-Rename-Namesake--}
```
public System.Collections.IEnumerator iterator_Rename_Namesake()
```


Enumeratörü al.

**Returns:**
com.aspose.ms.System.Collections.IEnumerator - Bu `IEnumerator`.
