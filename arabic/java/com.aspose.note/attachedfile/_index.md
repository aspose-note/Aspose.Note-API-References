---
title: "AttachedFile"
second_title: "مرجع Aspose.Note for Java API"
description: "يمثل ملفًا مرفقًا."
type: docs
weight: 11
url: /ar/java/com.aspose.note/attachedfile/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node)

**All Implemented Interfaces:**
[com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode), [com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode), [com.aspose.note.ITaggable](../../com.aspose.note/itaggable)
```
public class AttachedFile extends Node implements IPageChildNode, IOutlineElementChildNode, ITaggable
```

يمثل ملفًا مرفقًا.
## المنشئات

| المنشئ | الوصف |
| --- | --- |
| [AttachedFile(String path)](#AttachedFile-java.lang.String-) | ينشئ مثيلاً جديدًا من الفئة `AttachedFile`. |
| [AttachedFile(String path, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)](#AttachedFile-java.lang.String-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-) | ينشئ مثيلاً جديدًا من الفئة `AttachedFile`. |
| [AttachedFile(String fileName, InputStream attachedFileStream)](#AttachedFile-java.lang.String-java.io.InputStream-) | ينشئ مثيلاً جديدًا من الفئة `AttachedFile`. |
| [AttachedFile(String fileName, InputStream attachedFileStream, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)](#AttachedFile-java.lang.String-java.io.InputStream-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-) | ينشئ مثيلاً جديدًا من الفئة `AttachedFile`. |
| [AttachedFile()](#AttachedFile--) | ينشئ مثيلاً جديدًا من الفئة `AttachedFile`. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | يقبل زائر العقدة. |
| [getAlignment()](#getAlignment--) | يحصل على المحاذاة. |
| [getAlternativeTextDescription()](#getAlternativeTextDescription--) | يحصل أو يضبط نصًا بديلًا للجسم لأيقونة الملف المرفق. |
| [getAlternativeTextTitle()](#getAlternativeTextTitle--) | يحصل أو يضبط عنوان النص البديل لأيقونة الملف المرفق. |
| [getBytes()](#getBytes--) | يحصل على البيانات الثنائية لملف مضمّن. |
| [getExtension()](#getExtension--) | يحصل على امتداد الملف المضمّن. |
| [getFileName()](#getFileName--) | يحصل على اسم الملف المضمّن. |
| [getFilePath()](#getFilePath--) | يحصل على المسار إلى الملف الأصلي. |
| [getHeight()](#getHeight--) | يحصل على الارتفاع الأصلي لأيقونة الملف المضمّن. |
| [getHorizontalOffset()](#getHorizontalOffset--) | يحصل على الإزاحة الأفقية. |
| [getIcon()](#getIcon--) | يحصل على البيانات الثنائية للأيقونة المرتبطة بالملف المضمّن. |
| [getIconExtension()](#getIconExtension--) | يحصل على امتداد الأيقونة. |
| [getLastModifiedTime()](#getLastModifiedTime--) | يحصل على وقت التعديل الأخير. |
| [getMaxHeight()](#getMaxHeight--) | يحصل على الحد الأقصى للارتفاع لعرض أيقونة الملف المضمن. |
| [getMaxWidth()](#getMaxWidth--) | يحصل على الحد الأقصى للعرض لعرض أيقونة الملف المضمن. |
| [getParsingErrorInfo()](#getParsingErrorInfo--) | يحصل على البيانات حول الخطأ الذي حدث أثناء الوصول إلى الملف. |
| [getTags()](#getTags--) | يحصل على قائمة العلامات لملف مرفق. |
| [getText()](#getText--) | يحصل على التمثيل النصي للملف المضمن. |
| [getVerticalOffset()](#getVerticalOffset--) | يحصل على الإزاحة العمودية. |
| [getWidth()](#getWidth--) | يحصل على العرض الأصلي لأيقونة الملف المضمن. |
| [isPrintout()](#isPrintout--) | يحصل على قيمة تشير إلى ما إذا كان عرض الملف هو نسخة مطبوعة. |
| [isSizeSetByUser()](#isSizeSetByUser--) | يحصل على قيمة تشير إلى ما إذا كان حجم الأيقونة قد تم تحديثه صراحةً من قبل المستخدم. |
| [setAlignment(int value)](#setAlignment-int-) | يضبط المحاذاة. |
| [setAlternativeTextDescription(String value)](#setAlternativeTextDescription-java.lang.String-) | يحصل أو يضبط نصًا بديلًا للجسم لأيقونة الملف المرفق. |
| [setAlternativeTextTitle(String value)](#setAlternativeTextTitle-java.lang.String-) | يحصل أو يضبط عنوان النص البديل لأيقونة الملف المرفق. |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | يضبط الإزاحة الأفقية. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | يضبط وقت التعديل الأخير. |
| [setMaxHeight(float value)](#setMaxHeight-float-) | يضبط الحد الأقصى للارتفاع لعرض أيقونة الملف المضمن. |
| [setMaxWidth(float value)](#setMaxWidth-float-) | يضبط الحد الأقصى للعرض لعرض أيقونة الملف المضمن. |
| [setPrintout(boolean value)](#setPrintout-boolean-) | يضبط قيمة تشير إلى ما إذا كان عرض الملف هو نسخة مطبوعة. |
| [setSizeSetByUser(boolean value)](#setSizeSetByUser-boolean-) | يضبط قيمة تشير إلى ما إذا كان حجم الأيقونة قد تم تحديثه صراحةً من قبل المستخدم. |
| [setText(String value)](#setText-java.lang.String-) | يضبط التمثيل النصي للملف المضمن. |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | يضبط الإزاحة العمودية. |
### AttachedFile(String path) {#AttachedFile-java.lang.String-}
```
public AttachedFile(String path)
```


ينشئ مثيلاً جديدًا من الفئة `AttachedFile`.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| path | java.lang.String | سلسلة نصية تحتوي على المسار إلى الملف الذي سيتم إنشاء `AttachedFile` منه. |

### AttachedFile(String path, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat) {#AttachedFile-java.lang.String-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-}
```
public AttachedFile(String path, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)
```


ينشئ مثيلاً جديدًا من الفئة `AttachedFile`.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| path | java.lang.String | سلسلة نصية تحتوي على المسار إلى الملف الذي سيتم إنشاء `AttachedFile` منه. |
| icon | java.io.InputStream | أيقونة للملف المرفق. |
| iconFormat | com.aspose.ms.System.Drawing.Imaging.ImageFormat |  |

### AttachedFile(String fileName, InputStream attachedFileStream) {#AttachedFile-java.lang.String-java.io.InputStream-}
```
public AttachedFile(String fileName, InputStream attachedFileStream)
```


ينشئ مثيلاً جديدًا من الفئة `AttachedFile`.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fileName | java.lang.String | اسم الملف المرفق. |
| attachedFileStream | java.io.InputStream | دفق يحتوي على بايتات الملف المرفق. |

### AttachedFile(String fileName, InputStream attachedFileStream, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat) {#AttachedFile-java.lang.String-java.io.InputStream-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-}
```
public AttachedFile(String fileName, InputStream attachedFileStream, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)
```


ينشئ مثيلاً جديدًا من الفئة `AttachedFile`.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fileName | java.lang.String | اسم الملف المرفق. |
| attachedFileStream | java.io.InputStream | دفق يحتوي على بايتات الملف المرفق. |
| icon | java.io.InputStream | أيقونة للملف المرفق. |
| iconFormat | com.aspose.ms.System.Drawing.Imaging.ImageFormat | تنسيق أيقونة الملف المرفق. |

### AttachedFile() {#AttachedFile--}
```
public AttachedFile()
```


ينشئ مثيلاً جديدًا من الفئة `AttachedFile`.

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


يحصل أو يضبط نصًا بديلًا للجسم لأيقونة الملف المرفق.

**Returns:**
java.lang.String
### getAlternativeTextTitle() {#getAlternativeTextTitle--}
```
public final String getAlternativeTextTitle()
```


يحصل أو يضبط عنوان النص البديل لأيقونة الملف المرفق.

**Returns:**
java.lang.String
### getBytes() {#getBytes--}
```
public byte[] getBytes()
```


يحصل على البيانات الثنائية لملف مضمّن.

**Returns:**
byte[]
### getExtension() {#getExtension--}
```
public String getExtension()
```


يحصل على امتداد الملف المضمّن.

**Returns:**
java.lang.String
### getFileName() {#getFileName--}
```
public String getFileName()
```


يحصل على اسم الملف المضمّن.

**Returns:**
java.lang.String
### getFilePath() {#getFilePath--}
```
public String getFilePath()
```


يحصل على المسار إلى الملف الأصلي.

**Returns:**
java.lang.String
### getHeight() {#getHeight--}
```
public float getHeight()
```


يحصل على الارتفاع الأصلي لأيقونة الملف المضمّن.

**Returns:**
float
### getHorizontalOffset() {#getHorizontalOffset--}
```
public float getHorizontalOffset()
```


يحصل على الإزاحة الأفقية.

**Returns:**
float
### getIcon() {#getIcon--}
```
public byte[] getIcon()
```


يحصل على البيانات الثنائية للأيقونة المرتبطة بالملف المضمّن.

**Returns:**
byte[]
### getIconExtension() {#getIconExtension--}
```
public String getIconExtension()
```


يحصل على امتداد الأيقونة.

**Returns:**
java.lang.String
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


يحصل على وقت التعديل الأخير.

**Returns:**
java.util.Date
### getMaxHeight() {#getMaxHeight--}
```
public float getMaxHeight()
```


يحصل على الحد الأقصى للارتفاع لعرض أيقونة الملف المضمن.

**Returns:**
float
### getMaxWidth() {#getMaxWidth--}
```
public float getMaxWidth()
```


يحصل على الحد الأقصى للعرض لعرض أيقونة الملف المضمن.

**Returns:**
float
### getParsingErrorInfo() {#getParsingErrorInfo--}
```
public final ParsingErrorInfo getParsingErrorInfo()
```


يحصل على البيانات حول الخطأ الذي حدث أثناء الوصول إلى الملف.

**Returns:**
[ParsingErrorInfo](../../com.aspose.note.infrastructure/parsingerrorinfo)
### getTags() {#getTags--}
```
public final System.Collections.Generic.List<ITag> getTags()
```


يحصل على قائمة العلامات لملف مرفق.

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.note.ITag&gt;
### getText() {#getText--}
```
public String getText()
```


يحصل على تمثيل النص للملف المضمن. يجب ألا يحتوي السلسلة على أي أحرف ذات القيمة 10 (سطر جديد) أو 13 (عودة سيارة).

**Returns:**
java.lang.String
### getVerticalOffset() {#getVerticalOffset--}
```
public float getVerticalOffset()
```


يحصل على الإزاحة العمودية.

**Returns:**
float
### getWidth() {#getWidth--}
```
public float getWidth()
```


يحصل على العرض الأصلي لأيقونة الملف المضمن.

**Returns:**
float
### isPrintout() {#isPrintout--}
```
public boolean isPrintout()
```


يحصل على قيمة تشير إلى ما إذا كان عرض الملف هو نسخة مطبوعة.

**Returns:**
boolean
### isSizeSetByUser() {#isSizeSetByUser--}
```
public boolean isSizeSetByUser()
```


يحصل على قيمة تشير إلى ما إذا كان حجم الأيقونة قد تم تحديثه صراحةً من قبل المستخدم.

**Returns:**
boolean
### setAlignment(int value) {#setAlignment-int-}
```
public void setAlignment(int value)
```


يضبط المحاذاة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int | قيمة المحاذاة. |

### setAlternativeTextDescription(String value) {#setAlternativeTextDescription-java.lang.String-}
```
public final void setAlternativeTextDescription(String value)
```


يحصل أو يضبط نصًا بديلًا للجسم لأيقونة الملف المرفق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setAlternativeTextTitle(String value) {#setAlternativeTextTitle-java.lang.String-}
```
public final void setAlternativeTextTitle(String value)
```


يحصل أو يضبط عنوان النص البديل لأيقونة الملف المرفق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public void setHorizontalOffset(float value)
```


يضبط الإزاحة الأفقية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | float | قيمة الإزاحات. |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


يضبط وقت التعديل الأخير.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.Date | قيمة التاريخ. |

### setMaxHeight(float value) {#setMaxHeight-float-}
```
public void setMaxHeight(float value)
```


يضبط الحد الأقصى للارتفاع لعرض أيقونة الملف المضمن.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | float | قيمة الحد الأقصى للارتفاع. |

### setMaxWidth(float value) {#setMaxWidth-float-}
```
public void setMaxWidth(float value)
```


يضبط الحد الأقصى للعرض لعرض أيقونة الملف المضمن.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | float | قيمة الحد الأقصى للعرض. |

### setPrintout(boolean value) {#setPrintout-boolean-}
```
public void setPrintout(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان عرض الملف هو نسخة مطبوعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean | قيمة جديدة. |

### setSizeSetByUser(boolean value) {#setSizeSetByUser-boolean-}
```
public void setSizeSetByUser(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان حجم الأيقونة قد تم تحديثه صراحةً من قبل المستخدم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean | قيمة جديدة. |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


يضبط تمثيل النص للملف المضمن. يجب ألا تحتوي السلسلة على أي أحرف ذات القيمة 10 (سطر جديد) أو 13 (عودة سيارة).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | قيمة النص. |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public void setVerticalOffset(float value)
```


يضبط الإزاحة العمودية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | float | قيمة الإزاحة. |

