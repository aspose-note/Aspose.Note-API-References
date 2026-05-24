---
title: "Table"
second_title: "Aspose.Note για Java Αναφορά API"
description: "Αναπαριστά έναν πίνακα."
type: docs
weight: 87
url: /el/java/com.aspose.note/table/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode

**All Implemented Interfaces:**
[com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode), [com.aspose.note.ITaggable](../../com.aspose.note/itaggable)
```
public final class Table extends CompositeNode<TableRow> implements IOutlineElementChildNode, ITaggable
```

Αναπαριστά έναν πίνακα.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [Table()](#Table--) | Αρχικοποιεί μια νέα παρουσία της κλάσης `Table`. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Δέχεται τον επισκέπτη του κόμβου. |
| [getColumns()](#getColumns--) | Λαμβάνει τις στήλες του πίνακα. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Λαμβάνει ή ορίζει την τελευταία τροποποιημένη ώρα. |
| [getTags()](#getTags--) | Λαμβάνει τη λίστα όλων των ετικετών ενός πίνακα. |
| [isBordersVisible()](#isBordersVisible--) | Λαμβάνει μια τιμή που υποδεικνύει εάν το περίγραμμα του πίνακα είναι ορατό. |
| [setBordersVisible(boolean value)](#setBordersVisible-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν το περίγραμμα του πίνακα είναι ορατό. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Λαμβάνει ή ορίζει την τελευταία τροποποιημένη ώρα. |
### Table() {#Table--}
```
public Table()
```


Αρχικοποιεί μια νέα παρουσία της κλάσης `Table`.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Δέχεται τον επισκέπτη του κόμβου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | Το αντικείμενο μιας κλάσης που προέρχεται από το `DocumentVisitor`. |

### getColumns() {#getColumns--}
```
public System.Collections.Generic.IGenericList<TableColumn> getColumns()
```


Λαμβάνει τις στήλες του πίνακα.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericList&lt;com.aspose.note.TableColumn&gt;
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Λαμβάνει ή ορίζει την τελευταία τροποποιημένη ώρα.

**Returns:**
java.util.Date
### getTags() {#getTags--}
```
public final System.Collections.Generic.List<ITag> getTags()
```


Λαμβάνει τη λίστα όλων των ετικετών ενός πίνακα.

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.note.ITag&gt;
### isBordersVisible() {#isBordersVisible--}
```
public boolean isBordersVisible()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν το περίγραμμα του πίνακα είναι ορατό.

**Returns:**
boolean
### setBordersVisible(boolean value) {#setBordersVisible-boolean-}
```
public void setBordersVisible(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν το περίγραμμα του πίνακα είναι ορατό.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Λαμβάνει ή ορίζει την τελευταία τροποποιημένη ώρα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.util.Date |  |

