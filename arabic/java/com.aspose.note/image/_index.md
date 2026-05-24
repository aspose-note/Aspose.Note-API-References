---
title: "صورة"
second_title: "مرجع Aspose.Note for Java API"
description: "يمثل صورة."
type: docs
weight: 33
url: /ar/java/com.aspose.note/image/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode

**All Implemented Interfaces:**
[com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode), [com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode), [com.aspose.note.ITaggable](../../com.aspose.note/itaggable)
```
public final class Image extends CompositeNode<Loop> implements IPageChildNode, IOutlineElementChildNode, ITaggable
```

يمثل صورة.
## المنشئات

| المنشئ | الوصف |
| --- | --- |
| [Image(String path)](#Image-java.lang.String-) | ينشئ مثيلاً جديداً من الفئة `Image`. |
| [Image(String fileName, InputStream imageStream)](#Image-java.lang.String-java.io.InputStream-) | ينشئ مثيلاً جديداً من الفئة `Image`. |
| [Image()](#Image--) | ينشئ مثيلاً جديداً من الفئة `Image`. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | يقبل زائر العقدة. |
| [getAlignment()](#getAlignment--) | يحصل على المحاذاة. |
| [getAlternativeTextDescription()](#getAlternativeTextDescription--) | يحصل على نص بديل للجسم للصورة. |
| [getAlternativeTextTitle()](#getAlternativeTextTitle--) | يحصل على عنوان النص البديل للصورة. |
| [getBytes()](#getBytes--) | يحصل على مخزن بيانات الصورة. |
| [getFileName()](#getFileName--) | يحصل على اسم الملف. |
| [getFilePath()](#getFilePath--) | يحصل على المسار إلى ملف الصورة. |
| [getFormat()](#getFormat--) | يحصل على تنسيق الصورة. |
| [getHeight()](#getHeight--) | يحصل على الارتفاع. |
| [getHorizontalOffset()](#getHorizontalOffset--) | يحصل على الإزاحة الأفقية. |
| [getHyperlinkUrl()](#getHyperlinkUrl--) | يحصل على الارتباط التشعبي المرتبط بالصورة. |
| [getLastModifiedTime()](#getLastModifiedTime--) | يحصل على وقت التعديل الأخير. |
| [getOriginalHeight()](#getOriginalHeight--) | يحصل على الارتفاع الأصلي. |
| [getOriginalWidth()](#getOriginalWidth--) | يحصل على العرض الأصلي. |
| [getTags()](#getTags--) | يحصل على قائمة بجميع العلامات الخاصة بصورة. |
| [getVerticalOffset()](#getVerticalOffset--) | يحصل على الإزاحة العمودية. |
| [getWidth()](#getWidth--) | يحصل على العرض. |
| [isBackground()](#isBackground--) | يحصل على ما إذا كانت الصورة صورة خلفية. |
| [replace(Image newImage)](#replace-com.aspose.note.Image-) | يستبدل بيانات الصورة الحالية بالبيانات من كائن Image المقدم. |
| [setAlignment(int value)](#setAlignment-int-) | يضبط المحاذاة. |
| [setAlternativeTextDescription(String value)](#setAlternativeTextDescription-java.lang.String-) | يضبط نصًا بديلًا للجسم للصورة. |
| [setAlternativeTextTitle(String value)](#setAlternativeTextTitle-java.lang.String-) | يضبط عنوان النص البديل للصورة. |
| [setBackground(boolean value)](#setBackground-boolean-) | يحصل على ما إذا كانت الصورة صورة خلفية. |
| [setHeight(float value)](#setHeight-float-) | يضبط الارتفاع. |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | يضبط الإزاحة الأفقية. |
| [setHyperlinkUrl(String value)](#setHyperlinkUrl-java.lang.String-) | يضبط الارتباط التشعبي المرتبط بالصورة. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | يضبط وقت التعديل الأخير. |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | يضبط الإزاحة العمودية. |
| [setWidth(float value)](#setWidth-float-) | يضبط العرض. |
### Image(String path) {#Image-java.lang.String-}
```
public Image(String path)
```


ينشئ مثيلاً جديداً من الفئة `Image`.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| path | java.lang.String | سلسلة تحتوي على المسار إلى الملف الذي سيتم إنشاء الـ `Image` منه. |

### Image(String fileName, InputStream imageStream) {#Image-java.lang.String-java.io.InputStream-}
```
public Image(String fileName, InputStream imageStream)
```


ينشئ مثيلاً جديداً من الفئة `Image`.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fileName | java.lang.String | اسم الصورة. |
| imageStream | java.io.InputStream | دفق يحتوي على الصورة. |

### Image() {#Image--}
```
public Image()
```


ينشئ مثيلاً جديداً من الفئة `Image`.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


يقبل زائر العقدة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | الكائن من فئة مشتقة من `DocumentVisitor`. |

### getAlignment() {#getAlignment--}
```
public int getAlignment()
```


يحصل على المحاذاة.

**Returns:**
int
### getAlternativeTextDescription() {#getAlternativeTextDescription--}
```
public final String getAlternativeTextDescription()
```


يحصل على نص بديل للجسم للصورة.

**Returns:**
java.lang.String
### getAlternativeTextTitle() {#getAlternativeTextTitle--}
```
public final String getAlternativeTextTitle()
```


يحصل على عنوان النص البديل للصورة.

**Returns:**
java.lang.String
### getBytes() {#getBytes--}
```
public byte[] getBytes()
```


يحصل على مخزن بيانات الصورة.

**Returns:**
byte[]
### getFileName() {#getFileName--}
```
public String getFileName()
```


يحصل على اسم الملف.

**Returns:**
java.lang.String
### getFilePath() {#getFilePath--}
```
public String getFilePath()
```


يحصل على المسار إلى ملف الصورة.

**Returns:**
java.lang.String
### getFormat() {#getFormat--}
```
public final System.Drawing.Imaging.ImageFormat getFormat()
```


يحصل على تنسيق الصورة.

**Returns:**
com.aspose.ms.System.Drawing.Imaging.ImageFormat
### getHeight() {#getHeight--}
```
public final float getHeight()
```


يحصل على الارتفاع. هذا هو الارتفاع الحقيقي للصورة في مستند MS OneNote.

**Returns:**
float
### getHorizontalOffset() {#getHorizontalOffset--}
```
public float getHorizontalOffset()
```


يحصل على الإزاحة الأفقية.

**Returns:**
float
### getHyperlinkUrl() {#getHyperlinkUrl--}
```
public String getHyperlinkUrl()
```


يحصل على الارتباط التشعبي المرتبط بالصورة.

**Returns:**
java.lang.String
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


يحصل على وقت التعديل الأخير.

**Returns:**
java.util.Date
### getOriginalHeight() {#getOriginalHeight--}
```
public float getOriginalHeight()
```


يحصل على الارتفاع الأصلي. هذا هو العرض الأصلي للصورة، قبل تغيير الحجم.

**Returns:**
float
### getOriginalWidth() {#getOriginalWidth--}
```
public float getOriginalWidth()
```


يحصل على العرض الأصلي. هذا هو العرض الأصلي للصورة، قبل تغيير الحجم.

**Returns:**
float
### getTags() {#getTags--}
```
public final System.Collections.Generic.List<ITag> getTags()
```


يحصل على قائمة بجميع العلامات الخاصة بصورة.

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.note.ITag&gt;
### getVerticalOffset() {#getVerticalOffset--}
```
public float getVerticalOffset()
```


يحصل على الإزاحة العمودية.

**Returns:**
float
### getWidth() {#getWidth--}
```
public final float getWidth()
```


يحصل على العرض. هذا هو العرض الحقيقي للصورة في مستند MS OneNote.

**Returns:**
float
### isBackground() {#isBackground--}
```
public final boolean isBackground()
```


يحصل على ما إذا كانت الصورة صورة خلفية.

**Returns:**
boolean
### replace(Image newImage) {#replace-com.aspose.note.Image-}
```
public void replace(Image newImage)
```


يستبدل بيانات الصورة الحالية بالبيانات من كائن Image المقدم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| newImage | [Image](../../com.aspose.note/image) |  |

### setAlignment(int value) {#setAlignment-int-}
```
public void setAlignment(int value)
```


يضبط المحاذاة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setAlternativeTextDescription(String value) {#setAlternativeTextDescription-java.lang.String-}
```
public final void setAlternativeTextDescription(String value)
```


يضبط نصًا بديلًا للجسم للصورة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setAlternativeTextTitle(String value) {#setAlternativeTextTitle-java.lang.String-}
```
public final void setAlternativeTextTitle(String value)
```


يضبط عنوان النص البديل للصورة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setBackground(boolean value) {#setBackground-boolean-}
```
public final void setBackground(boolean value)
```


يحصل على ما إذا كانت الصورة صورة خلفية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setHeight(float value) {#setHeight-float-}
```
public final void setHeight(float value)
```


يضبط الارتفاع. هذا هو الارتفاع الحقيقي للصورة في مستند MS OneNote.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | float |  |

### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public void setHorizontalOffset(float value)
```


يضبط الإزاحة الأفقية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | float |  |

### setHyperlinkUrl(String value) {#setHyperlinkUrl-java.lang.String-}
```
public void setHyperlinkUrl(String value)
```


يضبط الارتباط التشعبي المرتبط بالصورة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


يضبط وقت التعديل الأخير.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.Date |  |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public void setVerticalOffset(float value)
```


يضبط الإزاحة العمودية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | float |  |

### setWidth(float value) {#setWidth-float-}
```
public final void setWidth(float value)
```


يضبط العرض. هذا هو العرض الحقيقي للصورة في مستند MS OneNote.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | float |  |

