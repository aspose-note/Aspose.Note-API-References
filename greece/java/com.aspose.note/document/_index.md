---
title: "Document"
second_title: "Aspose.Note για Java Αναφορά API"
description: "Αναπαριστά ένα έγγραφο Aspose.Note."
type: docs
weight: 20
url: /el/java/com.aspose.note/document/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode

**All Implemented Interfaces:**
[com.aspose.note.INotebookChildNode](../../com.aspose.note/inotebookchildnode)
```
public class Document extends CompositeNode<Page> implements INotebookChildNode
```

Αναπαριστά ένα έγγραφο Aspose.Note.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [Document()](#Document--) | Αρχικοποιεί μια νέα παρουσία της κλάσης `Document`. |
| [Document(String filePath)](#Document-java.lang.String-) | Αρχικοποιεί μια νέα παρουσία της κλάσης `Document`. |
| [Document(String filePath, LoadOptions loadOptions)](#Document-java.lang.String-com.aspose.note.LoadOptions-) | Αρχικοποιεί μια νέα παρουσία της κλάσης `Document`. |
| [Document(InputStream inStream)](#Document-java.io.InputStream-) | Αρχικοποιεί μια νέα παρουσία της κλάσης `Document`. |
| [Document(InputStream inStream, LoadOptions loadOptions)](#Document-java.io.InputStream-com.aspose.note.LoadOptions-) | Αρχικοποιεί μια νέα παρουσία της κλάσης `Document`. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Δέχεται τον επισκέπτη του κόμβου. |
| [detectLayoutChanges()](#detectLayoutChanges--) | Ανιχνεύει όλες τις αλλαγές που έγιναν στη διάταξη του εγγράφου από την προηγούμενη κλήση του `DetectLayoutChanges`. |
| [getAutomaticLayoutChangesDetectionEnabled()](#getAutomaticLayoutChangesDetectionEnabled--) | Λαμβάνει μια τιμή που υποδεικνύει αν το Aspose.Note εκτελεί αυτόματη ανίχνευση αλλαγών διάταξης. |
| [getColor()](#getColor--) | Λαμβάνει το χρώμα. |
| [getCreationTime()](#getCreationTime--) | Λαμβάνει την ώρα δημιουργίας. |
| [getDisplayName()](#getDisplayName--) | Λαμβάνει το εμφανιζόμενο όνομα. |
| [getFileFormat()](#getFileFormat--) | Λαμβάνει τη μορφή αρχείου (OneNote 2010, OneNote Online). |
| [getGuid()](#getGuid--) | Λαμβάνει το παγκοσμίως μοναδικό αναγνωριστικό του αντικειμένου. |
| [getGuidInternal()](#getGuidInternal--) |  |
| [getPageHistory(Page page)](#getPageHistory-com.aspose.note.Page-) | Λαμβάνει το `PageHistory` που περιέχει πλήρη ιστορικό για κάθε σελίδα που παρουσιάζεται σε ένα έγγραφο (η πιο παλιά στη θέση 0). |
| [isEncrypted(InputStream stream, Document[] document)](#isEncrypted-java.io.InputStream-com.aspose.note.Document---) | Ελέγχει εάν ένα έγγραφο από ροή είναι κρυπτογραφημένο. |
| [isEncrypted(InputStream stream, LoadOptions options, Document[] document)](#isEncrypted-java.io.InputStream-com.aspose.note.LoadOptions-com.aspose.note.Document---) | Ελέγχει εάν ένα έγγραφο από ροή είναι κρυπτογραφημένο. |
| [isEncrypted(InputStream stream, String password, Document[] document)](#isEncrypted-java.io.InputStream-java.lang.String-com.aspose.note.Document---) | Ελέγχει εάν ένα έγγραφο από ροή είναι κρυπτογραφημένο. |
| [isEncrypted(String filePath, Document[] document)](#isEncrypted-java.lang.String-com.aspose.note.Document---) | Ελέγχει εάν ένα έγγραφο από αρχείο είναι κρυπτογραφημένο. |
| [isEncrypted(String filePath, LoadOptions options, Document[] document)](#isEncrypted-java.lang.String-com.aspose.note.LoadOptions-com.aspose.note.Document---) | Ελέγχει εάν ένα έγγραφο από αρχείο είναι κρυπτογραφημένο. |
| [isEncrypted(String filePath, String password, Document[] document)](#isEncrypted-java.lang.String-java.lang.String-com.aspose.note.Document---) | Ελέγχει εάν ένα έγγραφο από αρχείο είναι κρυπτογραφημένο. |
| [print()](#print--) | Εκτυπώνει το έγγραφο χρησιμοποιώντας τον προεπιλεγμένο εκτυπωτή. |
| [print(PrintOptions options)](#print-com.aspose.note.PrintOptions-) | Εκτυπώνει το έγγραφο χρησιμοποιώντας τον προεπιλεγμένο εκτυπωτή. |
| [print(String printerName)](#print-java.lang.String-) | Εκτυπώνει το έγγραφο χρησιμοποιώντας τον προεπιλεγμένο εκτυπωτή. |
| [print(AttributeSet printSettings)](#print-javax.print.attribute.AttributeSet-) | Εκτυπώνει το έγγραφο χρησιμοποιώντας τον προεπιλεγμένο εκτυπωτή. |
| [save(OutputStream stream)](#save-java.io.OutputStream-) | Αποθηκεύει το έγγραφο OneNote σε μια ροή. |
| [save(OutputStream stream, SaveOptions options)](#save-java.io.OutputStream-com.aspose.note.SaveOptions-) | Αποθηκεύει το έγγραφο OneNote σε μια ροή χρησιμοποιώντας τις καθορισμένες επιλογές αποθήκευσης. |
| [save(OutputStream stream, int format)](#save-java.io.OutputStream-int-) | Αποθηκεύει το έγγραφο OneNote σε μια ροή στη καθορισμένη μορφή. |
| [save(String fileName)](#save-java.lang.String-) | Αποθηκεύει το έγγραφο OneNote σε ένα αρχείο. |
| [save(String fileName, SaveOptions options)](#save-java.lang.String-com.aspose.note.SaveOptions-) | Αποθηκεύει το έγγραφο OneNote σε ένα αρχείο χρησιμοποιώντας τις καθορισμένες επιλογές αποθήκευσης. |
| [save(String fileName, int format)](#save-java.lang.String-int-) | Αποθηκεύει το έγγραφο OneNote σε ένα αρχείο στη καθορισμένη μορφή. |
| [setAutomaticLayoutChangesDetectionEnabled(boolean value)](#setAutomaticLayoutChangesDetectionEnabled-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν το Aspose.Note εκτελεί αυτόματα ανίχνευση αλλαγών διάταξης. |
| [setColor(Color value)](#setColor-java.awt.Color-) | Ορίζει το χρώμα. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Ορίζει την ώρα δημιουργίας. |
| [setDisplayName(String value)](#setDisplayName-java.lang.String-) | Ορίζει το εμφανιζόμενο όνομα. |
### Document() {#Document--}
```
public Document()
```


Αρχικοποιεί μια νέα παρουσία της κλάσης `Document`. Δημιουργεί ένα κενό έγγραφο OneNote.

### Document(String filePath) {#Document-java.lang.String-}
```
public Document(String filePath)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης `Document`. Ανοίγει ένα υπάρχον έγγραφο OneNote από αρχείο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| filePath | java.lang.String | Η διαδρομή του αρχείου. |

### Document(String filePath, LoadOptions loadOptions) {#Document-java.lang.String-com.aspose.note.LoadOptions-}
```
public Document(String filePath, LoadOptions loadOptions)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης `Document`. Ανοίγει ένα υπάρχον έγγραφο OneNote από αρχείο. Επιτρέπει τον καθορισμό πρόσθετων επιλογών όπως ένας κωδικός κρυπτογράφησης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| filePath | java.lang.String | Η διαδρομή του αρχείου. |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | Επιλογές που χρησιμοποιούνται για τη φόρτωση ενός εγγράφου. Μπορεί να είναι null. |

### Document(InputStream inStream) {#Document-java.io.InputStream-}
```
public Document(InputStream inStream)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης `Document`. Ανοίγει ένα υπάρχον έγγραφο OneNote από ροή.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| inStream | java.io.InputStream | Η ροή. |

### Document(InputStream inStream, LoadOptions loadOptions) {#Document-java.io.InputStream-com.aspose.note.LoadOptions-}
```
public Document(InputStream inStream, LoadOptions loadOptions)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης `Document`. Ανοίγει ένα υπάρχον έγγραφο OneNote από ροή. Επιτρέπει τον καθορισμό πρόσθετων επιλογών όπως ένας κωδικός κρυπτογράφησης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| inStream | java.io.InputStream | Η ροή. |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | Επιλογές που χρησιμοποιούνται για τη φόρτωση ενός εγγράφου. Μπορεί να είναι null. |

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Δέχεται τον επισκέπτη του κόμβου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | Το αντικείμενο μιας κλάσης που προέρχεται από το `DocumentVisitor`. |

### detectLayoutChanges() {#detectLayoutChanges--}
```
public void detectLayoutChanges()
```


Ανιχνεύει όλες τις αλλαγές που έγιναν στη διάταξη του εγγράφου από την προηγούμενη κλήση του `DetectLayoutChanges`. Σε περίπτωση που το `AutomaticLayoutChangesDetectionEnabled` είναι ορισμένο σε true, χρησιμοποιείται αυτόματα στην αρχή της εξαγωγής του εγγράφου.

### getAutomaticLayoutChangesDetectionEnabled() {#getAutomaticLayoutChangesDetectionEnabled--}
```
public boolean getAutomaticLayoutChangesDetectionEnabled()
```


Λαμβάνει μια τιμή που υποδεικνύει εάν το Aspose.Note εκτελεί αυτόματα ανίχνευση αλλαγών διάταξης. Η προεπιλεγμένη τιμή είναι `true`.

**Returns:**
boolean
### getColor() {#getColor--}
```
public Color getColor()
```


Λαμβάνει το χρώμα.

**Returns:**
java.awt.Color
### getCreationTime() {#getCreationTime--}
```
public Date getCreationTime()
```


Λαμβάνει την ώρα δημιουργίας.

**Returns:**
java.util.Date
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


Λαμβάνει το εμφανιζόμενο όνομα.

**Returns:**
java.lang.String
### getFileFormat() {#getFileFormat--}
```
public int getFileFormat()
```


Λαμβάνει τη μορφή αρχείου (OneNote 2010, OneNote Online).

**Returns:**
int
### getGuid() {#getGuid--}
```
public UUID getGuid()
```


Λαμβάνει το παγκοσμίως μοναδικό αναγνωριστικό του αντικειμένου.

**Returns:**
java.util.UUID
### getGuidInternal() {#getGuidInternal--}
```
public System.Guid getGuidInternal()
```




**Returns:**
com.aspose.ms.System.Guid
### getPageHistory(Page page) {#getPageHistory-com.aspose.note.Page-}
```
public PageHistory getPageHistory(Page page)
```


Λαμβάνει το `PageHistory` που περιέχει πλήρες ιστορικό για κάθε σελίδα που παρουσιάζεται σε ένα έγγραφο (η πιο παλιά στη θέση 0). Η τρέχουσα αναθεώρηση της σελίδας μπορεί να προσπελαστεί ως `PageHistory.current` και είναι αποθηκευμένη ξεχωριστά από τη συλλογή των ιστορικών εκδόσεων.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | Η τρέχουσα αναθεώρηση μιας σελίδας. |

**Returns:**
[PageHistory](../../com.aspose.note/pagehistory) - The `PageHistory`.
### isEncrypted(InputStream stream, Document[] document) {#isEncrypted-java.io.InputStream-com.aspose.note.Document---}
```
public static boolean isEncrypted(InputStream stream, Document[] document)
```


Ελέγχει εάν ένα έγγραφο από ροή είναι κρυπτογραφημένο. Για να το ελέγξουμε, πρέπει να φορτώσουμε πλήρως αυτό το έγγραφο. Έτσι αυτή η μέθοδος μπορεί να προκαλέσει ποινή απόδοσης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ροή | java.io.InputStream | Η ροή. |
| document | [Document\[\]](../../com.aspose.note/document) | Το φορτωμένο έγγραφο. |

**Returns:**
boolean - Επιστρέφει true εάν το έγγραφο είναι κρυπτογραφημένο, διαφορετικά false.
### isEncrypted(InputStream stream, LoadOptions options, Document[] document) {#isEncrypted-java.io.InputStream-com.aspose.note.LoadOptions-com.aspose.note.Document---}
```
public static boolean isEncrypted(InputStream stream, LoadOptions options, Document[] document)
```


Ελέγχει εάν ένα έγγραφο από ροή είναι κρυπτογραφημένο. Για να το ελέγξουμε, πρέπει να φορτώσουμε πλήρως αυτό το έγγραφο. Έτσι αυτή η μέθοδος μπορεί να προκαλέσει ποινή απόδοσης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ροή | java.io.InputStream | Η ροή. |
| options | [LoadOptions](../../com.aspose.note/loadoptions) | Οι επιλογές φόρτωσης. |
| document | [Document\[\]](../../com.aspose.note/document) | Το φορτωμένο έγγραφο. |

**Returns:**
boolean - Επιστρέφει true εάν το έγγραφο είναι κρυπτογραφημένο, διαφορετικά false.
### isEncrypted(InputStream stream, String password, Document[] document) {#isEncrypted-java.io.InputStream-java.lang.String-com.aspose.note.Document---}
```
public static boolean isEncrypted(InputStream stream, String password, Document[] document)
```


Ελέγχει εάν ένα έγγραφο από ροή είναι κρυπτογραφημένο. Για να το ελέγξουμε, πρέπει να φορτώσουμε πλήρως αυτό το έγγραφο. Έτσι αυτή η μέθοδος μπορεί να προκαλέσει ποινή απόδοσης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ροή | java.io.InputStream | Η ροή. |
| password | java.lang.String | Ο κωδικός για την αποκρυπτογράφηση ενός εγγράφου. |
| document | [Document\[\]](../../com.aspose.note/document) | Το φορτωμένο έγγραφο. |

**Returns:**
boolean - Επιστρέφει true εάν το έγγραφο είναι κρυπτογραφημένο, διαφορετικά false.
### isEncrypted(String filePath, Document[] document) {#isEncrypted-java.lang.String-com.aspose.note.Document---}
```
public static boolean isEncrypted(String filePath, Document[] document)
```


Ελέγχει εάν ένα έγγραφο από αρχείο είναι κρυπτογραφημένο. Για να το ελέγξουμε, πρέπει να φορτώσουμε πλήρως αυτό το έγγραφο. Έτσι αυτή η μέθοδος μπορεί να προκαλέσει ποινή απόδοσης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| filePath | java.lang.String | Η διαδρομή του αρχείου. |
| document | [Document\[\]](../../com.aspose.note/document) | Το φορτωμένο έγγραφο. |

**Returns:**
boolean - Επιστρέφει true εάν το έγγραφο είναι κρυπτογραφημένο, διαφορετικά false.
### isEncrypted(String filePath, LoadOptions options, Document[] document) {#isEncrypted-java.lang.String-com.aspose.note.LoadOptions-com.aspose.note.Document---}
```
public static boolean isEncrypted(String filePath, LoadOptions options, Document[] document)
```


Ελέγχει εάν ένα έγγραφο από αρχείο είναι κρυπτογραφημένο. Για να το ελέγξουμε, πρέπει να φορτώσουμε πλήρως αυτό το έγγραφο. Έτσι αυτή η μέθοδος μπορεί να προκαλέσει ποινή απόδοσης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| filePath | java.lang.String | Η διαδρομή του αρχείου. |
| options | [LoadOptions](../../com.aspose.note/loadoptions) | Οι επιλογές φόρτωσης. |
| document | [Document\[\]](../../com.aspose.note/document) | Το φορτωμένο έγγραφο. |

**Returns:**
boolean - Επιστρέφει true εάν το έγγραφο είναι κρυπτογραφημένο, διαφορετικά false.
### isEncrypted(String filePath, String password, Document[] document) {#isEncrypted-java.lang.String-java.lang.String-com.aspose.note.Document---}
```
public static boolean isEncrypted(String filePath, String password, Document[] document)
```


Ελέγχει εάν ένα έγγραφο από αρχείο είναι κρυπτογραφημένο. Για να το ελέγξουμε, πρέπει να φορτώσουμε πλήρως αυτό το έγγραφο. Έτσι αυτή η μέθοδος μπορεί να προκαλέσει ποινή απόδοσης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| filePath | java.lang.String | Η διαδρομή του αρχείου. |
| password | java.lang.String | Ο κωδικός για την αποκρυπτογράφηση ενός εγγράφου. |
| document | [Document\[\]](../../com.aspose.note/document) | Το φορτωμένο έγγραφο. |

**Returns:**
boolean - Επιστρέφει true εάν το έγγραφο είναι κρυπτογραφημένο, διαφορετικά false.
### print() {#print--}
```
public void print()
```


Εκτυπώνει το έγγραφο χρησιμοποιώντας τον προεπιλεγμένο εκτυπωτή.

### print(PrintOptions options) {#print-com.aspose.note.PrintOptions-}
```
public void print(PrintOptions options)
```


Εκτυπώνει το έγγραφο χρησιμοποιώντας τον προεπιλεγμένο εκτυπωτή.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| options | [PrintOptions](../../com.aspose.note/printoptions) | Επιλογές που χρησιμοποιούνται για την εκτύπωση ενός εγγράφου. Μπορεί να είναι null. |

### print(String printerName) {#print-java.lang.String-}
```
public void print(String printerName)
```


Εκτυπώνει το έγγραφο χρησιμοποιώντας τον προεπιλεγμένο εκτυπωτή.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| printerName | java.lang.String |  |

### print(AttributeSet printSettings) {#print-javax.print.attribute.AttributeSet-}
```
public void print(AttributeSet printSettings)
```


Εκτυπώνει το έγγραφο χρησιμοποιώντας τον προεπιλεγμένο εκτυπωτή.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| printSettings | javax.print.attribute.AttributeSet |  |

### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public void save(OutputStream stream)
```


Αποθηκεύει το έγγραφο OneNote σε μια ροή.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ροή | java.io.OutputStream | Το System.iO.stream όπου θα αποθηκευτεί το έγγραφο. |

### save(OutputStream stream, SaveOptions options) {#save-java.io.OutputStream-com.aspose.note.SaveOptions-}
```
public void save(OutputStream stream, SaveOptions options)
```


Αποθηκεύει το έγγραφο OneNote σε μια ροή χρησιμοποιώντας τις καθορισμένες επιλογές αποθήκευσης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ροή | java.io.OutputStream | Το System.iO.stream όπου θα αποθηκευτεί το έγγραφο. |
| options | [SaveOptions](../../com.aspose.note/saveoptions) | Καθορίζει τις επιλογές πώς το έγγραφο αποθηκεύεται στο stream. |

### save(OutputStream stream, int format) {#save-java.io.OutputStream-int-}
```
public void save(OutputStream stream, int format)
```


Αποθηκεύει το έγγραφο OneNote σε μια ροή στη καθορισμένη μορφή.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ροή | java.io.OutputStream | Το System.iO.stream όπου θα αποθηκευτεί το έγγραφο. |
| format | int | Η μορφή στην οποία θα αποθηκευτεί το έγγραφο. |

### save(String fileName) {#save-java.lang.String-}
```
public void save(String fileName)
```


Αποθηκεύει το έγγραφο OneNote σε ένα αρχείο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fileName | java.lang.String | Το πλήρες όνομα του αρχείου. Εάν υπάρχει ήδη αρχείο με το καθορισμένο πλήρες όνομα, το υπάρχον αρχείο θα αντικατασταθεί. |

### save(String fileName, SaveOptions options) {#save-java.lang.String-com.aspose.note.SaveOptions-}
```
public void save(String fileName, SaveOptions options)
```


Αποθηκεύει το έγγραφο OneNote σε ένα αρχείο χρησιμοποιώντας τις καθορισμένες επιλογές αποθήκευσης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fileName | java.lang.String | Το πλήρες όνομα του αρχείου. Εάν υπάρχει ήδη αρχείο με το καθορισμένο πλήρες όνομα, το υπάρχον αρχείο θα αντικατασταθεί. |
| options | [SaveOptions](../../com.aspose.note/saveoptions) | Καθορίζει τις επιλογές για το πώς αποθηκεύεται το έγγραφο σε αρχείο. |

### save(String fileName, int format) {#save-java.lang.String-int-}
```
public void save(String fileName, int format)
```


Αποθηκεύει το έγγραφο OneNote σε ένα αρχείο στη καθορισμένη μορφή.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fileName | java.lang.String | Το πλήρες όνομα του αρχείου. Εάν υπάρχει ήδη αρχείο με το καθορισμένο πλήρες όνομα, το υπάρχον αρχείο θα αντικατασταθεί. |
| format | int | Η μορφή στην οποία θα αποθηκευτεί το έγγραφο. |

### setAutomaticLayoutChangesDetectionEnabled(boolean value) {#setAutomaticLayoutChangesDetectionEnabled-boolean-}
```
public void setAutomaticLayoutChangesDetectionEnabled(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν το Aspose.Note εκτελεί αυτόματα ανίχνευση αλλαγών διάταξης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | Νέα τιμή. Μπορεί να είναι null. |

### setColor(Color value) {#setColor-java.awt.Color-}
```
public void setColor(Color value)
```


Ορίζει το χρώμα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.awt.Color | Τιμή του Color. |

### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public void setCreationTime(Date value)
```


Ορίζει την ώρα δημιουργίας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.util.Date | Τιμή του DateTime. |

### setDisplayName(String value) {#setDisplayName-java.lang.String-}
```
public void setDisplayName(String value)
```


Ορίζει το εμφανιζόμενο όνομα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String | Τιμή του DateTime. |

