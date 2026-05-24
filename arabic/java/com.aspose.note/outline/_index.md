---
title: "المخطط"
second_title: "مرجع Aspose.Note for Java API"
description: "يمثل مخططًا."
type: docs
weight: 66
url: /ar/java/com.aspose.note/outline/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode, com.aspose.note.IndentatedNode

**All Implemented Interfaces:**
[com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode)
```
public final class Outline extends IndentatedNode<IOutlineChildNode,Outline> implements IPageChildNode
```

يمثل مخططًا.
## المنشئات

| المنشئ | الوصف |
| --- | --- |
| [Outline()](#Outline--) | يُنشئ مثيلًا جديدًا من الفئة [Outline](../../com.aspose.note/outline). |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | يقبل زائر العقدة. |
| [getDescendantsCannotBeMoved()](#getDescendantsCannotBeMoved--) | يحصل على ما إذا كان يمكن نقل سلالف المخطط. |
| [getHorizontalOffset()](#getHorizontalOffset--) | يحصل أو يضبط الإزاحة الأفقية. |
| [getInternalIndentPosition()](#getInternalIndentPosition--) |  |
| [getLastModifiedTime()](#getLastModifiedTime--) | يحصل أو يضبط وقت التعديل الأخير. |
| [getMaxHeight()](#getMaxHeight--) | يحصل أو يضبط الحد الأقصى للارتفاع. |
| [getMaxWidth()](#getMaxWidth--) | يحصل أو يضبط الحد الأقصى للعرض. |
| [getMinWidth()](#getMinWidth--) | يحصل أو يضبط الحد الأدنى للعرض. |
| [getReservedWidth()](#getReservedWidth--) | يحصل أو يضبط العرض المحجوز. |
| [getVerticalOffset()](#getVerticalOffset--) | يحصل أو يضبط الإزاحة العمودية. |
| [setDescendantsCannotBeMoved(boolean value)](#setDescendantsCannotBeMoved-boolean-) | يحصل على ما إذا كان يمكن نقل سلالف المخطط. |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | يحصل أو يضبط الإزاحة الأفقية. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | يحصل أو يضبط وقت التعديل الأخير. |
| [setMaxHeight(float value)](#setMaxHeight-float-) | يحصل أو يضبط الحد الأقصى للارتفاع. |
| [setMaxWidth(float value)](#setMaxWidth-float-) | يحصل أو يضبط الحد الأقصى للعرض. |
| [setMinWidth(float value)](#setMinWidth-float-) | يحصل أو يضبط الحد الأدنى للعرض. |
| [setReservedWidth(float value)](#setReservedWidth-float-) | يحصل أو يضبط العرض المحجوز. |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | يحصل أو يضبط الإزاحة العمودية. |
### Outline() {#Outline--}
```
public Outline()
```


يُنشئ مثيلًا جديدًا من الفئة [Outline](../../com.aspose.note/outline).

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


يقبل زائر العقدة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | الكائن من فئة مشتقة من `DocumentVisitor`. |

### getDescendantsCannotBeMoved() {#getDescendantsCannotBeMoved--}
```
public boolean getDescendantsCannotBeMoved()
```


يحصل على ما إذا كان يمكن نقل سلالف المخطط.

**Returns:**
boolean
### getHorizontalOffset() {#getHorizontalOffset--}
```
public float getHorizontalOffset()
```


يحصل أو يضبط الإزاحة الأفقية.

**Returns:**
float
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
### getMaxHeight() {#getMaxHeight--}
```
public float getMaxHeight()
```


يحصل أو يضبط الحد الأقصى للارتفاع.

**Returns:**
float
### getMaxWidth() {#getMaxWidth--}
```
public float getMaxWidth()
```


يحصل أو يضبط الحد الأقصى للعرض.

**Returns:**
float
### getMinWidth() {#getMinWidth--}
```
public float getMinWidth()
```


يحصل أو يضبط الحد الأدنى للعرض.

**Returns:**
float
### getReservedWidth() {#getReservedWidth--}
```
public float getReservedWidth()
```


يحصل أو يضبط العرض المحجوز.

**Returns:**
float
### getVerticalOffset() {#getVerticalOffset--}
```
public float getVerticalOffset()
```


يحصل أو يضبط الإزاحة العمودية.

**Returns:**
float
### setDescendantsCannotBeMoved(boolean value) {#setDescendantsCannotBeMoved-boolean-}
```
public void setDescendantsCannotBeMoved(boolean value)
```


يحصل على ما إذا كان يمكن نقل سلالف المخطط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public void setHorizontalOffset(float value)
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

### setMaxHeight(float value) {#setMaxHeight-float-}
```
public void setMaxHeight(float value)
```


يحصل أو يضبط الحد الأقصى للارتفاع.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | float |  |

### setMaxWidth(float value) {#setMaxWidth-float-}
```
public void setMaxWidth(float value)
```


يحصل أو يضبط الحد الأقصى للعرض.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | float |  |

### setMinWidth(float value) {#setMinWidth-float-}
```
public void setMinWidth(float value)
```


يحصل أو يضبط الحد الأدنى للعرض.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | float |  |

### setReservedWidth(float value) {#setReservedWidth-float-}
```
public void setReservedWidth(float value)
```


يحصل أو يضبط العرض المحجوز.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | float |  |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public void setVerticalOffset(float value)
```


يحصل أو يضبط الإزاحة العمودية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | float |  |

