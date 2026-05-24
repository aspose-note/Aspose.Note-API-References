---
title: "CheckBox"
second_title: "Aspose.Note για Java Αναφορά API"
description: "Η βασική κλάση για ετικέτες που μπορούν να εναλλάσσουν την κατάσταση τους μεταξύ ολοκληρωμένης και μη ολοκληρωμένης."
type: docs
weight: 13
url: /el/java/com.aspose.note/checkbox/
---

**Inheritance:**
java.lang.Object, com.aspose.note.TagExtended
```
public abstract class CheckBox extends TagExtended
```

Η βασική κλάση για ετικέτες που μπορούν να εναλλάσσουν την κατάσταση τους μεταξύ ολοκληρωμένης και μη ολοκληρωμένης.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getChecked()](#getChecked--) | Λαμβάνει μια τιμή που υποδεικνύει εάν το CheckBox βρίσκεται σε κατάσταση ολοκληρωμένης. |
| [getCompletedTime()](#getCompletedTime--) | Λαμβάνει ή ορίζει την ώρα ολοκλήρωσης. |
| [getCreationTime()](#getCreationTime--) | Λαμβάνει ή ορίζει την ώρα δημιουργίας. |
| [getIcon()](#getIcon--) | Λαμβάνει ή ορίζει το εικονίδιο. |
| [getStatus()](#getStatus--) | Λαμβάνει ή ορίζει την κατάσταση. |
| [setCompleted()](#setCompleted--) | Ορίζει την ετικέτα στην κατάσταση ολοκληρωμένη χρησιμοποιώντας την τρέχουσα ώρα ως ώρα ολοκλήρωσης. |
| [setCompleted(Date completedTime)](#setCompleted-java.util.Date-) | Ορίζει την ετικέτα στην κατάσταση ολοκληρωμένη. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Λαμβάνει ή ορίζει την ώρα δημιουργίας. |
| [setOpen()](#setOpen--) | Ορίζει την ετικέτα σε κατάσταση ανοιχτής. |
### getChecked() {#getChecked--}
```
public final boolean getChecked()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν το CheckBox βρίσκεται σε κατάσταση ολοκληρωμένης.

**Returns:**
boolean
### getCompletedTime() {#getCompletedTime--}
```
public final Date getCompletedTime()
```


Λαμβάνει ή ορίζει την ώρα ολοκλήρωσης.

Τιμή: Το `Nullable\{DateTime\}`.

**Returns:**
java.util.Date
### getCreationTime() {#getCreationTime--}
```
public final Date getCreationTime()
```


Λαμβάνει ή ορίζει την ώρα δημιουργίας.

Τιμή: Το java.util.Date.

**Returns:**
java.util.Date
### getIcon() {#getIcon--}
```
public abstract int getIcon()
```


Λαμβάνει ή ορίζει το εικονίδιο.

Τιμή: Το [TagIcon](../../com.aspose.note.infrastructure/tagicon).

**Returns:**
int
### getStatus() {#getStatus--}
```
public final int getStatus()
```


Λαμβάνει ή ορίζει την κατάσταση.

Τιμή: Το [TagStatus](../../com.aspose.note/tagstatus).

**Returns:**
int
### setCompleted() {#setCompleted--}
```
public final void setCompleted()
```


Ορίζει την ετικέτα στην κατάσταση ολοκληρωμένη χρησιμοποιώντας την τρέχουσα ώρα ως ώρα ολοκλήρωσης.

### setCompleted(Date completedTime) {#setCompleted-java.util.Date-}
```
public final void setCompleted(Date completedTime)
```


Ορίζει την ετικέτα στην κατάσταση ολοκληρωμένη.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| completedTime | java.util.Date | Η ώρα ολοκλήρωσης. |

### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public final void setCreationTime(Date value)
```


Λαμβάνει ή ορίζει την ώρα δημιουργίας.

Τιμή: Το java.util.Date.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.util.Date |  |

### setOpen() {#setOpen--}
```
public void setOpen()
```


Ορίζει την ετικέτα σε κατάσταση ανοιχτής.

