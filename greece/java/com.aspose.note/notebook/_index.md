---
title: "Σημειωματάριο"
second_title: "Aspose.Note για Java Αναφορά API"
description: "Αντιπροσωπεύει ένα σημειωματάριο Aspose.Note."
type: docs
weight: 56
url: /el/java/com.aspose.note/notebook/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.note.INotebookChildNode](../../com.aspose.note/inotebookchildnode), com.aspose.ms.System.Collections.Generic.IGenericEnumerable
```
public class Notebook implements INotebookChildNode, System.Collections.Generic.IGenericEnumerable<INotebookChildNode>
```

Αντιπροσωπεύει ένα σημειωματάριο Aspose.Note.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [Notebook()](#Notebook--) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης `Notebook`. |
| [Notebook(String filePath)](#Notebook-java.lang.String-) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης `Notebook`. |
| [Notebook(String filePath, NotebookLoadOptions loadOptions)](#Notebook-java.lang.String-com.aspose.note.NotebookLoadOptions-) | Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης `Notebook`. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [&lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass)](#-T1-getChildNodes-java.lang.Class-T1--) | Λαμβάνει όλους τους κόμβους-παιδιά με βάση τον τύπο του κόμβου. |
| [appendChild(INotebookChildNode newChild)](#appendChild-com.aspose.note.INotebookChildNode-) | Προσθέτει τον κόμβο στο τέλος της λίστας. |
| [getColor()](#getColor--) | Λαμβάνει ή ορίζει το χρώμα. |
| [getCount()](#getCount--) | Λαμβάνει τον αριθμό των στοιχείων που περιέχονται στο `Notebook`. |
| [getDisplayName()](#getDisplayName--) | Λαμβάνει ή ορίζει το όνομα εμφάνισης. |
| [getFileFormat()](#getFileFormat--) | Λαμβάνει τη μορφή αρχείου (OneNote 2010, OneNote Online). |
| [getGuid()](#getGuid--) | Λαμβάνει το παγκοσμίως μοναδικό αναγνωριστικό του αντικειμένου. |
| [getGuidInternal()](#getGuidInternal--) |  |
| [get_Item(int index)](#get-Item-int-) | Λαμβάνει τον κόμβο-παιδί του σημειωματάριου με το δεδομένο δείκτη. |
| [isHistoryEnabled()](#isHistoryEnabled--) | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει αν το ιστορικό είναι ενεργοποιημένο. |
| [iterator()](#iterator--) | Επιστρέφει έναν απαριθμητή που διατρέχει τους κόμβους-παιδιά του `Notebook`. |
| [loadChildDocument(InputStream stream)](#loadChildDocument-java.io.InputStream-) | Προσθέτει έναν κόμβο εγγράφου-παιδί. |
| [loadChildDocument(InputStream stream, LoadOptions loadOptions)](#loadChildDocument-java.io.InputStream-com.aspose.note.LoadOptions-) | Προσθέτει έναν κόμβο εγγράφου-παιδί. |
| [loadChildDocument(String filePath)](#loadChildDocument-java.lang.String-) | Προσθέτει έναν κόμβο εγγράφου-παιδί. |
| [loadChildDocument(String filePath, LoadOptions loadOptions)](#loadChildDocument-java.lang.String-com.aspose.note.LoadOptions-) | Προσθέτει έναν κόμβο εγγράφου-παιδί. |
| [loadChildNotebook(String filePath)](#loadChildNotebook-java.lang.String-) | Προσθέτει έναν κόμβο σημειωματάριου-παιδί. |
| [loadChildNotebook(String filePath, NotebookLoadOptions loadOptions)](#loadChildNotebook-java.lang.String-com.aspose.note.NotebookLoadOptions-) | Προσθέτει έναν κόμβο σημειωματάριου-παιδί. |
| [removeChild(INotebookChildNode oldChild)](#removeChild-com.aspose.note.INotebookChildNode-) | Αφαιρεί τον κόμβο-παιδί. |
| [save(OutputStream stream)](#save-java.io.OutputStream-) | Αποθηκεύει το έγγραφο OneNote σε μια ροή. |
| [save(OutputStream stream, NotebookSaveOptions options)](#save-java.io.OutputStream-com.aspose.note.NotebookSaveOptions-) | Αποθηκεύει το έγγραφο OneNote σε μια ροή χρησιμοποιώντας τις καθορισμένες επιλογές αποθήκευσης. |
| [save(OutputStream stream, int format)](#save-java.io.OutputStream-int-) | Αποθηκεύει το έγγραφο OneNote σε μια ροή στη καθορισμένη μορφή. |
| [save(String fileName)](#save-java.lang.String-) | Αποθηκεύει το έγγραφο OneNote σε ένα αρχείο. |
| [save(String fileName, NotebookSaveOptions options)](#save-java.lang.String-com.aspose.note.NotebookSaveOptions-) | Αποθηκεύει το έγγραφο OneNote σε ένα αρχείο χρησιμοποιώντας τις καθορισμένες επιλογές αποθήκευσης. |
| [save(String fileName, int format)](#save-java.lang.String-int-) | Αποθηκεύει το έγγραφο OneNote σε ένα αρχείο στη καθορισμένη μορφή. |
| [setColor(Color value)](#setColor-java.awt.Color-) | Λαμβάνει ή ορίζει το χρώμα. |
| [setDisplayName(String value)](#setDisplayName-java.lang.String-) | Λαμβάνει ή ορίζει το όνομα εμφάνισης. |
| [setHistoryEnabled(boolean value)](#setHistoryEnabled-boolean-) | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει αν το ιστορικό είναι ενεργοποιημένο. |
### Notebook() {#Notebook--}
```
public Notebook()
```


Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης `Notebook`.

### Notebook(String filePath) {#Notebook-java.lang.String-}
```
public Notebook(String filePath)
```


Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης `Notebook`. Ανοίγει ένα υπάρχον σημειωματάριο OneNote από ένα αρχείο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| filePath | java.lang.String | Η διαδρομή του αρχείου. |

### Notebook(String filePath, NotebookLoadOptions loadOptions) {#Notebook-java.lang.String-com.aspose.note.NotebookLoadOptions-}
```
public Notebook(String filePath, NotebookLoadOptions loadOptions)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης `Notebook`. Ανοίγει ένα υπάρχον σημειωματάριο OneNote από ένα αρχείο. Επιτρέπει τον καθορισμό πρόσθετων επιλογών όπως μια στρατηγική φόρτωσης παιδιών ("lazy"/instant).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| filePath | java.lang.String | Η διαδρομή του αρχείου. |
| loadOptions | [NotebookLoadOptions](../../com.aspose.note/notebookloadoptions) | Οι επιλογές φόρτωσης. |

### &lt;T1&gt;getChildNodes(Class&lt;T1&gt; typeParameterClass) {#-T1-getChildNodes-java.lang.Class-T1--}
```
public List<T1> <T1>getChildNodes(Class<T1> typeParameterClass)
```


Λαμβάνει όλους τους κόμβους-παιδιά με βάση τον τύπο του κόμβου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| typeParameterClass | java.lang.Class&lt;T1&gt; |  |

**Returns:**
java.util.List&lt;T1&gt; - Μια λίστα παιδικών κόμβων.

`T1`: Ο τύπος των στοιχείων στη επιστρεφόμενη λίστα.
### appendChild(INotebookChildNode newChild) {#appendChild-com.aspose.note.INotebookChildNode-}
```
public INotebookChildNode appendChild(INotebookChildNode newChild)
```


Προσθέτει τον κόμβο στο τέλος της λίστας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| newChild | [INotebookChildNode](../../com.aspose.note/inotebookchildnode) | Ο κόμβος προς προσθήκη. |

**Returns:**
[INotebookChildNode](../../com.aspose.note/inotebookchildnode) - The added node.
### getColor() {#getColor--}
```
public Color getColor()
```


Λαμβάνει ή ορίζει το χρώμα.

**Returns:**
java.awt.Color
### getCount() {#getCount--}
```
public int getCount()
```


Λαμβάνει τον αριθμό των στοιχείων που περιέχονται στο `Notebook`.

**Returns:**
int
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


Λαμβάνει ή ορίζει το όνομα εμφάνισης.

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

Τιμή: Το GUID.

**Returns:**
java.util.UUID
### getGuidInternal() {#getGuidInternal--}
```
public System.Guid getGuidInternal()
```




**Returns:**
com.aspose.ms.System.Guid
### get_Item(int index) {#get-Item-int-}
```
public INotebookChildNode get_Item(int index)
```


Λαμβάνει τον κόμβο-παιδί του σημειωματάριου με το δεδομένο δείκτη.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| index | int | Δείκτης προς παιδικό κόμβο. |

**Returns:**
[INotebookChildNode](../../com.aspose.note/inotebookchildnode) - The child node on the `index` position.
### isHistoryEnabled() {#isHistoryEnabled--}
```
public boolean isHistoryEnabled()
```


Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει αν το ιστορικό είναι ενεργοποιημένο.

**Returns:**
boolean
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<INotebookChildNode> iterator()
```


Επιστρέφει έναν απαριθμητή που διατρέχει τους κόμβους-παιδιά του `Notebook`.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;com.aspose.note.INotebookChildNode&gt; - Ένα `IEnumerator`.
### loadChildDocument(InputStream stream) {#loadChildDocument-java.io.InputStream-}
```
public void loadChildDocument(InputStream stream)
```


Προσθέτει έναν παιδικό κόμβο εγγράφου. Ανοίγει ένα υπάρχον έγγραφο OneNote από μια ροή.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ροή | java.io.InputStream | Η ροή. |

### loadChildDocument(InputStream stream, LoadOptions loadOptions) {#loadChildDocument-java.io.InputStream-com.aspose.note.LoadOptions-}
```
public void loadChildDocument(InputStream stream, LoadOptions loadOptions)
```


Προσθέτει έναν παιδικό κόμβο εγγράφου. Ανοίγει ένα υπάρχον έγγραφο OneNote από μια ροή. Επιτρέπει τον καθορισμό πρόσθετων επιλογών φόρτωσης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ροή | java.io.InputStream | Η ροή. |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | Οι επιλογές φόρτωσης. |

### loadChildDocument(String filePath) {#loadChildDocument-java.lang.String-}
```
public void loadChildDocument(String filePath)
```


Προσθέτει έναν παιδικό κόμβο εγγράφου. Ανοίγει ένα υπάρχον έγγραφο OneNote από ένα αρχείο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| filePath | java.lang.String | Η διαδρομή του αρχείου. |

### loadChildDocument(String filePath, LoadOptions loadOptions) {#loadChildDocument-java.lang.String-com.aspose.note.LoadOptions-}
```
public void loadChildDocument(String filePath, LoadOptions loadOptions)
```


Προσθέτει έναν παιδικό κόμβο εγγράφου. Ανοίγει ένα υπάρχον έγγραφο OneNote από ένα αρχείο. Επιτρέπει τον καθορισμό πρόσθετων επιλογών φόρτωσης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| filePath | java.lang.String | Η διαδρομή του αρχείου. |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | Οι επιλογές φόρτωσης. |

### loadChildNotebook(String filePath) {#loadChildNotebook-java.lang.String-}
```
public void loadChildNotebook(String filePath)
```


Προσθέτει έναν παιδικό κόμβο σημειωματάριου. Ανοίγει ένα υπάρχον σημειωματάριο OneNote από ένα αρχείο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| filePath | java.lang.String | Η διαδρομή του αρχείου. |

### loadChildNotebook(String filePath, NotebookLoadOptions loadOptions) {#loadChildNotebook-java.lang.String-com.aspose.note.NotebookLoadOptions-}
```
public void loadChildNotebook(String filePath, NotebookLoadOptions loadOptions)
```


Προσθέτει έναν παιδικό κόμβο σημειωματάριου. Ανοίγει ένα υπάρχον σημειωματάριο OneNote από ένα αρχείο. Επιτρέπει τον καθορισμό πρόσθετων επιλογών φόρτωσης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| filePath | java.lang.String | Η διαδρομή του αρχείου. |
| loadOptions | [NotebookLoadOptions](../../com.aspose.note/notebookloadoptions) | Οι επιλογές φόρτωσης. |

### removeChild(INotebookChildNode oldChild) {#removeChild-com.aspose.note.INotebookChildNode-}
```
public INotebookChildNode removeChild(INotebookChildNode oldChild)
```


Αφαιρεί τον κόμβο-παιδί.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| oldChild | [INotebookChildNode](../../com.aspose.note/inotebookchildnode) | Ο κόμβος προς αφαίρεση. |

**Returns:**
[INotebookChildNode](../../com.aspose.note/inotebookchildnode) - The removed node.
### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public void save(OutputStream stream)
```


Αποθηκεύει το έγγραφο OneNote σε μια ροή.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ροή | java.io.OutputStream | Η ροή. |

### save(OutputStream stream, NotebookSaveOptions options) {#save-java.io.OutputStream-com.aspose.note.NotebookSaveOptions-}
```
public void save(OutputStream stream, NotebookSaveOptions options)
```


Αποθηκεύει το έγγραφο OneNote σε μια ροή χρησιμοποιώντας τις καθορισμένες επιλογές αποθήκευσης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ροή | java.io.OutputStream | Η ροή. |
| options | [NotebookSaveOptions](../../com.aspose.note/notebooksaveoptions) | Καθορίζει τις επιλογές για το πώς αποθηκεύεται το έγγραφο. |

### save(OutputStream stream, int format) {#save-java.io.OutputStream-int-}
```
public void save(OutputStream stream, int format)
```


Αποθηκεύει το έγγραφο OneNote σε μια ροή στη καθορισμένη μορφή.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ροή | java.io.OutputStream | Η ροή. |
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

### save(String fileName, NotebookSaveOptions options) {#save-java.lang.String-com.aspose.note.NotebookSaveOptions-}
```
public void save(String fileName, NotebookSaveOptions options)
```


Αποθηκεύει το έγγραφο OneNote σε ένα αρχείο χρησιμοποιώντας τις καθορισμένες επιλογές αποθήκευσης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fileName | java.lang.String | Το πλήρες όνομα του αρχείου. Εάν υπάρχει ήδη αρχείο με το καθορισμένο πλήρες όνομα, το υπάρχον αρχείο θα αντικατασταθεί. |
| options | [NotebookSaveOptions](../../com.aspose.note/notebooksaveoptions) | Καθορίζει τις επιλογές για το πώς αποθηκεύεται το έγγραφο σε αρχείο. |

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

### setColor(Color value) {#setColor-java.awt.Color-}
```
public void setColor(Color value)
```


Λαμβάνει ή ορίζει το χρώμα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.awt.Color |  |

### setDisplayName(String value) {#setDisplayName-java.lang.String-}
```
public void setDisplayName(String value)
```


Λαμβάνει ή ορίζει το όνομα εμφάνισης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String |  |

### setHistoryEnabled(boolean value) {#setHistoryEnabled-boolean-}
```
public void setHistoryEnabled(boolean value)
```


Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει αν το ιστορικό είναι ενεργοποιημένο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean |  |

