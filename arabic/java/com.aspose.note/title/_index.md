---
title: "Title"
second_title: "مرجع Aspose.Note for Java API"
description: "يمثل عنوانًا."
type: docs
weight: 95
url: /ar/java/com.aspose.note/title/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase)

**All Implemented Interfaces:**
com.aspose.note.ICompositeNodeT, [com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode)
```
public final class Title extends CompositeNodeBase implements ICompositeNodeT<RichText>, IPageChildNode
```

يمثل عنوانًا.
## المنشئات

| المنشئ | الوصف |
| --- | --- |
| [Title()](#Title--) | ينشئ مثيلًا جديدًا من الفئة `Title`. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [&lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass)](#-T1-getChildNodes-java.lang.Class-T1--) | احصل على جميع العقد الفرعية وفقًا لنوع العقدة. |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | يقبل زائر العقدة. |
| [getChildNodes(int type)](#getChildNodes-int-) |  |
| [getHorizontalOffset()](#getHorizontalOffset--) | يحصل أو يضبط الإزاحة الأفقية. |
| [getLastModifiedTime()](#getLastModifiedTime--) | يحصل أو يضبط وقت التعديل الأخير. |
| [getTitleDate()](#getTitleDate--) | يحصل أو يضبط تمثيلًا نصيًا للتاريخ في العنوان. |
| [getTitleText()](#getTitleText--) | يحصل أو يضبط نص العنوان. |
| [getTitleTime()](#getTitleTime--) | يحصل أو يضبط تمثيلًا نصيًا للوقت في العنوان. |
| [getVerticalOffset()](#getVerticalOffset--) | يحصل أو يضبط الإزاحة العمودية. |
| [isComposite()](#isComposite--) | يحصل على قيمة تشير إلى ما إذا كان هذا العنصر مركبًا. |
| [iterator()](#iterator--) | يرجع عدادًا يتنقل عبر العقد الفرعية للـ [Title](../../com.aspose.note/title). |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | يحصل أو يضبط الإزاحة الأفقية. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | يحصل أو يضبط وقت التعديل الأخير. |
| [setTitleDate(RichText value)](#setTitleDate-com.aspose.note.RichText-) | يحصل أو يضبط تمثيلًا نصيًا للتاريخ في العنوان. |
| [setTitleText(RichText value)](#setTitleText-com.aspose.note.RichText-) | يحصل أو يضبط نص العنوان. |
| [setTitleTime(RichText value)](#setTitleTime-com.aspose.note.RichText-) | يحصل أو يضبط تمثيلًا نصيًا للوقت في العنوان. |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | يحصل أو يضبط الإزاحة العمودية. |
### Title() {#Title--}
```
public Title()
```


ينشئ مثيلًا جديدًا من الفئة `Title`.

### &lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass) {#-T1-getChildNodes-java.lang.Class-T1--}
```
public List<T1> <T1>getChildNodes(Class<T1> typeParameterClass)
```


احصل على جميع العقد الفرعية وفقًا لنوع العقدة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| typeParameterClass | java.lang.Class&lt;T1&gt; |  |

**Returns:**
java.util.List&lt;T1&gt; - قائمة بالعقد الفرعية.

`T1`: نوع العناصر في القائمة المعادة.
### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


يقبل زائر العقدة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | الكائن من فئة مشتقة من `DocumentVisitor`. |

### getChildNodes(int type) {#getChildNodes-int-}
```
public List<INode> getChildNodes(int type)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| النوع | int |  |

**Returns:**
java.util.List&lt;com.aspose.note.INode&gt;
### getHorizontalOffset() {#getHorizontalOffset--}
```
public final float getHorizontalOffset()
```


يحصل أو يضبط الإزاحة الأفقية.

**Returns:**
float
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


يحصل أو يضبط وقت التعديل الأخير.

**Returns:**
java.util.Date
### getTitleDate() {#getTitleDate--}
```
public final RichText getTitleDate()
```


يحصل أو يضبط تمثيلًا نصيًا للتاريخ في العنوان.

**Returns:**
[RichText](../../com.aspose.note/richtext)
### getTitleText() {#getTitleText--}
```
public RichText getTitleText()
```


يحصل أو يضبط نص العنوان.

**Returns:**
[RichText](../../com.aspose.note/richtext)
### getTitleTime() {#getTitleTime--}
```
public final RichText getTitleTime()
```


يحصل أو يضبط تمثيلًا نصيًا للوقت في العنوان.

**Returns:**
[RichText](../../com.aspose.note/richtext)
### getVerticalOffset() {#getVerticalOffset--}
```
public final float getVerticalOffset()
```


يحصل أو يضبط الإزاحة العمودية.

**Returns:**
float
### isComposite() {#isComposite--}
```
public boolean isComposite()
```


يحصل على قيمة تشير إلى ما إذا كان هذا العنصر مركبًا. إذا كان صحيحًا يمكن للعنصر أن يحتوي على عقد فرعية.

**Returns:**
boolean
### iterator() {#iterator--}
```
public final System.Collections.Generic.IGenericEnumerator<RichText> iterator()
```


يرجع عدادًا يتنقل عبر العقد الفرعية للـ [Title](../../com.aspose.note/title).

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.note.RichText&gt; - الـ IEnumerator.
### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public final void setHorizontalOffset(float value)
```


يحصل أو يضبط الإزاحة الأفقية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | float |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


يحصل أو يضبط وقت التعديل الأخير.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.Date |  |

### setTitleDate(RichText value) {#setTitleDate-com.aspose.note.RichText-}
```
public final void setTitleDate(RichText value)
```


يحصل أو يضبط تمثيلًا نصيًا للتاريخ في العنوان.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [RichText](../../com.aspose.note/richtext) |  |

### setTitleText(RichText value) {#setTitleText-com.aspose.note.RichText-}
```
public final void setTitleText(RichText value)
```


يحصل أو يضبط نص العنوان.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [RichText](../../com.aspose.note/richtext) |  |

### setTitleTime(RichText value) {#setTitleTime-com.aspose.note.RichText-}
```
public final void setTitleTime(RichText value)
```


يحصل أو يضبط تمثيلًا نصيًا للوقت في العنوان.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [RichText](../../com.aspose.note/richtext) |  |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public final void setVerticalOffset(float value)
```


يحصل أو يضبط الإزاحة العمودية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | float |  |

