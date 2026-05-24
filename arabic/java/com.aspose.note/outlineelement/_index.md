---
title: "OutlineElement"
second_title: "مرجع Aspose.Note for Java API"
description: "يمثل OutlineElement."
type: docs
weight: 67
url: /ar/java/com.aspose.note/outlineelement/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode, com.aspose.note.IndentatedNode

**All Implemented Interfaces:**
[com.aspose.note.IOutlineChildNode](../../com.aspose.note/ioutlinechildnode), [com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode)
```
public final class OutlineElement extends IndentatedNode<IOutlineElementChildNode,OutlineElement> implements IOutlineChildNode, IOutlineElementChildNode
```

يمثل OutlineElement.
## المنشئات

| المنشئ | الوصف |
| --- | --- |
| [OutlineElement()](#OutlineElement--) | يُنشئ مثيلاً جديدًا من الفئة `OutlineElement`. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | يقبل زائر العقدة. |
| [getAuthorMostRecent()](#getAuthorMostRecent--) | يحصل على المؤلف الأحدث لعنصر المخطط. |
| [getAuthorOriginal()](#getAuthorOriginal--) | يحصل على المؤلف الأصلي لعنصر المخطط. |
| [getCreationTime()](#getCreationTime--) | يحصل أو يعيّن وقت الإنشاء. |
| [getLastModifiedTime()](#getLastModifiedTime--) | يحصل أو يضبط وقت التعديل الأخير. |
| [getNumberList()](#getNumberList--) | يحصل أو يعيّن النمط لرأس القائمة المرقمة. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | يحصل أو يعيّن وقت الإنشاء. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | يحصل أو يضبط وقت التعديل الأخير. |
| [setNumberList(NumberList value)](#setNumberList-com.aspose.note.NumberList-) | يحصل أو يعيّن النمط لرأس القائمة المرقمة. |
### OutlineElement() {#OutlineElement--}
```
public OutlineElement()
```


يُنشئ مثيلاً جديدًا من الفئة `OutlineElement`.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


يقبل زائر العقدة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | الكائن من فئة مشتقة من `DocumentVisitor`. |

### getAuthorMostRecent() {#getAuthorMostRecent--}
```
public final String getAuthorMostRecent()
```


يحصل على المؤلف الأحدث لعنصر المخطط.

القيمة: المؤلف الأحدث.

**Returns:**
java.lang.String
### getAuthorOriginal() {#getAuthorOriginal--}
```
public final String getAuthorOriginal()
```


يحصل على المؤلف الأصلي لعنصر المخطط.

القيمة: المؤلف الأصلي.

**Returns:**
java.lang.String
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
### getNumberList() {#getNumberList--}
```
public NumberList getNumberList()
```


يحصل أو يعيّن النمط لرأس القائمة المرقمة.

**Returns:**
[NumberList](../../com.aspose.note/numberlist)
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

### setNumberList(NumberList value) {#setNumberList-com.aspose.note.NumberList-}
```
public void setNumberList(NumberList value)
```


يحصل أو يعيّن النمط لرأس القائمة المرقمة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [NumberList](../../com.aspose.note/numberlist) |  |

