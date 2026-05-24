---
title: "PageHistory"
second_title: "مرجع Aspose.Note for Java API"
description: "يمثل تاريخ الصفحة."
type: docs
weight: 70
url: /ar/java/com.aspose.note/pagehistory/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.ms.System.Collections.Generic.IGenericList
```
public class PageHistory implements System.Collections.Generic.IGenericList<Page>
```

يمثل تاريخ الصفحة.
## المنشئات

| المنشئ | الوصف |
| --- | --- |
| [PageHistory(Page page)](#PageHistory-com.aspose.note.Page-) | يُهيئ مثالًا جديدًا من الفئة `PageHistory`. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [addItem(Page item)](#addItem-com.aspose.note.Page-) | يضيف نسخة الصفحة إلى نهاية `PageHistory`. |
| [addRange(System.Collections.Generic.IGenericEnumerable&lt;Page&gt; items)](#addRange-com.aspose.ms.System.Collections.Generic.IGenericEnumerable-com.aspose.note.Page--) | يضيف نسخ الصفحات إلى نهاية `PageHistory`. |
| [clear()](#clear--) | يمسح سجل الصفحات. |
| [containsItem(Page item)](#containsItem-com.aspose.note.Page-) | يحدد ما إذا كان سجل الصفحات يحتوي على نسخة الصفحة. |
| [copyToTArray(Page[] array, int arrayIndex)](#copyToTArray-com.aspose.note.Page---int-) | ينسخ إصدارات الصفحة إلى مصفوفة، بدءًا من فهرس معين.. |
| [getCurrent()](#getCurrent--) | يحصل على إصدار الصفحة الحالي. |
| [get_Item(int index)](#get-Item-int-) | يحصل أو يضبط إصدار الصفحة في الفهرس المحدد لـ `PageHistory`. |
| [indexOfItem(Page item)](#indexOfItem-com.aspose.note.Page-) | يحدد فهرس إصدار صفحة معين في تاريخ الصفحات. |
| [insertItem(int index, Page item)](#insertItem-int-com.aspose.note.Page-) | يدرج إصدار صفحة في تاريخ الصفحات. |
| [isReadOnly()](#isReadOnly--) | يحصل على قيمة تشير إلى ما إذا كان تاريخ الصفحات للقراءة فقط. |
| [iterator()](#iterator--) | يعيد عدادًا يتنقل عبر العقد الفرعية لـ `PageHistory`. |
| [removeAt(int index)](#removeAt-int-) | يزيل إصدار الصفحة في الفهرس المحدد لـ `PageHistory`. |
| [removeItem(Page item)](#removeItem-com.aspose.note.Page-) | يزيل إصدار الصفحة من `PageHistory`. |
| [removeRange(int index, int count)](#removeRange-int-int-) | يزيل نطاقًا من إصدارات الصفحة من `PageHistory`. |
| [set_Item(int index, Page value)](#set-Item-int-com.aspose.note.Page-) | يحصل أو يضبط إصدار الصفحة في الفهرس المحدد لـ `PageHistory`. |
| [size()](#size--) | يحصل على عدد إصدارات الصفحة في تاريخ الصفحات. |
### PageHistory(Page page) {#PageHistory-com.aspose.note.Page-}
```
public PageHistory(Page page)
```


يُهيئ مثالًا جديدًا من الفئة `PageHistory`.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | إصدار الصفحة الحالي. |

### addItem(Page item) {#addItem-com.aspose.note.Page-}
```
public void addItem(Page item)
```


يضيف نسخة الصفحة إلى نهاية `PageHistory`.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | إصدار الصفحة. |

### addRange(System.Collections.Generic.IGenericEnumerable&lt;Page&gt; items) {#addRange-com.aspose.ms.System.Collections.Generic.IGenericEnumerable-com.aspose.note.Page--}
```
public void addRange(System.Collections.Generic.IGenericEnumerable<Page> items)
```


يضيف نسخ الصفحات إلى نهاية `PageHistory`.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| العناصر | com.aspose.ms.System.Collections.Generic.IGenericEnumerable&lt;com.aspose.note.Page&gt; | مجموعة `IEnumerable\{Page\}` لإصدارات الصفحة. |

### clear() {#clear--}
```
public void clear()
```


يمسح سجل الصفحات.

### containsItem(Page item) {#containsItem-com.aspose.note.Page-}
```
public boolean containsItem(Page item)
```


يحدد ما إذا كان سجل الصفحات يحتوي على نسخة الصفحة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | إصدار الصفحة. |

**Returns:**
منطقي - الـ `bool`.
### copyToTArray(Page[] array, int arrayIndex) {#copyToTArray-com.aspose.note.Page---int-}
```
public void copyToTArray(Page[] array, int arrayIndex)
```


ينسخ إصدارات الصفحة إلى مصفوفة، بدءًا من فهرس معين..

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| array | [Page\[\]](../../com.aspose.note/page) | المصفوفة الهدف. |
| arrayIndex | int | فهرس المصفوفة. |

### getCurrent() {#getCurrent--}
```
public Page getCurrent()
```


يحصل على إصدار الصفحة الحالي.

**Returns:**
[Page](../../com.aspose.note/page)
### get_Item(int index) {#get-Item-int-}
```
public Page get_Item(int index)
```


يحصل أو يضبط إصدار الصفحة في الفهرس المحدد لـ `PageHistory`.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| index | int | الفهرس. |

**Returns:**
[Page](../../com.aspose.note/page) - The page version.
### indexOfItem(Page item) {#indexOfItem-com.aspose.note.Page-}
```
public int indexOfItem(Page item)
```


يحدد فهرس إصدار صفحة معين في تاريخ الصفحات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | إصدار الصفحة. |

**Returns:**
عدد صحيح - الـ `int`.
### insertItem(int index, Page item) {#insertItem-int-com.aspose.note.Page-}
```
public void insertItem(int index, Page item)
```


يدرج إصدار صفحة في تاريخ الصفحات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| index | int | الفهرس. |
| item | [Page](../../com.aspose.note/page) | إصدار الصفحة. |

### isReadOnly() {#isReadOnly--}
```
public boolean isReadOnly()
```


يحصل على قيمة تشير إلى ما إذا كان تاريخ الصفحات للقراءة فقط.

**Returns:**
boolean
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<Page> iterator()
```


يعيد عدادًا يتنقل عبر العقد الفرعية لـ `PageHistory`.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.note.Page&gt; - الـ `IEnumerator`.
### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


يزيل إصدار الصفحة في الفهرس المحدد لـ `PageHistory`.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| index | int | الفهرس. |

### removeItem(Page item) {#removeItem-com.aspose.note.Page-}
```
public boolean removeItem(Page item)
```


يزيل إصدار الصفحة من `PageHistory`.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | إصدار الصفحة. |

**Returns:**
منطقي - الـ `bool`.
### removeRange(int index, int count) {#removeRange-int-int-}
```
public void removeRange(int index, int count)
```


يزيل نطاقًا من إصدارات الصفحة من `PageHistory`.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| index | int | الفهرس. |
| count | int | العدد. |

### set_Item(int index, Page value) {#set-Item-int-com.aspose.note.Page-}
```
public void set_Item(int index, Page value)
```


يحصل أو يضبط إصدار الصفحة في الفهرس المحدد لـ `PageHistory`.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| index | int | الفهرس. |
| value | [Page](../../com.aspose.note/page) |  |

### size() {#size--}
```
public int size()
```


يحصل على عدد إصدارات الصفحة في تاريخ الصفحات.

**Returns:**
int
