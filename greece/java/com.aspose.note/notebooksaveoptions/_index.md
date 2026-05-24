---
title: "NotebookSaveOptions"
second_title: "Aspose.Note για Java Αναφορά API"
description: "Μια αφηρημένη βασική κλάση που αντιπροσωπεύει τις επιλογές αποθήκευσης του σημειωματάριου για μια συγκεκριμένη μορφή."
type: docs
weight: 61
url: /el/java/com.aspose.note/notebooksaveoptions/
---

**Inheritance:**
java.lang.Object
```
public abstract class NotebookSaveOptions
```

Μια αφηρημένη βασική κλάση που αντιπροσωπεύει τις επιλογές αποθήκευσης του σημειωματάριου για μια συγκεκριμένη μορφή.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getDeferredSaving()](#getDeferredSaving--) | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν τα έγγραφα παιδιών πρέπει να αποθηκευτούν ρητά. |
| [getDocumentSaveOptionsInternal()](#getDocumentSaveOptionsInternal--) | Λαμβάνει τις επιλογές αποθήκευσης για όλα τα έγγραφα παιδιών του σημειωματάριου. |
| [getFlatten()](#getFlatten--) | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν η ιεραρχία των παιδιών του σημειωματάριου αποθηκεύεται επίπεδη. |
| [getSaveFormat()](#getSaveFormat--) | Λαμβάνει τη μορφή με την οποία αποθηκεύεται το σημειωματάριο. |
| [setDeferredSaving(boolean value)](#setDeferredSaving-boolean-) | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν τα έγγραφα παιδιών πρέπει να αποθηκευτούν ρητά. |
| [setFlatten(boolean value)](#setFlatten-boolean-) | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν η ιεραρχία των παιδιών του σημειωματάριου αποθηκεύεται επίπεδη. |
### getDeferredSaving() {#getDeferredSaving--}
```
public boolean getDeferredSaving()
```


Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν τα έγγραφα παιδιών πρέπει να αποθηκευτούν ρητά.

--------------------

Η προεπιλεγμένη τιμή είναι `false`, έτσι τα θυγατρικά έγγραφα θα αποθηκευτούν έμμεσα. Η τιμή `true` υποδεικνύει ότι ο χρήστης πρέπει να αποθηκεύει ρητά κάθε θυγατρικό κόμβο του σημειωματάριου. Εάν το σημειωματάριο αποθηκεύεται σε ροή, η τιμή είναι πάντα `true` παρόλο που είχε οριστεί ρητά από τον χρήστη σε `false`.

**Returns:**
boolean
### getDocumentSaveOptionsInternal() {#getDocumentSaveOptionsInternal--}
```
public abstract SaveOptions getDocumentSaveOptionsInternal()
```


Λαμβάνει τις επιλογές αποθήκευσης για όλα τα έγγραφα παιδιών του σημειωματάριου.

**Returns:**
[SaveOptions](../../com.aspose.note/saveoptions) - The `SaveOptions`.
### getFlatten() {#getFlatten--}
```
public boolean getFlatten()
```


Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν η ιεραρχία των παιδιών του σημειωματάριου αποθηκεύεται επίπεδη.

**Returns:**
boolean
### getSaveFormat() {#getSaveFormat--}
```
public abstract int getSaveFormat()
```


Λαμβάνει τη μορφή με την οποία αποθηκεύεται το σημειωματάριο.

**Returns:**
int
### setDeferredSaving(boolean value) {#setDeferredSaving-boolean-}
```
public void setDeferredSaving(boolean value)
```


Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν τα έγγραφα παιδιών πρέπει να αποθηκευτούν ρητά.

--------------------

Η προεπιλεγμένη τιμή είναι `false`, έτσι τα θυγατρικά έγγραφα θα αποθηκευτούν έμμεσα. Η τιμή `true` υποδεικνύει ότι ο χρήστης πρέπει να αποθηκεύει ρητά κάθε θυγατρικό κόμβο του σημειωματάριου. Εάν το σημειωματάριο αποθηκεύεται σε ροή, η τιμή είναι πάντα `true` παρόλο που είχε οριστεί ρητά από τον χρήστη σε `false`.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean |  |

### setFlatten(boolean value) {#setFlatten-boolean-}
```
public void setFlatten(boolean value)
```


Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν η ιεραρχία των παιδιών του σημειωματάριου αποθηκεύεται επίπεδη.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean |  |

