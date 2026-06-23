---
title: "المخطط"
second_title: "مرجع Aspose.Note لـ Java API"
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
| [Outline()](#Outline--) | يقوم بإنشاء نسخة جديدة من الفئة [Outline](../../com.aspose.note/outline). |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | يقبل زائر العقدة. |
| [getDescendantsCannotBeMoved()](#getDescendantsCannotBeMoved--) | يحصل على ما إذا كان يمكن نقل سلالات المخطط. |
| [getHorizontalOffset()](#getHorizontalOffset--) | يحصل على أو يضبط الإزاحة الأفقية. |
| [getInternalIndentPosition()](#getInternalIndentPosition--) |  |
| [getLastModifiedTime()](#getLastModifiedTime--) | يحصل أو يعيّن وقت التعديل الأخير. |
| [getMaxHeight()](#getMaxHeight--) | يحصل على أو يضبط الحد الأقصى للارتفاع. |
| [getMaxWidth()](#getMaxWidth--) | يحصل على أو يضبط الحد الأقصى للعرض. |
| [getMinWidth()](#getMinWidth--) | يحصل على أو يضبط الحد الأدنى للعرض. |
| [getReservedWidth()](#getReservedWidth--) | يحصل على أو يضبط العرض المحجوز. |
| [getVerticalOffset()](#getVerticalOffset--) | يحصل على أو يضبط الإزاحة العمودية. |
| [setDescendantsCannotBeMoved(boolean value)](#setDescendantsCannotBeMoved-boolean-) | يحصل على ما إذا كان يمكن نقل سلالات المخطط. |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | يحصل على أو يضبط الإزاحة الأفقية. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | يحصل أو يعيّن وقت التعديل الأخير. |
| [setMaxHeight(float value)](#setMaxHeight-float-) | يحصل على أو يضبط الحد الأقصى للارتفاع. |
| [setMaxWidth(float value)](#setMaxWidth-float-) | يحصل على أو يضبط الحد الأقصى للعرض. |
| [setMinWidth(float value)](#setMinWidth-float-) | يحصل على أو يضبط الحد الأدنى للعرض. |
| [setReservedWidth(float value)](#setReservedWidth-float-) | يحصل على أو يضبط العرض المحجوز. |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | يحصل على أو يضبط الإزاحة العمودية. |
### Outline() {#Outline--}
```
public Outline()
```


يقوم بإنشاء نسخة جديدة من الفئة [Outline](../../com.aspose.note/outline).

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


يحصل على ما إذا كان يمكن نقل سلالات المخطط.

**Returns:**
boolean
### getHorizontalOffset() {#getHorizontalOffset--}
```
public float getHorizontalOffset()
```


يحصل على أو يضبط الإزاحة الأفقية.

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


يحصل أو يعيّن وقت التعديل الأخير.

**Returns:**
java.util.Date
### getMaxHeight() {#getMaxHeight--}
```
public float getMaxHeight()
```


يحصل على أو يضبط الحد الأقصى للارتفاع.

**Returns:**
float
### getMaxWidth() {#getMaxWidth--}
```
public float getMaxWidth()
```


يحصل على أو يضبط الحد الأقصى للعرض.

**Returns:**
float
### getMinWidth() {#getMinWidth--}
```
public float getMinWidth()
```


يحصل على أو يضبط الحد الأدنى للعرض.

**Returns:**
float
### getReservedWidth() {#getReservedWidth--}
```
public float getReservedWidth()
```


يحصل على أو يضبط العرض المحجوز.

**Returns:**
float
### getVerticalOffset() {#getVerticalOffset--}
```
public float getVerticalOffset()
```


يحصل على أو يضبط الإزاحة العمودية.

**Returns:**
float
### setDescendantsCannotBeMoved(boolean value) {#setDescendantsCannotBeMoved-boolean-}
```
public void setDescendantsCannotBeMoved(boolean value)
```


يحصل على ما إذا كان يمكن نقل سلالات المخطط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public void setHorizontalOffset(float value)
```


يحصل على أو يضبط الإزاحة الأفقية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | float |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


يحصل أو يعيّن وقت التعديل الأخير.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.Date |  |

### setMaxHeight(float value) {#setMaxHeight-float-}
```
public void setMaxHeight(float value)
```


يحصل على أو يضبط الحد الأقصى للارتفاع.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | float |  |

### setMaxWidth(float value) {#setMaxWidth-float-}
```
public void setMaxWidth(float value)
```


يحصل على أو يضبط الحد الأقصى للعرض.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | float |  |

### setMinWidth(float value) {#setMinWidth-float-}
```
public void setMinWidth(float value)
```


يحصل على أو يضبط الحد الأدنى للعرض.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | float |  |

### setReservedWidth(float value) {#setReservedWidth-float-}
```
public void setReservedWidth(float value)
```


يحصل على أو يضبط العرض المحجوز.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | float |  |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public void setVerticalOffset(float value)
```


يحصل على أو يضبط الإزاحة العمودية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | float |  |

