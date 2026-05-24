---
title: "ITag"
second_title: "Aspose.Note για Java Αναφορά API"
description: "Η διεπαφή για ετικέτες όλων των ειδών."
type: docs
weight: 109
url: /el/java/com.aspose.note/itag/
---
```
public interface ITag
```

Η διεπαφή για ετικέτες όλων των ειδών.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getCompletedTime()](#getCompletedTime--) | Λαμβάνει την ώρα ολοκλήρωσης. |
| [getCreationTime()](#getCreationTime--) | Λαμβάνει την ώρα δημιουργίας. |
| [getIcon()](#getIcon--) | Λαμβάνει το εικονίδιο. |
| [getLabel()](#getLabel--) | Λαμβάνει το κείμενο ετικέτας. |
| [getStatus()](#getStatus--) | Λαμβάνει την κατάσταση. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Ορίζει την ώρα δημιουργίας. |
### getCompletedTime() {#getCompletedTime--}
```
public abstract Date getCompletedTime()
```


Λαμβάνει την ώρα ολοκλήρωσης.

Τιμή: Το `Nullable\{DateTime\}`.

**Returns:**
java.util.Date
### getCreationTime() {#getCreationTime--}
```
public abstract Date getCreationTime()
```


Λαμβάνει την ώρα δημιουργίας.

Τιμή: Το java.util.Date.

**Returns:**
java.util.Date
### getIcon() {#getIcon--}
```
public abstract int getIcon()
```


Λαμβάνει το εικονίδιο.

Τιμή: Το [TagIcon](../../com.aspose.note.infrastructure/tagicon).

**Returns:**
int
### getLabel() {#getLabel--}
```
public abstract String getLabel()
```


Λαμβάνει το κείμενο ετικέτας.

**Returns:**
java.lang.String
### getStatus() {#getStatus--}
```
public abstract int getStatus()
```


Λαμβάνει την κατάσταση.

Τιμή: Το [TagStatus](../../com.aspose.note/tagstatus).

**Returns:**
int
### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public abstract void setCreationTime(Date value)
```


Ορίζει την ώρα δημιουργίας.

Τιμή: Το java.util.Date.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.util.Date |  |

