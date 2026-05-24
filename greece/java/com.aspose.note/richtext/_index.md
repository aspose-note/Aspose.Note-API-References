---
title: "RichText"
second_title: "Aspose.Note για Java Αναφορά API"
description: "Αναπαριστά πλούσιο κείμενο."
type: docs
weight: 82
url: /el/java/com.aspose.note/richtext/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node)

**All Implemented Interfaces:**
[com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode), [com.aspose.note.ITaggable](../../com.aspose.note/itaggable), com.aspose.ms.System.Collections.Generic.IGenericEnumerable
```
public class RichText extends Node implements IOutlineElementChildNode, ITaggable, System.Collections.Generic.IGenericEnumerable<Character>
```

Αναπαριστά πλούσιο κείμενο.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [RichText()](#RichText--) | Αρχικοποιεί μια νέα παρουσία της κλάσης [RichText](../../com.aspose.note/richtext). |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Δέχεται τον επισκέπτη του κόμβου. |
| [append(String value)](#append-java.lang.String-) | Προσθέτει μια συμβολοσειρά στην τελευταία περιοχή κειμένου. |
| [append(String value, TextStyle style)](#append-java.lang.String-com.aspose.note.TextStyle-) | Προσθέτει μια συμβολοσειρά στο τέλος. |
| [appendFront(String value)](#appendFront-java.lang.String-) | Προσθέτει μια συμβολοσειρά στην αρχή της πρώτης περιοχής κειμένου. |
| [appendFront(String value, TextStyle style)](#appendFront-java.lang.String-com.aspose.note.TextStyle-) | Προσθέτει μια συμβολοσειρά στην αρχή. |
| [clear()](#clear--) | Καθαρίζει το περιεχόμενο αυτού του αντικειμένου. |
| [getAlignment()](#getAlignment--) | Λαμβάνει την ευθυγράμμιση. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Λαμβάνει την ώρα τελευταίας τροποποίησης. |
| [getLength()](#getLength--) |  |
| [getLineSpacing()](#getLineSpacing--) | Λαμβάνει το διάστημα γραμμής. |
| [getParagraphStyle()](#getParagraphStyle--) | Λαμβάνει το στυλ παραγράφου. |
| [getSpaceAfter()](#getSpaceAfter--) | Λαμβάνει το ελάχιστο ποσό χώρου μετά. |
| [getSpaceBefore()](#getSpaceBefore--) | Λαμβάνει το ελάχιστο ποσό χώρου πριν. |
| [getStyles()](#getStyles--) | Λαμβάνει τα στυλ. |
| [getTags()](#getTags--) | Λαμβάνει τη λίστα όλων των ετικετών μιας παραγράφου. |
| [getText()](#getText--) | Λαμβάνει το κείμενο. |
| [getTextRuns()](#getTextRuns--) |  |
| [indexOf(char value)](#indexOf-char-) | Επιστρέφει τον μηδενικό δείκτη της πρώτης εμφάνισης του καθορισμένου χαρακτήρα Unicode σε αυτή τη συμβολοσειρά. |
| [indexOf(char value, int startIndex)](#indexOf-char-int-) | Επιστρέφει τον μηδενικό δείκτη της πρώτης εμφάνισης του καθορισμένου χαρακτήρα Unicode σε αυτή τη συμβολοσειρά. |
| [indexOf(char value, int startIndex, int count)](#indexOf-char-int-int-) | Επιστρέφει τον μηδενικό δείκτη της πρώτης εμφάνισης του καθορισμένου χαρακτήρα σε αυτή την παρουσία. |
| [indexOf(String value)](#indexOf-java.lang.String-) | Επιστρέφει τον μηδενικό δείκτη της πρώτης εμφάνισης της καθορισμένης συμβολοσειράς σε αυτή την παρουσία. |
| [indexOf(String value, int startIndex)](#indexOf-java.lang.String-int-) | Επιστρέφει τον μηδενικό δείκτη της πρώτης εμφάνισης της καθορισμένης συμβολοσειράς σε αυτή την παρουσία. |
| [indexOf(String value, int startIndex, int count)](#indexOf-java.lang.String-int-int-) | Επιστρέφει τον μηδενικό δείκτη της πρώτης εμφάνισης της καθορισμένης συμβολοσειράς σε αυτή την παρουσία. |
| [indexOf(String value, int startIndex, int count, short comparisonType)](#indexOf-java.lang.String-int-int-short-) | Επιστρέφει τον μηδενικό δείκτη της πρώτης εμφάνισης της καθορισμένης συμβολοσειράς στην τρέχουσα παρουσία. |
| [indexOf(String value, short comparisonType)](#indexOf-java.lang.String-short-) | Επιστρέφει τον μηδενικό δείκτη της πρώτης εμφάνισης της καθορισμένης συμβολοσειράς στην τρέχουσα παρουσία. |
| [indexOf_Rename_Namesake(String value, int startIndex, short comparisonType)](#indexOf-Rename-Namesake-java.lang.String-int-short-) | Επιστρέφει τον μηδενικό δείκτη της πρώτης εμφάνισης της καθορισμένης συμβολοσειράς στην τρέχουσα παρουσία. |
| [insert(int startIndex, String value)](#insert-int-java.lang.String-) | Εισάγει μια καθορισμένη συμβολοσειρά σε μια καθορισμένη θέση δείκτη σε αυτή την παρουσία. |
| [insert(int startIndex, String value, TextStyle style)](#insert-int-java.lang.String-com.aspose.note.TextStyle-) | Εισάγει μια καθορισμένη συμβολοσειρά με καθορισμένο στυλ σε μια καθορισμένη θέση δείκτη σε αυτή την παρουσία. |
| [iterator()](#iterator--) |  |
| [remove(int startIndex)](#remove-int-) | Αφαιρεί όλους τους χαρακτήρες στην τρέχουσα παρουσία, ξεκινώντας από μια καθορισμένη θέση και συνεχίζοντας μέχρι την τελευταία θέση. |
| [remove(int startIndex, int count)](#remove-int-int-) | Αφαιρεί καθορισμένο αριθμό χαρακτήρων στην τρέχουσα παρουσία, ξεκινώντας από μια καθορισμένη θέση. |
| [replace(char oldChar, char newChar)](#replace-char-char-) | Αντικαθιστά όλες τις εμφανίσεις ενός καθορισμένου χαρακτήρα Unicode σε αυτή την παρουσία με έναν άλλο καθορισμένο χαρακτήρα Unicode. |
| [replace(String oldValue, String newValue)](#replace-java.lang.String-java.lang.String-) | Αντικαθιστά όλες τις εμφανίσεις μιας καθορισμένης συμβολοσειράς στην τρέχουσα παρουσία με μια άλλη καθορισμένη συμβολοσειρά. |
| [replace(String oldValue, String newValue, TextStyle style)](#replace-java.lang.String-java.lang.String-com.aspose.note.TextStyle-) | Αντικαθιστά όλες τις εμφανίσεις μιας καθορισμένης συμβολοσειράς στην τρέχουσα παρουσία με μια άλλη καθορισμένη συμβολοσειρά σε καθορισμένο στυλ. |
| [setAlignment(int value)](#setAlignment-int-) | Ορίζει την ευθυγράμμιση. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Ορίζει την ώρα τελευταίας τροποποίησης. |
| [setLineSpacing(float value)](#setLineSpacing-float-) |  |
| [setLineSpacing(Float value)](#setLineSpacing-java.lang.Float-) | Ορίζει το διάστημα γραμμής. |
| [setParagraphStyle(ParagraphStyle value)](#setParagraphStyle-com.aspose.note.ParagraphStyle-) | Ορίζει το στυλ παραγράφου. |
| [setSpaceAfter(float value)](#setSpaceAfter-float-) |  |
| [setSpaceAfter(Float value)](#setSpaceAfter-java.lang.Float-) | Ορίζει το ελάχιστο ποσό χώρου μετά. |
| [setSpaceBefore(float value)](#setSpaceBefore-float-) |  |
| [setSpaceBefore(Float value)](#setSpaceBefore-java.lang.Float-) | Ορίζει το ελάχιστο ποσό χώρου πριν. |
| [setText(String value)](#setText-java.lang.String-) | Ορίζει το κείμενο. |
| [trim()](#trim--) | Αφαιρεί όλους τους αρχικούς και τελικούς χαρακτήρες λευκού διαστήματος. |
| [trim(char trimChar)](#trim-char-) | Αφαιρεί όλες τις αρχικές και τελικές εμφανίσεις ενός χαρακτήρα. |
| [trim(char[] trimChars)](#trim-char...-) | Αφαιρεί όλες τις αρχικές και τελικές εμφανίσεις ενός συνόλου χαρακτήρων που καθορίζονται σε έναν πίνακα. |
| [trimEnd()](#trimEnd--) | Αφαιρεί όλους τους τελικούς χαρακτήρες λευκού διαστήματος. |
| [trimEnd(char trimChar)](#trimEnd-char-) | Αφαιρεί όλες τις τελικές εμφανίσεις ενός χαρακτήρα. |
| [trimEnd(char[] trimChars)](#trimEnd-char...-) | Αφαιρεί όλες τις τελικές εμφανίσεις ενός συνόλου χαρακτήρων που καθορίζονται σε έναν πίνακα. |
| [trimStart()](#trimStart--) | Αφαιρεί όλους τους αρχικούς χαρακτήρες λευκού διαστήματος. |
| [trimStart(char trimChar)](#trimStart-char-) | Αφαιρεί όλες τις αρχικές εμφανίσεις ενός καθορισμένου χαρακτήρα. |
| [trimStart(char[] trimChars)](#trimStart-char...-) | Αφαιρεί όλες τις αρχικές εμφανίδες ενός συνόλου χαρακτήρων που καθορίζονται σε έναν πίνακα. |
### RichText() {#RichText--}
```
public RichText()
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [RichText](../../com.aspose.note/richtext).

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Δέχεται τον επισκέπτη του κόμβου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | Το αντικείμενο μιας κλάσης που προέρχεται από το [DocumentVisitor](../../com.aspose.note/documentvisitor). |

### append(String value) {#append-java.lang.String-}
```
public RichText append(String value)
```


Προσθέτει μια συμβολοσειρά στην τελευταία περιοχή κειμένου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | Η προστιθέμενη τιμή. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### append(String value, TextStyle style) {#append-java.lang.String-com.aspose.note.TextStyle-}
```
public final RichText append(String value, TextStyle style)
```


Προσθέτει μια συμβολοσειρά στο τέλος.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | Η προστιθέμενη τιμή. |
| style | [TextStyle](../../com.aspose.note/textstyle) | Το στυλ της προστιθέμενης συμβολοσειράς. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### appendFront(String value) {#appendFront-java.lang.String-}
```
public RichText appendFront(String value)
```


Προσθέτει μια συμβολοσειρά στην αρχή της πρώτης περιοχής κειμένου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | Η προστιθέμενη τιμή. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### appendFront(String value, TextStyle style) {#appendFront-java.lang.String-com.aspose.note.TextStyle-}
```
public RichText appendFront(String value, TextStyle style)
```


Προσθέτει μια συμβολοσειρά στην αρχή.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | Η προστιθέμενη τιμή. |
| style | [TextStyle](../../com.aspose.note/textstyle) | Το στυλ της προστιθέμενης συμβολοσειράς. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### clear() {#clear--}
```
public final RichText clear()
```


Καθαρίζει το περιεχόμενο αυτού του αντικειμένου.

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### getAlignment() {#getAlignment--}
```
public int getAlignment()
```


Λαμβάνει την ευθυγράμμιση.

**Returns:**
int
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Λαμβάνει την ώρα τελευταίας τροποποίησης.

**Returns:**
java.util.Date
### getLength() {#getLength--}
```
public final int getLength()
```




**Returns:**
int
### getLineSpacing() {#getLineSpacing--}
```
public Float getLineSpacing()
```


Λαμβάνει το διάστημα γραμμής.

**Returns:**
java.lang.Float
### getParagraphStyle() {#getParagraphStyle--}
```
public final ParagraphStyle getParagraphStyle()
```


Λαμβάνει το στυλ παραγράφου. Αυτές οι ρυθμίσεις χρησιμοποιούνται εάν δεν υπάρχει αντικείμενο TextStyle που ταιριάζει στη συλλογή [getStyles](../../com.aspose.note/richtext\#getStyles) ή εάν αυτό το αντικείμενο δεν καθορίζει την απαιτούμενη ρύθμιση.

**Returns:**
[ParagraphStyle](../../com.aspose.note/paragraphstyle)
### getSpaceAfter() {#getSpaceAfter--}
```
public Float getSpaceAfter()
```


Λαμβάνει το ελάχιστο ποσό χώρου μετά.

**Returns:**
java.lang.Float
### getSpaceBefore() {#getSpaceBefore--}
```
public Float getSpaceBefore()
```


Λαμβάνει το ελάχιστο ποσό χώρου πριν.

**Returns:**
java.lang.Float
### getStyles() {#getStyles--}
```
public System.Collections.Generic.IGenericEnumerable<TextStyle> getStyles()
```


Λαμβάνει τα στυλ.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerable&lt;com.aspose.note.TextStyle&gt;
### getTags() {#getTags--}
```
public final System.Collections.Generic.List<ITag> getTags()
```


Λαμβάνει τη λίστα όλων των ετικετών μιας παραγράφου.

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.note.ITag&gt;
### getText() {#getText--}
```
public final String getText()
```


Λαμβάνει το κείμενο. Η συμβολοσειρά ΔΕΝ ΠΡΕΠΕΙ ΝΑ περιέχει κανέναν χαρακτήρα της τιμής 10 (αλλαγή γραμμής).

**Returns:**
java.lang.String
### getTextRuns() {#getTextRuns--}
```
public final System.Collections.Generic.IGenericEnumerable<TextRun> getTextRuns()
```




**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerable&lt;com.aspose.note.TextRun&gt;
### indexOf(char value) {#indexOf-char-}
```
public final int indexOf(char value)
```


Επιστρέφει τον μηδενικό δείκτη της πρώτης εμφάνισης του καθορισμένου χαρακτήρα Unicode σε αυτή τη συμβολοσειρά.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | char | Η τιμή. |

**Returns:**
int - Το `int`.
### indexOf(char value, int startIndex) {#indexOf-char-int-}
```
public final int indexOf(char value, int startIndex)
```


Επιστρέφει τον μηδενικό δείκτη της πρώτης εμφάνισης του καθορισμένου χαρακτήρα Unicode σε αυτή τη συμβολοσειρά. Η αναζήτηση ξεκινά σε μια καθορισμένη θέση χαρακτήρα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | char | Η τιμή. |
| startIndex | int | Η αρχική θέση αναζήτησης. |

**Returns:**
int - Το `int`.
### indexOf(char value, int startIndex, int count) {#indexOf-char-int-int-}
```
public final int indexOf(char value, int startIndex, int count)
```


Επιστρέφει τον μηδενικό δείκτη της πρώτης εμφάνισης του καθορισμένου χαρακτήρα σε αυτή την περίπτωση. Η αναζήτηση ξεκινά σε μια καθορισμένη θέση χαρακτήρα και εξετάζει έναν καθορισμένο αριθμό θέσεων χαρακτήρων.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | char | Η τιμή. |
| startIndex | int | Η αρχική θέση αναζήτησης. |
| count | int | Ο αριθμός. |

**Returns:**
int - Το `int`.
### indexOf(String value) {#indexOf-java.lang.String-}
```
public final int indexOf(String value)
```


Επιστρέφει τον μηδενικό δείκτη της πρώτης εμφάνισης της καθορισμένης συμβολοσειράς σε αυτή την παρουσία.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | Η τιμή. |

**Returns:**
int - Το `int`.
### indexOf(String value, int startIndex) {#indexOf-java.lang.String-int-}
```
public final int indexOf(String value, int startIndex)
```


Επιστρέφει τον δείκτη μηδενικής βάσης της πρώτης εμφάνισης της καθορισμένης συμβολοσειράς σε αυτήν την περίπτωση. Η αναζήτηση ξεκινά σε μια καθορισμένη θέση χαρακτήρα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | Η τιμή. |
| startIndex | int | Η αρχική θέση αναζήτησης. |

**Returns:**
int - Το `int`.
### indexOf(String value, int startIndex, int count) {#indexOf-java.lang.String-int-int-}
```
public final int indexOf(String value, int startIndex, int count)
```


Επιστρέφει τον δείκτη μηδενικής βάσης της πρώτης εμφάνισης της καθορισμένης συμβολοσειράς σε αυτήν την περίπτωση. Η αναζήτηση ξεκινά σε μια καθορισμένη θέση χαρακτήρα και εξετάζει έναν καθορισμένο αριθμό θέσεων χαρακτήρων.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | Η τιμή. |
| startIndex | int | Η αρχική θέση αναζήτησης. |
| count | int | Ο αριθμός. |

**Returns:**
int - Το `int`.
### indexOf(String value, int startIndex, int count, short comparisonType) {#indexOf-java.lang.String-int-int-short-}
```
public final int indexOf(String value, int startIndex, int count, short comparisonType)
```


Επιστρέφει τον μηδενικό δείκτη της πρώτης εμφάνισης της καθορισμένης συμβολοσειράς στην τρέχουσα παρουσία.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | Η τιμή. |
| startIndex | int | Η αρχική θέση αναζήτησης. |
| count | int | Ο αριθμός. |
| comparisonType | short | Ο τύπος αναζήτησης που θα χρησιμοποιηθεί για τη καθορισμένη συμβολοσειρά |

**Returns:**
int - Το `int`.
### indexOf(String value, short comparisonType) {#indexOf-java.lang.String-short-}
```
public final int indexOf(String value, short comparisonType)
```


Επιστρέφει τον δείκτη μηδενικής βάσης της πρώτης εμφάνισης της καθορισμένης συμβολοσειράς στην τρέχουσα περίπτωση. Ένα παράμετρος καθορίζει τον τύπο αναζήτησης που θα χρησιμοποιηθεί για τη καθορισμένη συμβολοσειρά.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | Η τιμή. |
| comparisonType | short | Ο τύπος αναζήτησης που θα χρησιμοποιηθεί για τη καθορισμένη συμβολοσειρά |

**Returns:**
int - Το `int`.
### indexOf_Rename_Namesake(String value, int startIndex, short comparisonType) {#indexOf-Rename-Namesake-java.lang.String-int-short-}
```
public final int indexOf_Rename_Namesake(String value, int startIndex, short comparisonType)
```


Επιστρέφει τον δείκτη μηδενικής βάσης της πρώτης εμφάνισης της καθορισμένης συμβολοσειράς στην τρέχουσα περίπτωση. Οι παράμετροι καθορίζουν τη θέση έναρξης της αναζήτησης στην τρέχουσα συμβολοσειρά και τον τύπο αναζήτησης που θα χρησιμοποιηθεί για τη καθορισμένη συμβολοσειρά.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | Η τιμή. |
| startIndex | int | Η αρχική θέση αναζήτησης. |
| comparisonType | short | Ο τύπος αναζήτησης που θα χρησιμοποιηθεί για τη καθορισμένη συμβολοσειρά |

**Returns:**
int - Το `int`.
### insert(int startIndex, String value) {#insert-int-java.lang.String-}
```
public final RichText insert(int startIndex, String value)
```


Εισάγει μια καθορισμένη συμβολοσειρά σε μια καθορισμένη θέση δείκτη σε αυτή την παρουσία.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| startIndex | int | Ο δείκτης έναρξης. |
| τιμή | java.lang.String | Η τιμή. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### insert(int startIndex, String value, TextStyle style) {#insert-int-java.lang.String-com.aspose.note.TextStyle-}
```
public final RichText insert(int startIndex, String value, TextStyle style)
```


Εισάγει μια καθορισμένη συμβολοσειρά με καθορισμένο στυλ σε μια καθορισμένη θέση δείκτη σε αυτή την παρουσία.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| startIndex | int | Ο δείκτης έναρξης. |
| τιμή | java.lang.String | Η τιμή. |
| style | [TextStyle](../../com.aspose.note/textstyle) | Το στυλ. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<Character> iterator()
```




**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;java.lang.Character&gt;
### remove(int startIndex) {#remove-int-}
```
public final RichText remove(int startIndex)
```


Αφαιρεί όλους τους χαρακτήρες στην τρέχουσα παρουσία, ξεκινώντας από μια καθορισμένη θέση και συνεχίζοντας μέχρι την τελευταία θέση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| startIndex | int | Ο δείκτης έναρξης. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### remove(int startIndex, int count) {#remove-int-int-}
```
public final RichText remove(int startIndex, int count)
```


Αφαιρεί καθορισμένο αριθμό χαρακτήρων στην τρέχουσα παρουσία, ξεκινώντας από μια καθορισμένη θέση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| startIndex | int | Ο δείκτης έναρξης. |
| count | int | Ο αριθμός. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### replace(char oldChar, char newChar) {#replace-char-char-}
```
public final RichText replace(char oldChar, char newChar)
```


Αντικαθιστά όλες τις εμφανίσεις ενός καθορισμένου χαρακτήρα Unicode σε αυτή την παρουσία με έναν άλλο καθορισμένο χαρακτήρα Unicode.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| oldChar | char | Ο παλιός χαρακτήρας. |
| newChar | char | Ο νέος χαρακτήρας. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### replace(String oldValue, String newValue) {#replace-java.lang.String-java.lang.String-}
```
public final RichText replace(String oldValue, String newValue)
```


Αντικαθιστά όλες τις εμφανίσεις μιας καθορισμένης συμβολοσειράς στην τρέχουσα παρουσία με μια άλλη καθορισμένη συμβολοσειρά.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| oldValue | java.lang.String | Η παλιά τιμή. |
| newValue | java.lang.String | Η νέα τιμή. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### replace(String oldValue, String newValue, TextStyle style) {#replace-java.lang.String-java.lang.String-com.aspose.note.TextStyle-}
```
public final RichText replace(String oldValue, String newValue, TextStyle style)
```


Αντικαθιστά όλες τις εμφανίσεις μιας καθορισμένης συμβολοσειράς στην τρέχουσα παρουσία με μια άλλη καθορισμένη συμβολοσειρά σε καθορισμένο στυλ.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| oldValue | java.lang.String | Η παλιά τιμή. |
| newValue | java.lang.String | Η νέα τιμή. |
| style | [TextStyle](../../com.aspose.note/textstyle) | Το στυλ της νέας τιμής. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### setAlignment(int value) {#setAlignment-int-}
```
public void setAlignment(int value)
```


Ορίζει την ευθυγράμμιση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Ορίζει την ώρα τελευταίας τροποποίησης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.util.Date |  |

### setLineSpacing(float value) {#setLineSpacing-float-}
```
public void setLineSpacing(float value)
```




**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | float |  |

### setLineSpacing(Float value) {#setLineSpacing-java.lang.Float-}
```
public void setLineSpacing(Float value)
```


Ορίζει το διάστημα γραμμής.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.Float |  |

### setParagraphStyle(ParagraphStyle value) {#setParagraphStyle-com.aspose.note.ParagraphStyle-}
```
public final void setParagraphStyle(ParagraphStyle value)
```


Ορίζει το στυλ παραγράφου. Αυτές οι ρυθμίσεις χρησιμοποιούνται εάν δεν υπάρχει αντικείμενο TextStyle που ταιριάζει στη συλλογή [getStyles](../../com.aspose.note/richtext\#getStyles), ή εάν αυτό το αντικείμενο δεν καθορίζει την απαιτούμενη ρύθμιση.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [ParagraphStyle](../../com.aspose.note/paragraphstyle) |  |

### setSpaceAfter(float value) {#setSpaceAfter-float-}
```
public void setSpaceAfter(float value)
```




**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | float |  |

### setSpaceAfter(Float value) {#setSpaceAfter-java.lang.Float-}
```
public void setSpaceAfter(Float value)
```


Ορίζει το ελάχιστο ποσό χώρου μετά.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.Float |  |

### setSpaceBefore(float value) {#setSpaceBefore-float-}
```
public void setSpaceBefore(float value)
```




**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | float |  |

### setSpaceBefore(Float value) {#setSpaceBefore-java.lang.Float-}
```
public void setSpaceBefore(Float value)
```


Ορίζει το ελάχιστο ποσό χώρου πριν.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.Float |  |

### setText(String value) {#setText-java.lang.String-}
```
public final void setText(String value)
```


Ορίζει το κείμενο. Η συμβολοσειρά ΠΡΕΠΕΙ να μην περιέχει κανέναν χαρακτήρα με τιμή 10 (αλλαγή γραμμής).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String |  |

### trim() {#trim--}
```
public final RichText trim()
```


Αφαιρεί όλους τους αρχικούς και τελικούς χαρακτήρες λευκού διαστήματος.

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trim(char trimChar) {#trim-char-}
```
public final RichText trim(char trimChar)
```


Αφαιρεί όλες τις αρχικές και τελικές εμφανίσεις ενός χαρακτήρα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| trimChar | char | Ο χαρακτήρας περικοπής. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trim(char[] trimChars) {#trim-char...-}
```
public final RichText trim(char[] trimChars)
```


Αφαιρεί όλες τις αρχικές και τελικές εμφανίσεις ενός συνόλου χαρακτήρων που καθορίζονται σε έναν πίνακα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| trimChars | char[] | Τα χαρακτήρες περικοπής. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimEnd() {#trimEnd--}
```
public final RichText trimEnd()
```


Αφαιρεί όλους τους τελικούς χαρακτήρες λευκού διαστήματος.

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimEnd(char trimChar) {#trimEnd-char-}
```
public final RichText trimEnd(char trimChar)
```


Αφαιρεί όλες τις τελικές εμφανίσεις ενός χαρακτήρα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| trimChar | char | Ο χαρακτήρας περικοπής. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimEnd(char[] trimChars) {#trimEnd-char...-}
```
public final RichText trimEnd(char[] trimChars)
```


Αφαιρεί όλες τις τελικές εμφανίσεις ενός συνόλου χαρακτήρων που καθορίζονται σε έναν πίνακα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| trimChars | char[] | Τα χαρακτήρες περικοπής. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimStart() {#trimStart--}
```
public final RichText trimStart()
```


Αφαιρεί όλους τους αρχικούς χαρακτήρες λευκού διαστήματος.

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimStart(char trimChar) {#trimStart-char-}
```
public final RichText trimStart(char trimChar)
```


Αφαιρεί όλες τις αρχικές εμφανίσεις ενός καθορισμένου χαρακτήρα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| trimChar | char | Ο χαρακτήρας περικοπής. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimStart(char[] trimChars) {#trimStart-char...-}
```
public final RichText trimStart(char[] trimChars)
```


Αφαιρεί όλες τις αρχικές εμφανίδες ενός συνόλου χαρακτήρων που καθορίζονται σε έναν πίνακα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| trimChars | char[] | Τα χαρακτήρες περικοπής. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
