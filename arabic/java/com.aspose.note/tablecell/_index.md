---
title: "TableCell"
second_title: "مرجع Aspose.Note for Java API"
description: "يمثل خلية جدول."
type: docs
weight: 88
url: /ar/java/com.aspose.note/tablecell/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode, com.aspose.note.IndentatedNode
```
public final class TableCell extends IndentatedNode<IOutlineChildNode,TableCell>
```

يمثل خلية جدول.
## المنشئات

| المنشئ | الوصف |
| --- | --- |
| [TableCell()](#TableCell--) | ينشئ مثيلاً جديداً من الفئة `TableCell`. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | يقبل زائر العقدة. |
| [getBackgroundColor()](#getBackgroundColor--) | يحصل على لون الخلفية. |
| [getInternalIndentPosition()](#getInternalIndentPosition--) |  |
| [getLastModifiedTime()](#getLastModifiedTime--) | يحصل أو يضبط وقت التعديل الأخير. |
| [getMaxWidth()](#getMaxWidth--) | يحصل على أقصى عرض. |
| [setBackgroundColor(Color value)](#setBackgroundColor-java.awt.Color-) | يضبط لون الخلفية. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | يحصل أو يضبط وقت التعديل الأخير. |
### TableCell() {#TableCell--}
```
public TableCell()
```


ينشئ مثيلاً جديداً من الفئة `TableCell`.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


يقبل زائر العقدة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | الكائن من فئة مشتقة من `DocumentVisitor`. |

### getBackgroundColor() {#getBackgroundColor--}
```
public Color getBackgroundColor()
```


يحصل على لون الخلفية.

**Returns:**
java.awt.Color
### getInternalIndentPosition() {#getInternalIndentPosition--}
```
public int getInternalIndentPosition()
```


يحصل على عدد العناصر التي يجب جمعها في مصفوفة RgOutlineIndentDistance للحصول على حجم المسافة البادئة.

**Returns:**
int
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


يحصل أو يضبط وقت التعديل الأخير.

**Returns:**
java.util.Date
### getMaxWidth() {#getMaxWidth--}
```
public float getMaxWidth()
```


يحصل على أقصى عرض.

**Returns:**
float
### setBackgroundColor(Color value) {#setBackgroundColor-java.awt.Color-}
```
public void setBackgroundColor(Color value)
```


يضبط لون الخلفية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.awt.Color |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


يحصل أو يضبط وقت التعديل الأخير.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.Date |  |

