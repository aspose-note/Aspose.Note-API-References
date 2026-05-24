---
title: "Outline"
second_title: "Aspose.Note για Java Αναφορά API"
description: "Αντιπροσωπεύει ένα περίγραμμα."
type: docs
weight: 66
url: /el/java/com.aspose.note/outline/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode, com.aspose.note.IndentatedNode

**All Implemented Interfaces:**
[com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode)
```
public final class Outline extends IndentatedNode<IOutlineChildNode,Outline> implements IPageChildNode
```

Αντιπροσωπεύει ένα περίγραμμα.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [Outline()](#Outline--) | Δημιουργεί μια νέα παρουσία της κλάσης [Outline](../../com.aspose.note/outline) class. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Δέχεται τον επισκέπτη του κόμβου. |
| [getDescendantsCannotBeMoved()](#getDescendantsCannotBeMoved--) | Λαμβάνει εάν οι απόγονοι του περιγράμματος μπορούν να μετακινηθούν. |
| [getHorizontalOffset()](#getHorizontalOffset--) | Λαμβάνει ή ορίζει την οριζόντια μετατόπιση. |
| [getInternalIndentPosition()](#getInternalIndentPosition--) |  |
| [getLastModifiedTime()](#getLastModifiedTime--) | Λαμβάνει ή ορίζει την τελευταία τροποποιημένη ώρα. |
| [getMaxHeight()](#getMaxHeight--) | Λαμβάνει ή ορίζει το μέγιστο ύψος. |
| [getMaxWidth()](#getMaxWidth--) | Λαμβάνει ή ορίζει το μέγιστο πλάτος. |
| [getMinWidth()](#getMinWidth--) | Λαμβάνει ή ορίζει το ελάχιστο πλάτος. |
| [getReservedWidth()](#getReservedWidth--) | Λαμβάνει ή ορίζει το δεσμευμένο πλάτος. |
| [getVerticalOffset()](#getVerticalOffset--) | Λαμβάνει ή ορίζει την κάθετη μετατόπιση. |
| [setDescendantsCannotBeMoved(boolean value)](#setDescendantsCannotBeMoved-boolean-) | Λαμβάνει εάν οι απόγονοι του περιγράμματος μπορούν να μετακινηθούν. |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | Λαμβάνει ή ορίζει την οριζόντια μετατόπιση. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Λαμβάνει ή ορίζει την τελευταία τροποποιημένη ώρα. |
| [setMaxHeight(float value)](#setMaxHeight-float-) | Λαμβάνει ή ορίζει το μέγιστο ύψος. |
| [setMaxWidth(float value)](#setMaxWidth-float-) | Λαμβάνει ή ορίζει το μέγιστο πλάτος. |
| [setMinWidth(float value)](#setMinWidth-float-) | Λαμβάνει ή ορίζει το ελάχιστο πλάτος. |
| [setReservedWidth(float value)](#setReservedWidth-float-) | Λαμβάνει ή ορίζει το δεσμευμένο πλάτος. |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | Λαμβάνει ή ορίζει την κάθετη μετατόπιση. |
### Outline() {#Outline--}
```
public Outline()
```


Δημιουργεί μια νέα παρουσία της κλάσης [Outline](../../com.aspose.note/outline) class.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Δέχεται τον επισκέπτη του κόμβου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | Το αντικείμενο μιας κλάσης που προέρχεται από το `DocumentVisitor`. |

### getDescendantsCannotBeMoved() {#getDescendantsCannotBeMoved--}
```
public boolean getDescendantsCannotBeMoved()
```


Λαμβάνει εάν οι απόγονοι του περιγράμματος μπορούν να μετακινηθούν.

**Returns:**
boolean
### getHorizontalOffset() {#getHorizontalOffset--}
```
public float getHorizontalOffset()
```


Λαμβάνει ή ορίζει την οριζόντια μετατόπιση.

**Returns:**
float
### getInternalIndentPosition() {#getInternalIndentPosition--}
```
public int getInternalIndentPosition()
```


Λαμβάνει τον αριθμό των στοιχείων που θα αθροιστούν στον πίνακα RgOutlineIndentDistance για να ληφθεί το μέγεθος εσοχής.

**Returns:**
int
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Λαμβάνει ή ορίζει την τελευταία τροποποιημένη ώρα.

**Returns:**
java.util.Date
### getMaxHeight() {#getMaxHeight--}
```
public float getMaxHeight()
```


Λαμβάνει ή ορίζει το μέγιστο ύψος.

**Returns:**
float
### getMaxWidth() {#getMaxWidth--}
```
public float getMaxWidth()
```


Λαμβάνει ή ορίζει το μέγιστο πλάτος.

**Returns:**
float
### getMinWidth() {#getMinWidth--}
```
public float getMinWidth()
```


Λαμβάνει ή ορίζει το ελάχιστο πλάτος.

**Returns:**
float
### getReservedWidth() {#getReservedWidth--}
```
public float getReservedWidth()
```


Λαμβάνει ή ορίζει το δεσμευμένο πλάτος.

**Returns:**
float
### getVerticalOffset() {#getVerticalOffset--}
```
public float getVerticalOffset()
```


Λαμβάνει ή ορίζει την κάθετη μετατόπιση.

**Returns:**
float
### setDescendantsCannotBeMoved(boolean value) {#setDescendantsCannotBeMoved-boolean-}
```
public void setDescendantsCannotBeMoved(boolean value)
```


Λαμβάνει εάν οι απόγονοι του περιγράμματος μπορούν να μετακινηθούν.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean |  |

### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public void setHorizontalOffset(float value)
```


Λαμβάνει ή ορίζει την οριζόντια μετατόπιση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | float |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Λαμβάνει ή ορίζει την τελευταία τροποποιημένη ώρα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.util.Date |  |

### setMaxHeight(float value) {#setMaxHeight-float-}
```
public void setMaxHeight(float value)
```


Λαμβάνει ή ορίζει το μέγιστο ύψος.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | float |  |

### setMaxWidth(float value) {#setMaxWidth-float-}
```
public void setMaxWidth(float value)
```


Λαμβάνει ή ορίζει το μέγιστο πλάτος.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | float |  |

### setMinWidth(float value) {#setMinWidth-float-}
```
public void setMinWidth(float value)
```


Λαμβάνει ή ορίζει το ελάχιστο πλάτος.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | float |  |

### setReservedWidth(float value) {#setReservedWidth-float-}
```
public void setReservedWidth(float value)
```


Λαμβάνει ή ορίζει το δεσμευμένο πλάτος.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | float |  |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public void setVerticalOffset(float value)
```


Λαμβάνει ή ορίζει την κάθετη μετατόπιση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | float |  |

