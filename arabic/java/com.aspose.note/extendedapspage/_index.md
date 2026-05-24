---
title: "ExtendedApsPage"
second_title: "مرجع Aspose.Note for Java API"
description: "يمثّل غلافًا لـ ApsGlyphs القياسي الذي يوسّع بعض سلوكيات الرسم."
type: docs
weight: 27
url: /ar/java/com.aspose.note/extendedapspage/
---

**Inheritance:**
java.lang.Object, com.aspose.foundation.rendering.ApsNode, com.aspose.foundation.rendering.ApsCompositeNode, com.aspose.foundation.rendering.ApsPage

**All Implemented Interfaces:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerable
```
public class ExtendedApsPage extends ApsPage implements System.Collections.Generic.IGenericEnumerable<ApsNode>
```

يمثل غلافًا لـ ApsGlyphs القياسي، الذي يوسع بعض سلوكيات الرسم.
## المنشئات

| المنشئ | الوصف |
| --- | --- |
| [ExtendedApsPage(System.Drawing.SizeF pageSize, float pageStartInNotePage, Margin margin)](#ExtendedApsPage-com.aspose.ms.System.Drawing.SizeF-float-com.aspose.foundation.layout.Margin-) | يُهيئ نسخة جديدة من الفئة `ExtendedApsPage`. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [getContentSize()](#getContentSize--) | يحصل على حجم الصفحة مستثنياً الهوامش. |
| [getMargin()](#getMargin--) | يحصل على هامش هذه الصفحة. |
| [getPageEndInNotePage()](#getPageEndInNotePage--) | يحصل على موضع نهاية الصفحة في صفحة MS OneNote، عندما تُقسم صفحة MS OneNote واحدة إلى عدة صفحات aps. |
| [getPageSize()](#getPageSize--) | يحصل على الحجم النهائي للصفحة. |
| [getPageStartInNotePage()](#getPageStartInNotePage--) | يحصل على موضع بداية الصفحة في صفحة MS OneNote، عندما تُقسم صفحة MS OneNote واحدة إلى عدة صفحات aps. |
| [iterator()](#iterator--) | يرجع المُعدِّد الذي يتنقّل عبر جميع العقد في هذه الصفحة. |
| [iterator_Rename_Namesake()](#iterator-Rename-Namesake--) | المُعدِّد get. |
### ExtendedApsPage(System.Drawing.SizeF pageSize, float pageStartInNotePage, Margin margin) {#ExtendedApsPage-com.aspose.ms.System.Drawing.SizeF-float-com.aspose.foundation.layout.Margin-}
```
public ExtendedApsPage(System.Drawing.SizeF pageSize, float pageStartInNotePage, Margin margin)
```


يُهيئ نسخة جديدة من الفئة `ExtendedApsPage`.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| pageSize | com.aspose.ms.System.Drawing.SizeF | حجم الصفحة. |
| pageStartInNotePage | float | بداية الصفحة في صفحة MS OneNote الأصلية. |
| margin | com.aspose.foundation.layout.Margin | الهامش الموسع للصفحة. |

### getContentSize() {#getContentSize--}
```
public System.Drawing.SizeF getContentSize()
```


يحصل على حجم الصفحة مستثنياً الهوامش.

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getMargin() {#getMargin--}
```
public Margin getMargin()
```


يحصل على هامش هذه الصفحة.

**Returns:**
com.aspose.foundation.layout.Margin
### getPageEndInNotePage() {#getPageEndInNotePage--}
```
public float getPageEndInNotePage()
```


يحصل على موضع نهاية الصفحة في صفحة MS OneNote، عندما تُقسم صفحة MS OneNote واحدة إلى عدة صفحات aps.

**Returns:**
float
### getPageSize() {#getPageSize--}
```
public System.Drawing.SizeF getPageSize()
```


يحصل على الحجم النهائي للصفحة.

**Returns:**
com.aspose.ms.System.Drawing.SizeF
### getPageStartInNotePage() {#getPageStartInNotePage--}
```
public float getPageStartInNotePage()
```


يحصل على موضع بداية الصفحة في صفحة MS OneNote، عندما تُقسم صفحة MS OneNote واحدة إلى عدة صفحات aps.

**Returns:**
float
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<ApsNode> iterator()
```


يرجع المُعدِّد الذي يتنقّل عبر جميع العقد في هذه الصفحة.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.foundation.rendering.ApsNode&gt; - الـ `IEnumerator`.
### iterator_Rename_Namesake() {#iterator-Rename-Namesake--}
```
public System.Collections.IEnumerator iterator_Rename_Namesake()
```


المُعدِّد get.

**Returns:**
com.aspose.ms.System.Collections.IEnumerator - الـ `IEnumerator`.
