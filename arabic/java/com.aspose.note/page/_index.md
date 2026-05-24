---
title: "Page"
second_title: "مرجع Aspose.Note for Java API"
description: "يمثل صفحة."
type: docs
weight: 69
url: /ar/java/com.aspose.note/page/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode
```
public final class Page extends CompositeNode<IPageChildNode>
```

يمثل صفحة.
## المنشئات

| المنشئ | الوصف |
| --- | --- |
| [Page()](#Page--) | ينشئ مثيلًا جديدًا للفئة `Page`. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | يقبل زائر العقدة. |
| [deepClone()](#deepClone--) | ينسخ الصفحة. |
| [deepClone(boolean cloneHistory)](#deepClone-boolean-) | ينسخ الصفحة. |
| [getAuthor()](#getAuthor--) | يحصل أو يعيّن المؤلف. |
| [getBackgroundColor()](#getBackgroundColor--) | يحصل أو يعيّن لون خلفية الصفحة. |
| [getCreationTime()](#getCreationTime--) | يحصل أو يعيّن وقت الإنشاء. |
| [getLastModifiedTime()](#getLastModifiedTime--) | يحصل أو يضبط وقت التعديل الأخير. |
| [getLevel()](#getLevel--) | يحصل أو يعيّن المستوى. |
| [getMargin()](#getMargin--) | يحصل أو يعيّن الهامش. |
| [getPageContentRevisionSummary()](#getPageContentRevisionSummary--) | يحصل أو يعيّن ملخص المراجعة للصفحة وعقدها الفرعية. |
| [getPageLayoutSize()](#getPageLayoutSize--) | يحصل على حجم تخطيط الصفحة المعروض في المحرر. |
| [getSizeType()](#getSizeType--) | يحصل أو يعيّن نوع حجم الصفحة. |
| [getTitle()](#getTitle--) | يحصل أو يعيّن العنوان. |
| [isConflictPage()](#isConflictPage--) | يحصل أو يعيّن قيمة تشير إلى ما إذا كانت هذه الصفحة صفحة تعارض. |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | يحصل أو يعيّن المؤلف. |
| [setBackgroundColor(Color value)](#setBackgroundColor-java.awt.Color-) | يحصل أو يعيّن لون خلفية الصفحة. |
| [setConflictPage(boolean value)](#setConflictPage-boolean-) | يحصل أو يعيّن قيمة تشير إلى ما إذا كانت هذه الصفحة صفحة تعارض. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | يحصل أو يعيّن وقت الإنشاء. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | يحصل أو يضبط وقت التعديل الأخير. |
| [setLevel(byte value)](#setLevel-byte-) | يحصل أو يعيّن المستوى. |
| [setMargin(Margins value)](#setMargin-com.aspose.note.Margins-) | يحصل أو يعيّن الهامش. |
| [setPageContentRevisionSummary(RevisionSummary value)](#setPageContentRevisionSummary-com.aspose.note.RevisionSummary-) | يحصل أو يعيّن ملخص المراجعة للصفحة وعقدها الفرعية. |
| [setPageLayoutSize(Dimension2D value)](#setPageLayoutSize-java.awt.geom.Dimension2D-) | يعيّن حجم تخطيط الصفحة المعروض في المحرر. |
| [setSizeType(int value)](#setSizeType-int-) | يحصل أو يعيّن نوع حجم الصفحة. |
| [setTitle(Title value)](#setTitle-com.aspose.note.Title-) | يحصل أو يعيّن العنوان. |
### Page() {#Page--}
```
public Page()
```


ينشئ مثيلًا جديدًا للفئة `Page`.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


يقبل زائر العقدة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | الكائن من فئة مشتقة من `DocumentVisitor`. |

### deepClone() {#deepClone--}
```
public final Page deepClone()
```


ينسخ الصفحة.

**Returns:**
[Page](../../com.aspose.note/page) - A clone of the page.
### deepClone(boolean cloneHistory) {#deepClone-boolean-}
```
public final Page deepClone(boolean cloneHistory)
```


ينسخ الصفحة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| cloneHistory | boolean | يحدد ما إذا كان يجب استنساخ تاريخ الصفحة.. |

**Returns:**
[Page](../../com.aspose.note/page) - A clone of the page.
### getAuthor() {#getAuthor--}
```
public String getAuthor()
```


يحصل أو يعيّن المؤلف.

**Returns:**
java.lang.String
### getBackgroundColor() {#getBackgroundColor--}
```
public final Color getBackgroundColor()
```


يحصل أو يعيّن لون خلفية الصفحة.

**Returns:**
java.awt.Color
### getCreationTime() {#getCreationTime--}
```
public Date getCreationTime()
```


يحصل أو يعيّن وقت الإنشاء.

**Returns:**
java.util.Date
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


يحصل أو يضبط وقت التعديل الأخير.

**Returns:**
java.util.Date
### getLevel() {#getLevel--}
```
public byte getLevel()
```


يحصل أو يعيّن المستوى.

**Returns:**
byte
### getMargin() {#getMargin--}
```
public Margins getMargin()
```


يحصل أو يعيّن الهامش.

**Returns:**
[Margins](../../com.aspose.note/margins)
### getPageContentRevisionSummary() {#getPageContentRevisionSummary--}
```
public RevisionSummary getPageContentRevisionSummary()
```


يحصل أو يعيّن ملخص المراجعة للصفحة وعقدها الفرعية.

**Returns:**
[RevisionSummary](../../com.aspose.note/revisionsummary)
### getPageLayoutSize() {#getPageLayoutSize--}
```
public final Dimension2D getPageLayoutSize()
```


يحصل على حجم تخطيط الصفحة المعروض في المحرر.

--------------------

تُستخدم هذه القيمة بواسطة تطبيق Microsoft OneNote لعرض تخطيط الصفحة الأساسي عند فتح المستند. لا تؤثر على الطباعة وحفظ المستند على أي حال. عندما يتم تعيين خاصية Page.SizeType إلى PageSizeType.SizeByContent، تُعيد هذه الخاصية الحجم الفعلي للمحتوى.

**Returns:**
java.awt.geom.Dimension2D
### getSizeType() {#getSizeType--}
```
public final int getSizeType()
```


يحصل أو يعيّن نوع حجم الصفحة.

--------------------

بشكل افتراضي، يتم تغيير حجم الصفحة تلقائيًا. القيمة الافتراضية هي [PageSizeType.SizeByContent](../../com.aspose.note/pagesizetype\#SizeByContent).

**Returns:**
int
### getTitle() {#getTitle--}
```
public Title getTitle()
```


يحصل أو يعيّن العنوان.

القيمة: الـ `Title`.

**Returns:**
[Title](../../com.aspose.note/title)
### isConflictPage() {#isConflictPage--}
```
public final boolean isConflictPage()
```


يحصل أو يعيّن قيمة تشير إلى ما إذا كانت هذه الصفحة صفحة تعارض.

--------------------

تظهر صفحة التعارض عندما يحاول مستخدمان تحديث نفس المحتوى. في هذه الحالة تُكتب تغييرات المستخدم الأول كالمعتاد. لكن لا يمكن دمج تغييرات المستخدم الآخر. لذا يتم إنشاء نسخة من الصفحة وتحديدها كتعارض.

في هذا الإصدار يتم حل التعارضات لصالح تغييرات المستخدم الأول. لذلك إذا كان للمستند صفحات تعارض فستظهر في السجل ولكن سيتم تخطيها عند الحفظ. يمكن إعادة تعيين هذه العلامة لحفظ هذه الصفحات في السجل كصفحات عادية.

يمكن العثور على مثال مفصل للتعامل مع صفحة التعارض في الوثائق عبر الإنترنت.

**Returns:**
boolean
### setAuthor(String value) {#setAuthor-java.lang.String-}
```
public void setAuthor(String value)
```


يحصل أو يعيّن المؤلف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setBackgroundColor(Color value) {#setBackgroundColor-java.awt.Color-}
```
public final void setBackgroundColor(Color value)
```


يحصل أو يعيّن لون خلفية الصفحة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.awt.Color |  |

### setConflictPage(boolean value) {#setConflictPage-boolean-}
```
public final void setConflictPage(boolean value)
```


يحصل أو يعيّن قيمة تشير إلى ما إذا كانت هذه الصفحة صفحة تعارض.

--------------------

تظهر صفحة التعارض عندما يحاول مستخدمان تحديث نفس المحتوى. في هذه الحالة تُكتب تغييرات المستخدم الأول كالمعتاد. لكن لا يمكن دمج تغييرات المستخدم الآخر. لذا يتم إنشاء نسخة من الصفحة وتحديدها كتعارض.

في هذا الإصدار يتم حل التعارضات لصالح تغييرات المستخدم الأول. لذلك إذا كان للمستند صفحات تعارض فستظهر في السجل ولكن سيتم تخطيها عند الحفظ. يمكن إعادة تعيين هذه العلامة لحفظ هذه الصفحات في السجل كصفحات عادية.

يمكن العثور على مثال مفصل للتعامل مع صفحة التعارض في الوثائق عبر الإنترنت.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public void setCreationTime(Date value)
```


يحصل أو يعيّن وقت الإنشاء.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.Date |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


يحصل أو يضبط وقت التعديل الأخير.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.Date |  |

### setLevel(byte value) {#setLevel-byte-}
```
public void setLevel(byte value)
```


يحصل أو يعيّن المستوى.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | byte |  |

### setMargin(Margins value) {#setMargin-com.aspose.note.Margins-}
```
public void setMargin(Margins value)
```


يحصل أو يعيّن الهامش.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Margins](../../com.aspose.note/margins) |  |

### setPageContentRevisionSummary(RevisionSummary value) {#setPageContentRevisionSummary-com.aspose.note.RevisionSummary-}
```
public void setPageContentRevisionSummary(RevisionSummary value)
```


يحصل أو يعيّن ملخص المراجعة للصفحة وعقدها الفرعية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [RevisionSummary](../../com.aspose.note/revisionsummary) |  |

### setPageLayoutSize(Dimension2D value) {#setPageLayoutSize-java.awt.geom.Dimension2D-}
```
public final void setPageLayoutSize(Dimension2D value)
```


يعيّن حجم تخطيط الصفحة المعروض في المحرر.

--------------------

تُستخدم هذه القيمة بواسطة تطبيق Microsoft OneNote لعرض تخطيط الصفحة الأساسي عند فتح المستند. لا تؤثر على الطباعة وحفظ المستند على أي حال. عندما يتم تعيين خاصية Page.SizeType إلى PageSizeType.SizeByContent، تُعيد هذه الخاصية الحجم الفعلي للمحتوى.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.awt.geom.Dimension2D |  |

### setSizeType(int value) {#setSizeType-int-}
```
public final void setSizeType(int value)
```


يحصل أو يعيّن نوع حجم الصفحة.

--------------------

بشكل افتراضي، يتم تغيير حجم الصفحة تلقائيًا. القيمة الافتراضية هي [PageSizeType.SizeByContent](../../com.aspose.note/pagesizetype\#SizeByContent).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setTitle(Title value) {#setTitle-com.aspose.note.Title-}
```
public void setTitle(Title value)
```


يحصل أو يعيّن العنوان.

القيمة: الـ `Title`.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Title](../../com.aspose.note/title) |  |

