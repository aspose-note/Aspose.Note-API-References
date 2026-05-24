---
title: "Εικόνα"
second_title: "Aspose.Note για Java Αναφορά API"
description: "Αναπαριστά μια Εικόνα."
type: docs
weight: 33
url: /el/java/com.aspose.note/image/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode

**All Implemented Interfaces:**
[com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode), [com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode), [com.aspose.note.ITaggable](../../com.aspose.note/itaggable)
```
public final class Image extends CompositeNode<Loop> implements IPageChildNode, IOutlineElementChildNode, ITaggable
```

Αναπαριστά μια Εικόνα.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [Image(String path)](#Image-java.lang.String-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης `Image`. |
| [Image(String fileName, InputStream imageStream)](#Image-java.lang.String-java.io.InputStream-) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης `Image`. |
| [Image()](#Image--) | Αρχικοποιεί ένα νέο αντικείμενο της κλάσης `Image`. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Δέχεται τον επισκέπτη του κόμβου. |
| [getAlignment()](#getAlignment--) | Λαμβάνει την ευθυγράμμιση. |
| [getAlternativeTextDescription()](#getAlternativeTextDescription--) | Λαμβάνει ένα κείμενο σώματος ως εναλλακτικό κείμενο για την εικόνα. |
| [getAlternativeTextTitle()](#getAlternativeTextTitle--) | Λαμβάνει έναν τίτλο εναλλακτικού κειμένου για την εικόνα. |
| [getBytes()](#getBytes--) | Λαμβάνει την αποθήκη δεδομένων της εικόνας. |
| [getFileName()](#getFileName--) | Λαμβάνει το όνομα του αρχείου. |
| [getFilePath()](#getFilePath--) | Λαμβάνει τη διαδρομή του αρχείου εικόνας. |
| [getFormat()](#getFormat--) | Λαμβάνει τη μορφή της εικόνας. |
| [getHeight()](#getHeight--) | Λαμβάνει το ύψος. |
| [getHorizontalOffset()](#getHorizontalOffset--) | Λαμβάνει την οριζόντια μετατόπιση. |
| [getHyperlinkUrl()](#getHyperlinkUrl--) | Λαμβάνει τον υπερσύνδεσμο που σχετίζεται με την εικόνα. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Λαμβάνει την ώρα τελευταίας τροποποίησης. |
| [getOriginalHeight()](#getOriginalHeight--) | Λαμβάνει το αρχικό ύψος. |
| [getOriginalWidth()](#getOriginalWidth--) | Λαμβάνει το αρχικό πλάτος. |
| [getTags()](#getTags--) | Λαμβάνει τη λίστα όλων των ετικετών μιας εικόνας. |
| [getVerticalOffset()](#getVerticalOffset--) | Λαμβάνει την κατακόρυφη μετατόπιση. |
| [getWidth()](#getWidth--) | Λαμβάνει το πλάτος. |
| [isBackground()](#isBackground--) | Λαμβάνει εάν η εικόνα είναι εικόνα φόντου. |
| [replace(Image newImage)](#replace-com.aspose.note.Image-) | Αντικαθιστά τα τρέχοντα δεδομένα εικόνας με τα δεδομένα από το παρεχόμενο αντικείμενο Image. |
| [setAlignment(int value)](#setAlignment-int-) | Ορίζει την ευθυγράμμιση. |
| [setAlternativeTextDescription(String value)](#setAlternativeTextDescription-java.lang.String-) | Ορίζει ένα κείμενο σώματος ως εναλλακτικό κείμενο για την εικόνα. |
| [setAlternativeTextTitle(String value)](#setAlternativeTextTitle-java.lang.String-) | Ορίζει έναν τίτλο εναλλακτικού κειμένου για την εικόνα. |
| [setBackground(boolean value)](#setBackground-boolean-) | Λαμβάνει εάν η εικόνα είναι εικόνα φόντου. |
| [setHeight(float value)](#setHeight-float-) | Ορίζει το ύψος. |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | Ορίζει την οριζόντια μετατόπιση. |
| [setHyperlinkUrl(String value)](#setHyperlinkUrl-java.lang.String-) | Ορίζει τον υπερσύνδεσμο που σχετίζεται με την εικόνα. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Ορίζει την ώρα τελευταίας τροποποίησης. |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | Ορίζει την κατακόρυφη μετατόπιση. |
| [setWidth(float value)](#setWidth-float-) | Ορίζει το πλάτος. |
### Image(String path) {#Image-java.lang.String-}
```
public Image(String path)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης `Image`.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| διαδρομή | java.lang.String | Μια συμβολοσειρά που περιέχει τη διαδρομή προς το αρχείο από το οποίο θα δημιουργηθεί το `Image`. |

### Image(String fileName, InputStream imageStream) {#Image-java.lang.String-java.io.InputStream-}
```
public Image(String fileName, InputStream imageStream)
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης `Image`.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fileName | java.lang.String | Ένα όνομα της εικόνας. |
| imageStream | java.io.InputStream | Μια ροή που περιέχει την εικόνα. |

### Image() {#Image--}
```
public Image()
```


Αρχικοποιεί ένα νέο αντικείμενο της κλάσης `Image`.

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


Λαμβάνει ένα κείμενο σώματος ως εναλλακτικό κείμενο για την εικόνα.

**Returns:**
java.lang.String
### getAlternativeTextTitle() {#getAlternativeTextTitle--}
```
public final String getAlternativeTextTitle()
```


Λαμβάνει έναν τίτλο εναλλακτικού κειμένου για την εικόνα.

**Returns:**
java.lang.String
### getBytes() {#getBytes--}
```
public byte[] getBytes()
```


Λαμβάνει την αποθήκη δεδομένων της εικόνας.

**Returns:**
byte[]
### getFileName() {#getFileName--}
```
public String getFileName()
```


Λαμβάνει το όνομα του αρχείου.

**Returns:**
java.lang.String
### getFilePath() {#getFilePath--}
```
public String getFilePath()
```


Λαμβάνει τη διαδρομή του αρχείου εικόνας.

**Returns:**
java.lang.String
### getFormat() {#getFormat--}
```
public final System.Drawing.Imaging.ImageFormat getFormat()
```


Λαμβάνει τη μορφή της εικόνας.

**Returns:**
com.aspose.ms.System.Drawing.Imaging.ImageFormat
### getHeight() {#getHeight--}
```
public final float getHeight()
```


Λαμβάνει το ύψος. Αυτό είναι το πραγματικό ύψος της εικόνας στο έγγραφο MS OneNote.

**Returns:**
float
### getHorizontalOffset() {#getHorizontalOffset--}
```
public float getHorizontalOffset()
```


Λαμβάνει την οριζόντια μετατόπιση.

**Returns:**
float
### getHyperlinkUrl() {#getHyperlinkUrl--}
```
public String getHyperlinkUrl()
```


Λαμβάνει τον υπερσύνδεσμο που σχετίζεται με την εικόνα.

**Returns:**
java.lang.String
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Λαμβάνει την ώρα τελευταίας τροποποίησης.

**Returns:**
java.util.Date
### getOriginalHeight() {#getOriginalHeight--}
```
public float getOriginalHeight()
```


Λαμβάνει το αρχικό ύψος. Αυτό είναι το αρχικό πλάτος της εικόνας, πριν από την αλλαγή μεγέθους.

**Returns:**
float
### getOriginalWidth() {#getOriginalWidth--}
```
public float getOriginalWidth()
```


Λαμβάνει το αρχικό πλάτος. Αυτό είναι το αρχικό πλάτος της εικόνας, πριν από την αλλαγή μεγέθους.

**Returns:**
float
### getTags() {#getTags--}
```
public final System.Collections.Generic.List<ITag> getTags()
```


Λαμβάνει τη λίστα όλων των ετικετών μιας εικόνας.

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.note.ITag&gt;
### getVerticalOffset() {#getVerticalOffset--}
```
public float getVerticalOffset()
```


Λαμβάνει την κατακόρυφη μετατόπιση.

**Returns:**
float
### getWidth() {#getWidth--}
```
public final float getWidth()
```


Λαμβάνει το πλάτος. Αυτό είναι το πραγματικό πλάτος της εικόνας στο έγγραφο MS OneNote.

**Returns:**
float
### isBackground() {#isBackground--}
```
public final boolean isBackground()
```


Λαμβάνει εάν η εικόνα είναι εικόνα φόντου.

**Returns:**
boolean
### replace(Image newImage) {#replace-com.aspose.note.Image-}
```
public void replace(Image newImage)
```


Αντικαθιστά τα τρέχοντα δεδομένα εικόνας με τα δεδομένα από το παρεχόμενο αντικείμενο Image.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| newImage | [Image](../../com.aspose.note/image) |  |

### setAlignment(int value) {#setAlignment-int-}
```
public void setAlignment(int value)
```


Ορίζει την ευθυγράμμιση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int |  |

### setAlternativeTextDescription(String value) {#setAlternativeTextDescription-java.lang.String-}
```
public final void setAlternativeTextDescription(String value)
```


Ορίζει ένα κείμενο σώματος ως εναλλακτικό κείμενο για την εικόνα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String |  |

### setAlternativeTextTitle(String value) {#setAlternativeTextTitle-java.lang.String-}
```
public final void setAlternativeTextTitle(String value)
```


Ορίζει έναν τίτλο εναλλακτικού κειμένου για την εικόνα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String |  |

### setBackground(boolean value) {#setBackground-boolean-}
```
public final void setBackground(boolean value)
```


Λαμβάνει εάν η εικόνα είναι εικόνα φόντου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean |  |

### setHeight(float value) {#setHeight-float-}
```
public final void setHeight(float value)
```


Ορίζει το ύψος. Αυτό είναι το πραγματικό ύψος της εικόνας στο έγγραφο MS OneNote.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | float |  |

### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public void setHorizontalOffset(float value)
```


Ορίζει την οριζόντια μετατόπιση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | float |  |

### setHyperlinkUrl(String value) {#setHyperlinkUrl-java.lang.String-}
```
public void setHyperlinkUrl(String value)
```


Ορίζει τον υπερσύνδεσμο που σχετίζεται με την εικόνα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Ορίζει την ώρα τελευταίας τροποποίησης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.util.Date |  |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public void setVerticalOffset(float value)
```


Ορίζει την κατακόρυφη μετατόπιση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | float |  |

### setWidth(float value) {#setWidth-float-}
```
public final void setWidth(float value)
```


Ορίζει το πλάτος. Αυτό είναι το πραγματικό πλάτος της εικόνας στο έγγραφο MS OneNote.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | float |  |

