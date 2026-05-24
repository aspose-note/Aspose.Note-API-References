---
title: "PageHistory"
second_title: "Aspose.Note για Java Αναφορά API"
description: "Αναπαριστά το ιστορικό της σελίδας."
type: docs
weight: 70
url: /el/java/com.aspose.note/pagehistory/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.ms.System.Collections.Generic.IGenericList
```
public class PageHistory implements System.Collections.Generic.IGenericList<Page>
```

Αναπαριστά το ιστορικό της σελίδας.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [PageHistory(Page page)](#PageHistory-com.aspose.note.Page-) | Αρχικοποιεί μια νέα παρουσία της κλάσης `PageHistory`. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [addItem(Page item)](#addItem-com.aspose.note.Page-) | Προσθέτει την έκδοση σελίδας στο τέλος του `PageHistory`. |
| [addRange(System.Collections.Generic.IGenericEnumerable&lt;Page&gt; items)](#addRange-com.aspose.ms.System.Collections.Generic.IGenericEnumerable-com.aspose.note.Page--) | Προσθέτει τις εκδόσεις σελίδας στο τέλος του `PageHistory`. |
| [clear()](#clear--) | Καθαρίζει το ιστορικό σελίδας. |
| [containsItem(Page item)](#containsItem-com.aspose.note.Page-) | Καθορίζει εάν το ιστορικό σελίδας περιέχει την έκδοση σελίδας. |
| [copyToTArray(Page[] array, int arrayIndex)](#copyToTArray-com.aspose.note.Page---int-) | Αντιγράφει τις εκδόσεις της σελίδας σε έναν πίνακα, ξεκινώντας από ένα συγκεκριμένο δείκτη.. |
| [getCurrent()](#getCurrent--) | Λαμβάνει την τρέχουσα έκδοση της σελίδας. |
| [get_Item(int index)](#get-Item-int-) | Λαμβάνει ή ορίζει την έκδοση της σελίδας στο καθορισμένο δείκτη του `PageHistory`. |
| [indexOfItem(Page item)](#indexOfItem-com.aspose.note.Page-) | Καθορίζει τον δείκτη μιας συγκεκριμένης έκδοσης σελίδας στο ιστορικό σελίδας. |
| [insertItem(int index, Page item)](#insertItem-int-com.aspose.note.Page-) | Εισάγει μια έκδοση σελίδας στο ιστορικό σελίδας. |
| [isReadOnly()](#isReadOnly--) | Λαμβάνει μια τιμή που υποδεικνύει αν το ιστορικό σελίδας είναι μόνο για ανάγνωση. |
| [iterator()](#iterator--) | Επιστρέφει έναν enumerator που διασχίζει τους κόμβους-παιδιά του `PageHistory`. |
| [removeAt(int index)](#removeAt-int-) | Αφαιρεί την έκδοση σελίδας στο καθορισμένο δείκτη του `PageHistory`. |
| [removeItem(Page item)](#removeItem-com.aspose.note.Page-) | Αφαιρεί την έκδοση σελίδας από το `PageHistory`. |
| [removeRange(int index, int count)](#removeRange-int-int-) | Αφαιρεί μια σειρά από εκδόσεις σελίδας από το `PageHistory`. |
| [set_Item(int index, Page value)](#set-Item-int-com.aspose.note.Page-) | Λαμβάνει ή ορίζει την έκδοση της σελίδας στο καθορισμένο δείκτη του `PageHistory`. |
| [size()](#size--) | Λαμβάνει τον αριθμό των εκδόσεων σελίδας στο ιστορικό σελίδας. |
### PageHistory(Page page) {#PageHistory-com.aspose.note.Page-}
```
public PageHistory(Page page)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης `PageHistory`.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | Η τρέχουσα έκδοση σελίδας. |

### addItem(Page item) {#addItem-com.aspose.note.Page-}
```
public void addItem(Page item)
```


Προσθέτει την έκδοση σελίδας στο τέλος του `PageHistory`.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | Η έκδοση σελίδας. |

### addRange(System.Collections.Generic.IGenericEnumerable&lt;Page&gt; items) {#addRange-com.aspose.ms.System.Collections.Generic.IGenericEnumerable-com.aspose.note.Page--}
```
public void addRange(System.Collections.Generic.IGenericEnumerable<Page> items)
```


Προσθέτει τις εκδόσεις σελίδας στο τέλος του `PageHistory`.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| αντικείμενα | com.aspose.ms.System.Collections.Generic.IGenericEnumerable&lt;com.aspose.note.Page&gt; | Η συλλογή `IEnumerable\{Page\}` των εκδόσεων σελίδας. |

### clear() {#clear--}
```
public void clear()
```


Καθαρίζει το ιστορικό σελίδας.

### containsItem(Page item) {#containsItem-com.aspose.note.Page-}
```
public boolean containsItem(Page item)
```


Καθορίζει εάν το ιστορικό σελίδας περιέχει την έκδοση σελίδας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | Η έκδοση σελίδας. |

**Returns:**
boolean - Το `bool`.
### copyToTArray(Page[] array, int arrayIndex) {#copyToTArray-com.aspose.note.Page---int-}
```
public void copyToTArray(Page[] array, int arrayIndex)
```


Αντιγράφει τις εκδόσεις της σελίδας σε έναν πίνακα, ξεκινώντας από ένα συγκεκριμένο δείκτη..

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| array | [Page\[\]](../../com.aspose.note/page) | Ο πίνακας-στόχος. |
| arrayIndex | int | Ο δείκτης του πίνακα. |

### getCurrent() {#getCurrent--}
```
public Page getCurrent()
```


Λαμβάνει την τρέχουσα έκδοση της σελίδας.

**Returns:**
[Page](../../com.aspose.note/page)
### get_Item(int index) {#get-Item-int-}
```
public Page get_Item(int index)
```


Λαμβάνει ή ορίζει την έκδοση της σελίδας στο καθορισμένο δείκτη του `PageHistory`.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| index | int | Ο δείκτης. |

**Returns:**
[Page](../../com.aspose.note/page) - The page version.
### indexOfItem(Page item) {#indexOfItem-com.aspose.note.Page-}
```
public int indexOfItem(Page item)
```


Καθορίζει τον δείκτη μιας συγκεκριμένης έκδοσης σελίδας στο ιστορικό σελίδας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | Η έκδοση σελίδας. |

**Returns:**
int - Το `int`.
### insertItem(int index, Page item) {#insertItem-int-com.aspose.note.Page-}
```
public void insertItem(int index, Page item)
```


Εισάγει μια έκδοση σελίδας στο ιστορικό σελίδας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| index | int | Ο δείκτης. |
| item | [Page](../../com.aspose.note/page) | Η έκδοση σελίδας. |

### isReadOnly() {#isReadOnly--}
```
public boolean isReadOnly()
```


Λαμβάνει μια τιμή που υποδεικνύει αν το ιστορικό σελίδας είναι μόνο για ανάγνωση.

**Returns:**
boolean
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<Page> iterator()
```


Επιστρέφει έναν enumerator που διασχίζει τους κόμβους-παιδιά του `PageHistory`.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.note.Page&gt; - Ο `IEnumerator`.
### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Αφαιρεί την έκδοση σελίδας στο καθορισμένο δείκτη του `PageHistory`.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| index | int | Ο δείκτης. |

### removeItem(Page item) {#removeItem-com.aspose.note.Page-}
```
public boolean removeItem(Page item)
```


Αφαιρεί την έκδοση σελίδας από το `PageHistory`.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| item | [Page](../../com.aspose.note/page) | Η έκδοση σελίδας. |

**Returns:**
boolean - Το `bool`.
### removeRange(int index, int count) {#removeRange-int-int-}
```
public void removeRange(int index, int count)
```


Αφαιρεί μια σειρά από εκδόσεις σελίδας από το `PageHistory`.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| index | int | Ο δείκτης. |
| count | int | Ο αριθμός. |

### set_Item(int index, Page value) {#set-Item-int-com.aspose.note.Page-}
```
public void set_Item(int index, Page value)
```


Λαμβάνει ή ορίζει την έκδοση της σελίδας στο καθορισμένο δείκτη του `PageHistory`.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| index | int | Ο δείκτης. |
| value | [Page](../../com.aspose.note/page) |  |

### size() {#size--}
```
public int size()
```


Λαμβάνει τον αριθμό των εκδόσεων σελίδας στο ιστορικό σελίδας.

**Returns:**
int
