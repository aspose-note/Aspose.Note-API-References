---
title: "RichText"
second_title: "مرجع Aspose.Note for Java API"
description: "يمثل نصًا غنيًا."
type: docs
weight: 82
url: /ar/java/com.aspose.note/richtext/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node)

**All Implemented Interfaces:**
[com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode), [com.aspose.note.ITaggable](../../com.aspose.note/itaggable), com.aspose.ms.System.Collections.Generic.IGenericEnumerable
```
public class RichText extends Node implements IOutlineElementChildNode, ITaggable, System.Collections.Generic.IGenericEnumerable<Character>
```

يمثل نصًا غنيًا.
## المنشئات

| المنشئ | الوصف |
| --- | --- |
| [RichText()](#RichText--) | ينشئ مثيلًا جديدًا من الفئة [RichText](../../com.aspose.note/richtext). |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | يقبل زائر العقدة. |
| [append(String value)](#append-java.lang.String-) | يضيف سلسلة إلى النطاق النصي الأخير. |
| [append(String value, TextStyle style)](#append-java.lang.String-com.aspose.note.TextStyle-) | يضيف سلسلة إلى النهاية. |
| [appendFront(String value)](#appendFront-java.lang.String-) | يضيف سلسلة إلى مقدمة النطاق النصي الأول. |
| [appendFront(String value, TextStyle style)](#appendFront-java.lang.String-com.aspose.note.TextStyle-) | يضيف سلسلة إلى المقدمة. |
| [clear()](#clear--) | يمسح محتوى هذا الكائن. |
| [getAlignment()](#getAlignment--) | يحصل على المحاذاة. |
| [getLastModifiedTime()](#getLastModifiedTime--) | يحصل على وقت التعديل الأخير. |
| [getLength()](#getLength--) |  |
| [getLineSpacing()](#getLineSpacing--) | يحصل على تباعد الأسطر. |
| [getParagraphStyle()](#getParagraphStyle--) | يحصل على نمط الفقرة. |
| [getSpaceAfter()](#getSpaceAfter--) | يحصل على الحد الأدنى للمسافة بعد. |
| [getSpaceBefore()](#getSpaceBefore--) | يحصل على الحد الأدنى للمسافة قبل. |
| [getStyles()](#getStyles--) | يحصل على الأنماط. |
| [getTags()](#getTags--) | يحصل على قائمة جميع العلامات في الفقرة. |
| [getText()](#getText--) | يحصل على النص. |
| [getTextRuns()](#getTextRuns--) |  |
| [indexOf(char value)](#indexOf-char-) | يعيد الفهرس الصفري للظهور الأول للحرف Unicode المحدد في هذه السلسلة. |
| [indexOf(char value, int startIndex)](#indexOf-char-int-) | يعيد الفهرس الصفري للظهور الأول للحرف Unicode المحدد في هذه السلسلة. |
| [indexOf(char value, int startIndex, int count)](#indexOf-char-int-int-) | يعيد الفهرس الصفري للظهور الأول للحرف المحدد في هذا الكائن. |
| [indexOf(String value)](#indexOf-java.lang.String-) | يعيد الفهرس الصفري للظهور الأول للسلسلة المحددة في هذا الكائن. |
| [indexOf(String value, int startIndex)](#indexOf-java.lang.String-int-) | يعيد الفهرس الصفري للظهور الأول للسلسلة المحددة في هذا الكائن. |
| [indexOf(String value, int startIndex, int count)](#indexOf-java.lang.String-int-int-) | يعيد الفهرس الصفري للظهور الأول للسلسلة المحددة في هذا الكائن. |
| [indexOf(String value, int startIndex, int count, short comparisonType)](#indexOf-java.lang.String-int-int-short-) | يعيد الفهرس الصفري للظهور الأول للسلسلة المحددة في الكائن الحالي. |
| [indexOf(String value, short comparisonType)](#indexOf-java.lang.String-short-) | يعيد الفهرس الصفري للظهور الأول للسلسلة المحددة في الكائن الحالي. |
| [indexOf_Rename_Namesake(String value, int startIndex, short comparisonType)](#indexOf-Rename-Namesake-java.lang.String-int-short-) | يعيد الفهرس الصفري للظهور الأول للسلسلة المحددة في الكائن الحالي. |
| [insert(int startIndex, String value)](#insert-int-java.lang.String-) | يدرج سلسلة محددة في موضع فهرس محدد في هذا الكائن. |
| [insert(int startIndex, String value, TextStyle style)](#insert-int-java.lang.String-com.aspose.note.TextStyle-) | يدرج سلسلة محددة مع نمط محدد في موضع فهرس محدد في هذا الكائن. |
| [iterator()](#iterator--) |  |
| [remove(int startIndex)](#remove-int-) | يزيل جميع الأحرف في الكائن الحالي، بدءًا من موضع محدد ومتابعة حتى الموضع الأخير. |
| [remove(int startIndex, int count)](#remove-int-int-) | يزيل عددًا محددًا من الأحرف في الكائن الحالي بدءًا من موضع محدد. |
| [replace(char oldChar, char newChar)](#replace-char-char-) | يستبدل جميع ظهورات حرف Unicode محدد في هذا الكائن بحرف Unicode آخر محدد. |
| [replace(String oldValue, String newValue)](#replace-java.lang.String-java.lang.String-) | يستبدل جميع ظهورات سلسلة محددة في الكائن الحالي بسلسلة أخرى محددة. |
| [replace(String oldValue, String newValue, TextStyle style)](#replace-java.lang.String-java.lang.String-com.aspose.note.TextStyle-) | يستبدل جميع ظهورات سلسلة محددة في الكائن الحالي بسلسلة أخرى محددة بنمط محدد. |
| [setAlignment(int value)](#setAlignment-int-) | يضبط المحاذاة. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | يضبط وقت التعديل الأخير. |
| [setLineSpacing(float value)](#setLineSpacing-float-) |  |
| [setLineSpacing(Float value)](#setLineSpacing-java.lang.Float-) | يضبط تباعد الأسطر. |
| [setParagraphStyle(ParagraphStyle value)](#setParagraphStyle-com.aspose.note.ParagraphStyle-) | يضبط نمط الفقرة. |
| [setSpaceAfter(float value)](#setSpaceAfter-float-) |  |
| [setSpaceAfter(Float value)](#setSpaceAfter-java.lang.Float-) | يضبط الحد الأدنى للمسافة بعد. |
| [setSpaceBefore(float value)](#setSpaceBefore-float-) |  |
| [setSpaceBefore(Float value)](#setSpaceBefore-java.lang.Float-) | يضبط الحد الأدنى للمسافة قبل. |
| [setText(String value)](#setText-java.lang.String-) | يضبط النص. |
| [trim()](#trim--) | يزيل جميع أحرف المسافات البيضاء في البداية والنهاية. |
| [trim(char trimChar)](#trim-char-) | يزيل جميع حالات الحرف في البداية والنهاية. |
| [trim(char[] trimChars)](#trim-char...-) | يزيل جميع تكرارات مجموعة الأحرف المحددة في مصفوفة في البداية والنهاية. |
| [trimEnd()](#trimEnd--) | يزيل جميع أحرف المسافات البيضاء في النهاية. |
| [trimEnd(char trimChar)](#trimEnd-char-) | يزيل جميع تكرارات الحرف في النهاية. |
| [trimEnd(char[] trimChars)](#trimEnd-char...-) | يزيل جميع تكرارات مجموعة الأحرف المحددة في مصفوفة في النهاية. |
| [trimStart()](#trimStart--) | يزيل جميع أحرف المسافات البيضاء في البداية. |
| [trimStart(char trimChar)](#trimStart-char-) | يزيل جميع تكرارات الحرف المحدد في البداية. |
| [trimStart(char[] trimChars)](#trimStart-char...-) | يزيل جميع تكرارات مجموعة الأحرف المحددة في مصفوفة في البداية. |
### RichText() {#RichText--}
```
public RichText()
```


ينشئ مثيلًا جديدًا من الفئة [RichText](../../com.aspose.note/richtext).

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


يقبل زائر العقدة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | كائن من فئة مشتقة من [DocumentVisitor](../../com.aspose.note/documentvisitor). |

### append(String value) {#append-java.lang.String-}
```
public RichText append(String value)
```


يضيف سلسلة إلى النطاق النصي الأخير.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | القيمة المضافة. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### append(String value, TextStyle style) {#append-java.lang.String-com.aspose.note.TextStyle-}
```
public final RichText append(String value, TextStyle style)
```


يضيف سلسلة إلى النهاية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | القيمة المضافة. |
| style | [TextStyle](../../com.aspose.note/textstyle) | نمط السلسلة المضافة. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### appendFront(String value) {#appendFront-java.lang.String-}
```
public RichText appendFront(String value)
```


يضيف سلسلة إلى مقدمة النطاق النصي الأول.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | القيمة المضافة. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### appendFront(String value, TextStyle style) {#appendFront-java.lang.String-com.aspose.note.TextStyle-}
```
public RichText appendFront(String value, TextStyle style)
```


يضيف سلسلة إلى المقدمة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | القيمة المضافة. |
| style | [TextStyle](../../com.aspose.note/textstyle) | نمط السلسلة المضافة. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### clear() {#clear--}
```
public final RichText clear()
```


يمسح محتوى هذا الكائن.

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### getAlignment() {#getAlignment--}
```
public int getAlignment()
```


يحصل على المحاذاة.

**Returns:**
int
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


يحصل على وقت التعديل الأخير.

**Returns:**
java.util.Date
### getLength() {#getLength--}
```
public final int getLength()
```




**Returns:**
int
### getLineSpacing() {#getLineSpacing--}
```
public Float getLineSpacing()
```


يحصل على تباعد الأسطر.

**Returns:**
java.lang.Float
### getParagraphStyle() {#getParagraphStyle--}
```
public final ParagraphStyle getParagraphStyle()
```


يحصل على نمط الفقرة. تُستخدم هذه الإعدادات إذا لم يكن هناك كائن TextStyle مطابق في مجموعة [getStyles](../../com.aspose.note/richtext\#getStyles) أو إذا لم يحدد هذا الكائن الإعداد المطلوب.

**Returns:**
[ParagraphStyle](../../com.aspose.note/paragraphstyle)
### getSpaceAfter() {#getSpaceAfter--}
```
public Float getSpaceAfter()
```


يحصل على الحد الأدنى للمسافة بعد.

**Returns:**
java.lang.Float
### getSpaceBefore() {#getSpaceBefore--}
```
public Float getSpaceBefore()
```


يحصل على الحد الأدنى للمسافة قبل.

**Returns:**
java.lang.Float
### getStyles() {#getStyles--}
```
public System.Collections.Generic.IGenericEnumerable<TextStyle> getStyles()
```


يحصل على الأنماط.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerable&lt;com.aspose.note.TextStyle&gt;
### getTags() {#getTags--}
```
public final System.Collections.Generic.List<ITag> getTags()
```


يحصل على قائمة جميع العلامات في الفقرة.

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.note.ITag&gt;
### getText() {#getText--}
```
public final String getText()
```


يحصل على النص. يجب ألا تحتوي السلسلة على أي أحرف ذات القيمة 10 (سطر جديد).

**Returns:**
java.lang.String
### getTextRuns() {#getTextRuns--}
```
public final System.Collections.Generic.IGenericEnumerable<TextRun> getTextRuns()
```




**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerable&lt;com.aspose.note.TextRun&gt;
### indexOf(char value) {#indexOf-char-}
```
public final int indexOf(char value)
```


يعيد الفهرس الصفري للظهور الأول للحرف Unicode المحدد في هذه السلسلة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | char | القيمة. |

**Returns:**
عدد صحيح - الـ `int`.
### indexOf(char value, int startIndex) {#indexOf-char-int-}
```
public final int indexOf(char value, int startIndex)
```


يرجع الفهرس الصفري للظهور الأول للحرف Unicode المحدد في هذه السلسلة. يبدأ البحث عند موضع حرف محدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | char | القيمة. |
| startIndex | int | موضع بدء البحث. |

**Returns:**
عدد صحيح - الـ `int`.
### indexOf(char value, int startIndex, int count) {#indexOf-char-int-int-}
```
public final int indexOf(char value, int startIndex, int count)
```


يرجع الفهرس الصفري للظهور الأول للحرف المحدد في هذه الحالة. يبدأ البحث عند موضع حرف محدد ويفحص عددًا محددًا من مواضع الأحرف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | char | القيمة. |
| startIndex | int | موضع بدء البحث. |
| count | int | العدد. |

**Returns:**
عدد صحيح - الـ `int`.
### indexOf(String value) {#indexOf-java.lang.String-}
```
public final int indexOf(String value)
```


يعيد الفهرس الصفري للظهور الأول للسلسلة المحددة في هذا الكائن.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | القيمة. |

**Returns:**
عدد صحيح - الـ `int`.
### indexOf(String value, int startIndex) {#indexOf-java.lang.String-int-}
```
public final int indexOf(String value, int startIndex)
```


يعيد الفهرس الصفري للظهور الأول للسلسلة المحددة في هذه الحالة. يبدأ البحث عند موضع حرف محدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | القيمة. |
| startIndex | int | موضع بدء البحث. |

**Returns:**
عدد صحيح - الـ `int`.
### indexOf(String value, int startIndex, int count) {#indexOf-java.lang.String-int-int-}
```
public final int indexOf(String value, int startIndex, int count)
```


يعيد الفهرس الصفري للظهور الأول للسلسلة المحددة في هذه الحالة. يبدأ البحث عند موضع حرف محدد ويفحص عددًا محددًا من مواضع الأحرف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | القيمة. |
| startIndex | int | موضع بدء البحث. |
| count | int | العدد. |

**Returns:**
عدد صحيح - الـ `int`.
### indexOf(String value, int startIndex, int count, short comparisonType) {#indexOf-java.lang.String-int-int-short-}
```
public final int indexOf(String value, int startIndex, int count, short comparisonType)
```


يعيد الفهرس الصفري للظهور الأول للسلسلة المحددة في الكائن الحالي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | القيمة. |
| startIndex | int | موضع بدء البحث. |
| count | int | العدد. |
| comparisonType | short | نوع البحث الذي سيُستخدم للسلسلة المحددة |

**Returns:**
عدد صحيح - الـ `int`.
### indexOf(String value, short comparisonType) {#indexOf-java.lang.String-short-}
```
public final int indexOf(String value, short comparisonType)
```


يعيد الفهرس الصفري للظهور الأول للسلسلة المحددة في الحالة الحالية. يحدد أحد المعاملات نوع البحث الذي سيُستخدم للسلسلة المحددة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | القيمة. |
| comparisonType | short | نوع البحث الذي سيُستخدم للسلسلة المحددة |

**Returns:**
عدد صحيح - الـ `int`.
### indexOf_Rename_Namesake(String value, int startIndex, short comparisonType) {#indexOf-Rename-Namesake-java.lang.String-int-short-}
```
public final int indexOf_Rename_Namesake(String value, int startIndex, short comparisonType)
```


يعيد الفهرس الصفري للظهور الأول للسلسلة المحددة في الحالة الحالية. تحدد المعاملات موضع بدء البحث في السلسلة الحالية ونوع البحث الذي سيُستخدم للسلسلة المحددة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String | القيمة. |
| startIndex | int | موضع بدء البحث. |
| comparisonType | short | نوع البحث الذي سيُستخدم للسلسلة المحددة |

**Returns:**
عدد صحيح - الـ `int`.
### insert(int startIndex, String value) {#insert-int-java.lang.String-}
```
public final RichText insert(int startIndex, String value)
```


يدرج سلسلة محددة في موضع فهرس محدد في هذا الكائن.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| startIndex | int | مؤشر البدء. |
| القيمة | java.lang.String | القيمة. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### insert(int startIndex, String value, TextStyle style) {#insert-int-java.lang.String-com.aspose.note.TextStyle-}
```
public final RichText insert(int startIndex, String value, TextStyle style)
```


يدرج سلسلة محددة مع نمط محدد في موضع فهرس محدد في هذا الكائن.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| startIndex | int | مؤشر البدء. |
| القيمة | java.lang.String | القيمة. |
| style | [TextStyle](../../com.aspose.note/textstyle) | النمط. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<Character> iterator()
```




**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;java.lang.Character&gt;
### remove(int startIndex) {#remove-int-}
```
public final RichText remove(int startIndex)
```


يزيل جميع الأحرف في الكائن الحالي، بدءًا من موضع محدد ومتابعة حتى الموضع الأخير.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| startIndex | int | مؤشر البدء. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### remove(int startIndex, int count) {#remove-int-int-}
```
public final RichText remove(int startIndex, int count)
```


يزيل عددًا محددًا من الأحرف في الكائن الحالي بدءًا من موضع محدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| startIndex | int | مؤشر البدء. |
| count | int | العدد. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### replace(char oldChar, char newChar) {#replace-char-char-}
```
public final RichText replace(char oldChar, char newChar)
```


يستبدل جميع ظهورات حرف Unicode محدد في هذا الكائن بحرف Unicode آخر محدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| oldChar | char | الحرف القديم. |
| newChar | char | الحرف الجديد. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### replace(String oldValue, String newValue) {#replace-java.lang.String-java.lang.String-}
```
public final RichText replace(String oldValue, String newValue)
```


يستبدل جميع ظهورات سلسلة محددة في الكائن الحالي بسلسلة أخرى محددة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| oldValue | java.lang.String | القيمة القديمة. |
| newValue | java.lang.String | القيمة الجديدة. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### replace(String oldValue, String newValue, TextStyle style) {#replace-java.lang.String-java.lang.String-com.aspose.note.TextStyle-}
```
public final RichText replace(String oldValue, String newValue, TextStyle style)
```


يستبدل جميع ظهورات سلسلة محددة في الكائن الحالي بسلسلة أخرى محددة بنمط محدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| oldValue | java.lang.String | القيمة القديمة. |
| newValue | java.lang.String | القيمة الجديدة. |
| style | [TextStyle](../../com.aspose.note/textstyle) | نمط القيمة الجديدة. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### setAlignment(int value) {#setAlignment-int-}
```
public void setAlignment(int value)
```


يضبط المحاذاة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


يضبط وقت التعديل الأخير.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.Date |  |

### setLineSpacing(float value) {#setLineSpacing-float-}
```
public void setLineSpacing(float value)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | float |  |

### setLineSpacing(Float value) {#setLineSpacing-java.lang.Float-}
```
public void setLineSpacing(Float value)
```


يضبط تباعد الأسطر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.Float |  |

### setParagraphStyle(ParagraphStyle value) {#setParagraphStyle-com.aspose.note.ParagraphStyle-}
```
public final void setParagraphStyle(ParagraphStyle value)
```


يضبط نمط الفقرة. تُستخدم هذه الإعدادات إذا لم يكن هناك كائن TextStyle مطابق في مجموعة [getStyles](../../com.aspose.note/richtext\#getStyles) أو إذا لم يحدد هذا الكائن الإعداد المطلوب.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [ParagraphStyle](../../com.aspose.note/paragraphstyle) |  |

### setSpaceAfter(float value) {#setSpaceAfter-float-}
```
public void setSpaceAfter(float value)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | float |  |

### setSpaceAfter(Float value) {#setSpaceAfter-java.lang.Float-}
```
public void setSpaceAfter(Float value)
```


يضبط الحد الأدنى للمسافة بعد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.Float |  |

### setSpaceBefore(float value) {#setSpaceBefore-float-}
```
public void setSpaceBefore(float value)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | float |  |

### setSpaceBefore(Float value) {#setSpaceBefore-java.lang.Float-}
```
public void setSpaceBefore(Float value)
```


يضبط الحد الأدنى للمسافة قبل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.Float |  |

### setText(String value) {#setText-java.lang.String-}
```
public final void setText(String value)
```


يضبط النص. يجب ألا تحتوي السلسلة على أي أحرف ذات القيمة 10 (سطر جديد).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### trim() {#trim--}
```
public final RichText trim()
```


يزيل جميع أحرف المسافات البيضاء في البداية والنهاية.

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trim(char trimChar) {#trim-char-}
```
public final RichText trim(char trimChar)
```


يزيل جميع حالات الحرف في البداية والنهاية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| trimChar | char | حرف القطع. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trim(char[] trimChars) {#trim-char...-}
```
public final RichText trim(char[] trimChars)
```


يزيل جميع تكرارات مجموعة الأحرف المحددة في مصفوفة في البداية والنهاية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| trimChars | char[] | حروف القطع. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimEnd() {#trimEnd--}
```
public final RichText trimEnd()
```


يزيل جميع أحرف المسافات البيضاء في النهاية.

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimEnd(char trimChar) {#trimEnd-char-}
```
public final RichText trimEnd(char trimChar)
```


يزيل جميع تكرارات الحرف في النهاية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| trimChar | char | حرف القطع. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimEnd(char[] trimChars) {#trimEnd-char...-}
```
public final RichText trimEnd(char[] trimChars)
```


يزيل جميع تكرارات مجموعة الأحرف المحددة في مصفوفة في النهاية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| trimChars | char[] | حروف القطع. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimStart() {#trimStart--}
```
public final RichText trimStart()
```


يزيل جميع أحرف المسافات البيضاء في البداية.

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimStart(char trimChar) {#trimStart-char-}
```
public final RichText trimStart(char trimChar)
```


يزيل جميع تكرارات الحرف المحدد في البداية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| trimChar | char | حرف القطع. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimStart(char[] trimChars) {#trimStart-char...-}
```
public final RichText trimStart(char[] trimChars)
```


يزيل جميع تكرارات مجموعة الأحرف المحددة في مصفوفة في البداية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| trimChars | char[] | حروف القطع. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
