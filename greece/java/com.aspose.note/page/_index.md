---
title: "Page"
second_title: "Aspose.Note για Java Αναφορά API"
description: "Αναπαριστά μια σελίδα."
type: docs
weight: 69
url: /el/java/com.aspose.note/page/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode
```
public final class Page extends CompositeNode<IPageChildNode>
```

Αναπαριστά μια σελίδα.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [Page()](#Page--) | Αρχικοποιεί μια νέα παρουσία της κλάσης `Page`. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Δέχεται τον επισκέπτη του κόμβου. |
| [deepClone()](#deepClone--) | Κλωνοποιεί τη σελίδα. |
| [deepClone(boolean cloneHistory)](#deepClone-boolean-) | Κλωνοποιεί τη σελίδα. |
| [getAuthor()](#getAuthor--) | Λαμβάνει ή ορίζει τον συγγραφέα. |
| [getBackgroundColor()](#getBackgroundColor--) | Λαμβάνει ή ορίζει το χρώμα φόντου της σελίδας. |
| [getCreationTime()](#getCreationTime--) | Λαμβάνει ή ορίζει την ώρα δημιουργίας. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Λαμβάνει ή ορίζει την τελευταία τροποποιημένη ώρα. |
| [getLevel()](#getLevel--) | Λαμβάνει ή ορίζει το επίπεδο. |
| [getMargin()](#getMargin--) | Λαμβάνει ή ορίζει το περιθώριο. |
| [getPageContentRevisionSummary()](#getPageContentRevisionSummary--) | Λαμβάνει ή ορίζει τη σύνοψη αναθεώρησης για τη σελίδα και τους υποκόμβους της. |
| [getPageLayoutSize()](#getPageLayoutSize--) | Λαμβάνει το μέγεθος διάταξης της σελίδας που εμφανίζεται στον επεξεργαστή. |
| [getSizeType()](#getSizeType--) | Λαμβάνει ή ορίζει τον τύπο μεγέθους μιας σελίδας. |
| [getTitle()](#getTitle--) | Λαμβάνει ή ορίζει τον τίτλο. |
| [isConflictPage()](#isConflictPage--) | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν αυτή η σελίδα είναι σελίδα σύγκρουσης. |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Λαμβάνει ή ορίζει τον συγγραφέα. |
| [setBackgroundColor(Color value)](#setBackgroundColor-java.awt.Color-) | Λαμβάνει ή ορίζει το χρώμα φόντου της σελίδας. |
| [setConflictPage(boolean value)](#setConflictPage-boolean-) | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν αυτή η σελίδα είναι σελίδα σύγκρουσης. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Λαμβάνει ή ορίζει την ώρα δημιουργίας. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Λαμβάνει ή ορίζει την τελευταία τροποποιημένη ώρα. |
| [setLevel(byte value)](#setLevel-byte-) | Λαμβάνει ή ορίζει το επίπεδο. |
| [setMargin(Margins value)](#setMargin-com.aspose.note.Margins-) | Λαμβάνει ή ορίζει το περιθώριο. |
| [setPageContentRevisionSummary(RevisionSummary value)](#setPageContentRevisionSummary-com.aspose.note.RevisionSummary-) | Λαμβάνει ή ορίζει τη σύνοψη αναθεώρησης για τη σελίδα και τους υποκόμβους της. |
| [setPageLayoutSize(Dimension2D value)](#setPageLayoutSize-java.awt.geom.Dimension2D-) | Ορίζει το μέγεθος διάταξης της σελίδας που εμφανίζεται στον επεξεργαστή. |
| [setSizeType(int value)](#setSizeType-int-) | Λαμβάνει ή ορίζει τον τύπο μεγέθους μιας σελίδας. |
| [setTitle(Title value)](#setTitle-com.aspose.note.Title-) | Λαμβάνει ή ορίζει τον τίτλο. |
### Page() {#Page--}
```
public Page()
```


Αρχικοποιεί μια νέα παρουσία της κλάσης `Page`.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Δέχεται τον επισκέπτη του κόμβου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | Το αντικείμενο μιας κλάσης που προέρχεται από το `DocumentVisitor`. |

### deepClone() {#deepClone--}
```
public final Page deepClone()
```


Κλωνοποιεί τη σελίδα.

**Returns:**
[Page](../../com.aspose.note/page) - A clone of the page.
### deepClone(boolean cloneHistory) {#deepClone-boolean-}
```
public final Page deepClone(boolean cloneHistory)
```


Κλωνοποιεί τη σελίδα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| cloneHistory | boolean | Καθορίζει εάν το ιστορικό της σελίδας πρέπει να κλωνοποιηθεί.. |

**Returns:**
[Page](../../com.aspose.note/page) - A clone of the page.
### getAuthor() {#getAuthor--}
```
public String getAuthor()
```


Λαμβάνει ή ορίζει τον συγγραφέα.

**Returns:**
java.lang.String
### getBackgroundColor() {#getBackgroundColor--}
```
public final Color getBackgroundColor()
```


Λαμβάνει ή ορίζει το χρώμα φόντου της σελίδας.

**Returns:**
java.awt.Color
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
### getLevel() {#getLevel--}
```
public byte getLevel()
```


Λαμβάνει ή ορίζει το επίπεδο.

**Returns:**
byte
### getMargin() {#getMargin--}
```
public Margins getMargin()
```


Λαμβάνει ή ορίζει το περιθώριο.

**Returns:**
[Margins](../../com.aspose.note/margins)
### getPageContentRevisionSummary() {#getPageContentRevisionSummary--}
```
public RevisionSummary getPageContentRevisionSummary()
```


Λαμβάνει ή ορίζει τη σύνοψη αναθεώρησης για τη σελίδα και τους υποκόμβους της.

**Returns:**
[RevisionSummary](../../com.aspose.note/revisionsummary)
### getPageLayoutSize() {#getPageLayoutSize--}
```
public final Dimension2D getPageLayoutSize()
```


Λαμβάνει το μέγεθος διάταξης της σελίδας που εμφανίζεται στον επεξεργαστή.

--------------------

Αυτή η τιμή χρησιμοποιείται από την εφαρμογή Microsoft OneNote για την εμφάνιση της υποκείμενης διάταξης της σελίδας όταν ανοίγει το έγγραφο. Δεν επηρεάζει την εκτύπωση και την αποθήκευση του εγγράφου ούτως ή άλλως. Όταν η ιδιότητα Page.SizeType ορίζεται σε PageSizeType.SizeByContent, αυτή η ιδιότητα επιστρέφει το πραγματικό μέγεθος του περιεχομένου.

**Returns:**
java.awt.geom.Dimension2D
### getSizeType() {#getSizeType--}
```
public final int getSizeType()
```


Λαμβάνει ή ορίζει τον τύπο μεγέθους μιας σελίδας.

--------------------

Από προεπιλογή, μια σελίδα αλλάζει μέγεθος αυτόματα. Η προεπιλεγμένη τιμή είναι [PageSizeType.SizeByContent](../../com.aspose.note/pagesizetype\\#SizeByContent).

**Returns:**
int
### getTitle() {#getTitle--}
```
public Title getTitle()
```


Λαμβάνει ή ορίζει τον τίτλο.

Τιμή: Ο `Title`.

**Returns:**
[Title](../../com.aspose.note/title)
### isConflictPage() {#isConflictPage--}
```
public final boolean isConflictPage()
```


Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν αυτή η σελίδα είναι σελίδα σύγκρουσης.

--------------------

Η σελίδα σύγκρουσης εμφανίζεται όταν δύο χρήστες προσπαθούν να ενημερώσουν το ίδιο περιεχόμενο. Σε αυτήν την περίπτωση οι αλλαγές του πρώτου χρήστη γράφονται όπως συνήθως. Αλλά οι αλλαγές του άλλου χρήστη δεν μπορούν να συγχωνευτούν. Έτσι δημιουργείται απλώς ένα αντίγραφο της σελίδας και σημειώνεται ως σύγκρουση.

Σε αυτήν την έκδοση, οι συγκρούσεις επιλύονται υπέρ των αλλαγών του πρώτου χρήστη. Έτσι, εάν το έγγραφο έχει σελίδες σύγκρουσης, θα εμφανίζονται στο ιστορικό αλλά θα παραλείπονται κατά την αποθήκευση. Είναι δυνατόν να επαναφέρετε αυτήν τη σημαία για να αποθηκεύσετε αυτές τις σελίδες στο ιστορικό ως συνηθισμένες.

Λεπτομερές παράδειγμα χειρισμού σελίδας σύγκρουσης μπορεί να βρεθεί στην διαδικτυακή τεκμηρίωση.

**Returns:**
boolean
### setAuthor(String value) {#setAuthor-java.lang.String-}
```
public void setAuthor(String value)
```


Λαμβάνει ή ορίζει τον συγγραφέα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String |  |

### setBackgroundColor(Color value) {#setBackgroundColor-java.awt.Color-}
```
public final void setBackgroundColor(Color value)
```


Λαμβάνει ή ορίζει το χρώμα φόντου της σελίδας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.awt.Color |  |

### setConflictPage(boolean value) {#setConflictPage-boolean-}
```
public final void setConflictPage(boolean value)
```


Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν αυτή η σελίδα είναι σελίδα σύγκρουσης.

--------------------

Η σελίδα σύγκρουσης εμφανίζεται όταν δύο χρήστες προσπαθούν να ενημερώσουν το ίδιο περιεχόμενο. Σε αυτήν την περίπτωση οι αλλαγές του πρώτου χρήστη γράφονται όπως συνήθως. Αλλά οι αλλαγές του άλλου χρήστη δεν μπορούν να συγχωνευτούν. Έτσι δημιουργείται απλώς ένα αντίγραφο της σελίδας και σημειώνεται ως σύγκρουση.

Σε αυτήν την έκδοση, οι συγκρούσεις επιλύονται υπέρ των αλλαγών του πρώτου χρήστη. Έτσι, εάν το έγγραφο έχει σελίδες σύγκρουσης, θα εμφανίζονται στο ιστορικό αλλά θα παραλείπονται κατά την αποθήκευση. Είναι δυνατόν να επαναφέρετε αυτήν τη σημαία για να αποθηκεύσετε αυτές τις σελίδες στο ιστορικό ως συνηθισμένες.

Λεπτομερές παράδειγμα χειρισμού σελίδας σύγκρουσης μπορεί να βρεθεί στην διαδικτυακή τεκμηρίωση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean |  |

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

### setLevel(byte value) {#setLevel-byte-}
```
public void setLevel(byte value)
```


Λαμβάνει ή ορίζει το επίπεδο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | byte |  |

### setMargin(Margins value) {#setMargin-com.aspose.note.Margins-}
```
public void setMargin(Margins value)
```


Λαμβάνει ή ορίζει το περιθώριο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [Margins](../../com.aspose.note/margins) |  |

### setPageContentRevisionSummary(RevisionSummary value) {#setPageContentRevisionSummary-com.aspose.note.RevisionSummary-}
```
public void setPageContentRevisionSummary(RevisionSummary value)
```


Λαμβάνει ή ορίζει τη σύνοψη αναθεώρησης για τη σελίδα και τους υποκόμβους της.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [RevisionSummary](../../com.aspose.note/revisionsummary) |  |

### setPageLayoutSize(Dimension2D value) {#setPageLayoutSize-java.awt.geom.Dimension2D-}
```
public final void setPageLayoutSize(Dimension2D value)
```


Ορίζει το μέγεθος διάταξης της σελίδας που εμφανίζεται στον επεξεργαστή.

--------------------

Αυτή η τιμή χρησιμοποιείται από την εφαρμογή Microsoft OneNote για την εμφάνιση της υποκείμενης διάταξης της σελίδας όταν ανοίγει το έγγραφο. Δεν επηρεάζει την εκτύπωση και την αποθήκευση του εγγράφου ούτως ή άλλως. Όταν η ιδιότητα Page.SizeType ορίζεται σε PageSizeType.SizeByContent, αυτή η ιδιότητα επιστρέφει το πραγματικό μέγεθος του περιεχομένου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.awt.geom.Dimension2D |  |

### setSizeType(int value) {#setSizeType-int-}
```
public final void setSizeType(int value)
```


Λαμβάνει ή ορίζει τον τύπο μεγέθους μιας σελίδας.

--------------------

Από προεπιλογή, μια σελίδα αλλάζει μέγεθος αυτόματα. Η προεπιλεγμένη τιμή είναι [PageSizeType.SizeByContent](../../com.aspose.note/pagesizetype\\#SizeByContent).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int |  |

### setTitle(Title value) {#setTitle-com.aspose.note.Title-}
```
public void setTitle(Title value)
```


Λαμβάνει ή ορίζει τον τίτλο.

Τιμή: Ο `Title`.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [Title](../../com.aspose.note/title) |  |

