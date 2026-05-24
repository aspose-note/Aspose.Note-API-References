---
title: "OutlineElement"
second_title: "Aspose.Note για Java Αναφορά API"
description: "Αναπαριστά ένα OutlineElement."
type: docs
weight: 67
url: /el/java/com.aspose.note/outlineelement/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode, com.aspose.note.IndentatedNode

**All Implemented Interfaces:**
[com.aspose.note.IOutlineChildNode](../../com.aspose.note/ioutlinechildnode), [com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode)
```
public final class OutlineElement extends IndentatedNode<IOutlineElementChildNode,OutlineElement> implements IOutlineChildNode, IOutlineElementChildNode
```

Αναπαριστά ένα OutlineElement.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [OutlineElement()](#OutlineElement--) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης `OutlineElement`. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Δέχεται τον επισκέπτη του κόμβου. |
| [getAuthorMostRecent()](#getAuthorMostRecent--) | Λαμβάνει τον πιο πρόσφατο συγγραφέα ενός στοιχείου περιγράμματος. |
| [getAuthorOriginal()](#getAuthorOriginal--) | Λαμβάνει τον αρχικό συγγραφέα ενός στοιχείου περιγράμματος. |
| [getCreationTime()](#getCreationTime--) | Λαμβάνει ή ορίζει την ώρα δημιουργίας. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Λαμβάνει ή ορίζει την τελευταία τροποποιημένη ώρα. |
| [getNumberList()](#getNumberList--) | Λαμβάνει ή ορίζει το στυλ για την κεφαλίδα αριθμημένης λίστας. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Λαμβάνει ή ορίζει την ώρα δημιουργίας. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Λαμβάνει ή ορίζει την τελευταία τροποποιημένη ώρα. |
| [setNumberList(NumberList value)](#setNumberList-com.aspose.note.NumberList-) | Λαμβάνει ή ορίζει το στυλ για την κεφαλίδα αριθμημένης λίστας. |
### OutlineElement() {#OutlineElement--}
```
public OutlineElement()
```


Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης `OutlineElement`.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Δέχεται τον επισκέπτη του κόμβου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | Το αντικείμενο μιας κλάσης που προέρχεται από το `DocumentVisitor`. |

### getAuthorMostRecent() {#getAuthorMostRecent--}
```
public final String getAuthorMostRecent()
```


Λαμβάνει τον πιο πρόσφατο συγγραφέα ενός στοιχείου περιγράμματος.

Τιμή: Ο πιο πρόσφατος συγγραφέας.

**Returns:**
java.lang.String
### getAuthorOriginal() {#getAuthorOriginal--}
```
public final String getAuthorOriginal()
```


Λαμβάνει τον αρχικό συγγραφέα ενός στοιχείου περιγράμματος.

Τιμή: Ο αρχικός συγγραφέας.

**Returns:**
java.lang.String
### getCreationTime() {#getCreationTime--}
```
public Date getCreationTime()
```


Λαμβάνει ή ορίζει την ώρα δημιουργίας.

**Returns:**
java.util.Date
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Λαμβάνει ή ορίζει την τελευταία τροποποιημένη ώρα.

**Returns:**
java.util.Date
### getNumberList() {#getNumberList--}
```
public NumberList getNumberList()
```


Λαμβάνει ή ορίζει το στυλ για την κεφαλίδα αριθμημένης λίστας.

**Returns:**
[NumberList](../../com.aspose.note/numberlist)
### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public void setCreationTime(Date value)
```


Λαμβάνει ή ορίζει την ώρα δημιουργίας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.util.Date |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Λαμβάνει ή ορίζει την τελευταία τροποποιημένη ώρα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.util.Date |  |

### setNumberList(NumberList value) {#setNumberList-com.aspose.note.NumberList-}
```
public void setNumberList(NumberList value)
```


Λαμβάνει ή ορίζει το στυλ για την κεφαλίδα αριθμημένης λίστας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [NumberList](../../com.aspose.note/numberlist) |  |

