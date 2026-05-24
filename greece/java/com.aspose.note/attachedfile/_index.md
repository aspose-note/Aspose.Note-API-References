---
title: "AttachedFile"
second_title: "Aspose.Note για Java Αναφορά API"
description: "Αναπαριστά ένα συνημμένο αρχείο."
type: docs
weight: 11
url: /el/java/com.aspose.note/attachedfile/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node)

**All Implemented Interfaces:**
[com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode), [com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode), [com.aspose.note.ITaggable](../../com.aspose.note/itaggable)
```
public class AttachedFile extends Node implements IPageChildNode, IOutlineElementChildNode, ITaggable
```

Αναπαριστά ένα συνημμένο αρχείο.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [AttachedFile(String path)](#AttachedFile-java.lang.String-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης `AttachedFile`. |
| [AttachedFile(String path, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)](#AttachedFile-java.lang.String-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης `AttachedFile`. |
| [AttachedFile(String fileName, InputStream attachedFileStream)](#AttachedFile-java.lang.String-java.io.InputStream-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης `AttachedFile`. |
| [AttachedFile(String fileName, InputStream attachedFileStream, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)](#AttachedFile-java.lang.String-java.io.InputStream-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης `AttachedFile`. |
| [AttachedFile()](#AttachedFile--) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης `AttachedFile`. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Δέχεται τον επισκέπτη του κόμβου. |
| [getAlignment()](#getAlignment--) | Λαμβάνει την ευθυγράμμιση. |
| [getAlternativeTextDescription()](#getAlternativeTextDescription--) | Λαμβάνει ή ορίζει ένα εναλλακτικό κείμενο σώματος για το εικονίδιο του συνημμένου αρχείου. |
| [getAlternativeTextTitle()](#getAlternativeTextTitle--) | Λαμβάνει ή ορίζει έναν τίτλο εναλλακτικού κειμένου για το εικονίδιο του συνημμένου αρχείου. |
| [getBytes()](#getBytes--) | Λαμβάνει τα δυαδικά δεδομένα για ένα ενσωματωμένο αρχείο. |
| [getExtension()](#getExtension--) | Λαμβάνει την επέκταση ενός ενσωματωμένου αρχείου. |
| [getFileName()](#getFileName--) | Λαμβάνει το όνομα του ενσωματωμένου αρχείου. |
| [getFilePath()](#getFilePath--) | Λαμβάνει τη διαδρομή προς το αρχικό αρχείο. |
| [getHeight()](#getHeight--) | Λαμβάνει το αρχικό ύψος του εικονιδίου του ενσωματωμένου αρχείου. |
| [getHorizontalOffset()](#getHorizontalOffset--) | Λαμβάνει την οριζόντια μετατόπιση. |
| [getIcon()](#getIcon--) | Λαμβάνει τα δυαδικά δεδομένα για το εικονίδιο που σχετίζεται με το ενσωματωμένο αρχείο. |
| [getIconExtension()](#getIconExtension--) | Λαμβάνει την επέκταση του εικονιδίου. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Λαμβάνει την ώρα τελευταίας τροποποίησης. |
| [getMaxHeight()](#getMaxHeight--) | Λαμβάνει το μέγιστο ύψος για την εμφάνιση του ενσωματωμένου εικονιδίου αρχείου. |
| [getMaxWidth()](#getMaxWidth--) | Λαμβάνει το μέγιστο πλάτος για την εμφάνιση του ενσωματωμένου εικονιδίου αρχείου. |
| [getParsingErrorInfo()](#getParsingErrorInfo--) | Λαμβάνει τα δεδομένα σχετικά με το σφάλμα που προέκυψε κατά την πρόσβαση στο αρχείο. |
| [getTags()](#getTags--) | Λαμβάνει τη λίστα των ετικετών ενός συνημμένου αρχείου. |
| [getText()](#getText--) | Λαμβάνει την κειμενική αναπαράσταση του ενσωματωμένου αρχείου. |
| [getVerticalOffset()](#getVerticalOffset--) | Λαμβάνει την κατακόρυφη μετατόπιση. |
| [getWidth()](#getWidth--) | Λαμβάνει το αρχικό πλάτος του ενσωματωμένου εικονιδίου αρχείου. |
| [isPrintout()](#isPrintout--) | Λαμβάνει μια τιμή που υποδεικνύει εάν η προβολή του αρχείου είναι εκτύπωση. |
| [isSizeSetByUser()](#isSizeSetByUser--) | Λαμβάνει μια τιμή που υποδεικνύει εάν η τιμή του μεγέθους του εικονιδίου ενημερώθηκε ρητά από τον χρήστη. |
| [setAlignment(int value)](#setAlignment-int-) | Ορίζει την ευθυγράμμιση. |
| [setAlternativeTextDescription(String value)](#setAlternativeTextDescription-java.lang.String-) | Λαμβάνει ή ορίζει ένα εναλλακτικό κείμενο σώματος για το εικονίδιο του συνημμένου αρχείου. |
| [setAlternativeTextTitle(String value)](#setAlternativeTextTitle-java.lang.String-) | Λαμβάνει ή ορίζει έναν τίτλο εναλλακτικού κειμένου για το εικονίδιο του συνημμένου αρχείου. |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | Ορίζει την οριζόντια μετατόπιση. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Ορίζει την ώρα τελευταίας τροποποίησης. |
| [setMaxHeight(float value)](#setMaxHeight-float-) | Ορίζει το μέγιστο ύψος για την εμφάνιση του ενσωματωμένου εικονιδίου αρχείου. |
| [setMaxWidth(float value)](#setMaxWidth-float-) | Ορίζει το μέγιστο πλάτος για την εμφάνιση του ενσωματωμένου εικονιδίου αρχείου. |
| [setPrintout(boolean value)](#setPrintout-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν η προβολή του αρχείου είναι εκτύπωση. |
| [setSizeSetByUser(boolean value)](#setSizeSetByUser-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν η τιμή του μεγέθους του εικονιδίου ενημερώθηκε ρητά από τον χρήστη. |
| [setText(String value)](#setText-java.lang.String-) | Ορίζει την κειμενική αναπαράσταση του ενσωματωμένου αρχείου. |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | Ορίζει την κατακόρυφη μετατόπιση. |
### AttachedFile(String path) {#AttachedFile-java.lang.String-}
```
public AttachedFile(String path)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης `AttachedFile`.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| διαδρομή | java.lang.String | Μια συμβολοσειρά που περιέχει τη διαδρομή προς το αρχείο από το οποίο θα δημιουργηθεί το `AttachedFile`. |

### AttachedFile(String path, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat) {#AttachedFile-java.lang.String-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-}
```
public AttachedFile(String path, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης `AttachedFile`.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| διαδρομή | java.lang.String | Μια συμβολοσειρά που περιέχει τη διαδρομή προς το αρχείο από το οποίο θα δημιουργηθεί το `AttachedFile`. |
| εικονίδιο | java.io.InputStream | Ένα εικονίδιο για το συνημμένο αρχείο. |
| iconFormat | com.aspose.ms.System.Drawing.Imaging.ImageFormat |  |

### AttachedFile(String fileName, InputStream attachedFileStream) {#AttachedFile-java.lang.String-java.io.InputStream-}
```
public AttachedFile(String fileName, InputStream attachedFileStream)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης `AttachedFile`.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fileName | java.lang.String | Ένα όνομα του συνημμένου αρχείου. |
| attachedFileStream | java.io.InputStream | Μία ροή που περιέχει τα byte του συνημμένου αρχείου. |

### AttachedFile(String fileName, InputStream attachedFileStream, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat) {#AttachedFile-java.lang.String-java.io.InputStream-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-}
```
public AttachedFile(String fileName, InputStream attachedFileStream, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης `AttachedFile`.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fileName | java.lang.String | Ένα όνομα του συνημμένου αρχείου. |
| attachedFileStream | java.io.InputStream | Μία ροή που περιέχει τα byte του συνημμένου αρχείου. |
| εικονίδιο | java.io.InputStream | Ένα εικονίδιο για το συνημμένο αρχείο. |
| iconFormat | com.aspose.ms.System.Drawing.Imaging.ImageFormat | Μια μορφή του εικονιδίου του συνημμένου αρχείου. |

### AttachedFile() {#AttachedFile--}
```
public AttachedFile()
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης `AttachedFile`.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Δέχεται τον επισκέπτη του κόμβου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | Το αντικείμενο μιας κλάσης που προέρχεται από το `DocumentVisitor`. |

### getAlignment() {#getAlignment--}
```
public int getAlignment()
```


Λαμβάνει την ευθυγράμμιση.

**Returns:**
int
### getAlternativeTextDescription() {#getAlternativeTextDescription--}
```
public final String getAlternativeTextDescription()
```


Λαμβάνει ή ορίζει ένα εναλλακτικό κείμενο σώματος για το εικονίδιο του συνημμένου αρχείου.

**Returns:**
java.lang.String
### getAlternativeTextTitle() {#getAlternativeTextTitle--}
```
public final String getAlternativeTextTitle()
```


Λαμβάνει ή ορίζει έναν τίτλο εναλλακτικού κειμένου για το εικονίδιο του συνημμένου αρχείου.

**Returns:**
java.lang.String
### getBytes() {#getBytes--}
```
public byte[] getBytes()
```


Λαμβάνει τα δυαδικά δεδομένα για ένα ενσωματωμένο αρχείο.

**Returns:**
byte[]
### getExtension() {#getExtension--}
```
public String getExtension()
```


Λαμβάνει την επέκταση ενός ενσωματωμένου αρχείου.

**Returns:**
java.lang.String
### getFileName() {#getFileName--}
```
public String getFileName()
```


Λαμβάνει το όνομα του ενσωματωμένου αρχείου.

**Returns:**
java.lang.String
### getFilePath() {#getFilePath--}
```
public String getFilePath()
```


Λαμβάνει τη διαδρομή προς το αρχικό αρχείο.

**Returns:**
java.lang.String
### getHeight() {#getHeight--}
```
public float getHeight()
```


Λαμβάνει το αρχικό ύψος του εικονιδίου του ενσωματωμένου αρχείου.

**Returns:**
float
### getHorizontalOffset() {#getHorizontalOffset--}
```
public float getHorizontalOffset()
```


Λαμβάνει την οριζόντια μετατόπιση.

**Returns:**
float
### getIcon() {#getIcon--}
```
public byte[] getIcon()
```


Λαμβάνει τα δυαδικά δεδομένα για το εικονίδιο που σχετίζεται με το ενσωματωμένο αρχείο.

**Returns:**
byte[]
### getIconExtension() {#getIconExtension--}
```
public String getIconExtension()
```


Λαμβάνει την επέκταση του εικονιδίου.

**Returns:**
java.lang.String
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Λαμβάνει την ώρα τελευταίας τροποποίησης.

**Returns:**
java.util.Date
### getMaxHeight() {#getMaxHeight--}
```
public float getMaxHeight()
```


Λαμβάνει το μέγιστο ύψος για την εμφάνιση του ενσωματωμένου εικονιδίου αρχείου.

**Returns:**
float
### getMaxWidth() {#getMaxWidth--}
```
public float getMaxWidth()
```


Λαμβάνει το μέγιστο πλάτος για την εμφάνιση του ενσωματωμένου εικονιδίου αρχείου.

**Returns:**
float
### getParsingErrorInfo() {#getParsingErrorInfo--}
```
public final ParsingErrorInfo getParsingErrorInfo()
```


Λαμβάνει τα δεδομένα σχετικά με το σφάλμα που προέκυψε κατά την πρόσβαση στο αρχείο.

**Returns:**
[ParsingErrorInfo](../../com.aspose.note.infrastructure/parsingerrorinfo)
### getTags() {#getTags--}
```
public final System.Collections.Generic.List<ITag> getTags()
```


Λαμβάνει τη λίστα των ετικετών ενός συνημμένου αρχείου.

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.note.ITag&gt;
### getText() {#getText--}
```
public String getText()
```


Λαμβάνει την αναπαράσταση κειμένου του ενσωματωμένου αρχείου. Η συμβολοσειρά ΔΕΝ ΠΡΕΠΕΙ να περιέχει κανέναν χαρακτήρα της τιμής 10 (αλλαγή γραμμής) ή 13 (επιστροφή γραμμής).

**Returns:**
java.lang.String
### getVerticalOffset() {#getVerticalOffset--}
```
public float getVerticalOffset()
```


Λαμβάνει την κατακόρυφη μετατόπιση.

**Returns:**
float
### getWidth() {#getWidth--}
```
public float getWidth()
```


Λαμβάνει το αρχικό πλάτος του ενσωματωμένου εικονιδίου αρχείου.

**Returns:**
float
### isPrintout() {#isPrintout--}
```
public boolean isPrintout()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν η προβολή του αρχείου είναι εκτύπωση.

**Returns:**
boolean
### isSizeSetByUser() {#isSizeSetByUser--}
```
public boolean isSizeSetByUser()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν η τιμή του μεγέθους του εικονιδίου ενημερώθηκε ρητά από τον χρήστη.

**Returns:**
boolean
### setAlignment(int value) {#setAlignment-int-}
```
public void setAlignment(int value)
```


Ορίζει την ευθυγράμμιση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | Τιμή του Alignment. |

### setAlternativeTextDescription(String value) {#setAlternativeTextDescription-java.lang.String-}
```
public final void setAlternativeTextDescription(String value)
```


Λαμβάνει ή ορίζει ένα εναλλακτικό κείμενο σώματος για το εικονίδιο του συνημμένου αρχείου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String |  |

### setAlternativeTextTitle(String value) {#setAlternativeTextTitle-java.lang.String-}
```
public final void setAlternativeTextTitle(String value)
```


Λαμβάνει ή ορίζει έναν τίτλο εναλλακτικού κειμένου για το εικονίδιο του συνημμένου αρχείου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String |  |

### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public void setHorizontalOffset(float value)
```


Ορίζει την οριζόντια μετατόπιση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | float | Τιμή του Offsets. |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Ορίζει την ώρα τελευταίας τροποποίησης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.util.Date | Τιμή του Date. |

### setMaxHeight(float value) {#setMaxHeight-float-}
```
public void setMaxHeight(float value)
```


Ορίζει το μέγιστο ύψος για την εμφάνιση του ενσωματωμένου εικονιδίου αρχείου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | float | Τιμή του Maximum height. |

### setMaxWidth(float value) {#setMaxWidth-float-}
```
public void setMaxWidth(float value)
```


Ορίζει το μέγιστο πλάτος για την εμφάνιση του ενσωματωμένου εικονιδίου αρχείου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | float | Τιμή του Maximum width. |

### setPrintout(boolean value) {#setPrintout-boolean-}
```
public void setPrintout(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν η προβολή του αρχείου είναι εκτύπωση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | Νέα τιμή. |

### setSizeSetByUser(boolean value) {#setSizeSetByUser-boolean-}
```
public void setSizeSetByUser(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν η τιμή του μεγέθους του εικονιδίου ενημερώθηκε ρητά από τον χρήστη.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | Νέα τιμή. |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Ορίζει την αναπαράσταση κειμένου του ενσωματωμένου αρχείου. Η συμβολοσειρά ΔΕΝ ΠΡΕΠΕΙ να περιέχει κανέναν χαρακτήρα της τιμής 10 (αλλαγή γραμμής) ή 13 (επιστροφή γραμμής).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | Τιμή του Text. |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public void setVerticalOffset(float value)
```


Ορίζει την κατακόρυφη μετατόπιση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | float | Τιμή του Offset. |

