---
title: "DocumentPrintAttributeSet"
second_title: "Aspose.Note για Java Αναφορά API"
description: "Αναπαριστά βοηθητική κλάση με φιλική προς το χρήστη διεπαφή για το AttributeSet."
type: docs
weight: 21
url: /el/java/com.aspose.note/documentprintattributeset/
---

**Inheritance:**
java.lang.Object, javax.print.attribute.HashAttributeSet
```
public final class DocumentPrintAttributeSet extends HashAttributeSet
```

Αναπαριστά βοηθητική κλάση με φιλική προς το χρήστη διεπαφή για το AttributeSet.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [DocumentPrintAttributeSet(int copies)](#DocumentPrintAttributeSet-int-) | Δημιουργεί μια νέα παρουσία του `DocumentPrintAttributeSet`. |
| [DocumentPrintAttributeSet(String printerName, int copies)](#DocumentPrintAttributeSet-java.lang.String-int-) | Δημιουργεί μια νέα παρουσία του `DocumentPrintAttributeSet`. |
| [DocumentPrintAttributeSet(String printerName)](#DocumentPrintAttributeSet-java.lang.String-) | Δημιουργεί μια νέα παρουσία του `DocumentPrintAttributeSet`. |
| [DocumentPrintAttributeSet()](#DocumentPrintAttributeSet--) | Δημιουργεί μια νέα παρουσία του `DocumentPrintAttributeSet`. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getCopies()](#getCopies--) |  |
| [getLandscape()](#getLandscape--) |  |
| [getPrinterName()](#getPrinterName--) |  |
| [setCollate(boolean value)](#setCollate-boolean-) | Ορίζει μια τιμή που υποδεικνύει εάν το έγγραφο είναι συγκεντρωμένο. |
| [setCopies(int value)](#setCopies-int-) | Ορίζει τον αριθμό των αντιτύπων που θα εκτυπωθούν. |
| [setDuplex(boolean value)](#setDuplex-boolean-) | Ορίζει τη ρύθμιση του εκτυπωτή για εκτύπωση διπλής όψης. |
| [setLandscape(boolean value)](#setLandscape-boolean-) | Ορίζει τον προσανατολισμό της σελίδας. |
| [setPrintRange(int page)](#setPrintRange-int-) | Ορίζει τη μεμονωμένη σελίδα που θα εκτυπωθεί. |
| [setPrintRange(int from, int to)](#setPrintRange-int-int-) | Ορίζει το εύρος σελίδων που θα εκτυπωθεί. |
| [setPrinterName(String printerName)](#setPrinterName-java.lang.String-) | Το όνομα του εκτυπωτή που θα χρησιμοποιηθεί. |
| [setPrinterName(String printerName, Locale locale)](#setPrinterName-java.lang.String-java.util.Locale-) | Το όνομα του εκτυπωτή που θα χρησιμοποιηθεί. |
### DocumentPrintAttributeSet(int copies) {#DocumentPrintAttributeSet-int-}
```
public DocumentPrintAttributeSet(int copies)
```


Δημιουργεί μια νέα παρουσία του `DocumentPrintAttributeSet`. Από προεπιλογή εκτυπώνονται όλες οι σελίδες του εγγράφου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| αντίτυπα | int | Ο αριθμός των αντιτύπων του εγγράφου που θα εκτυπωθούν. |

### DocumentPrintAttributeSet(String printerName, int copies) {#DocumentPrintAttributeSet-java.lang.String-int-}
```
public DocumentPrintAttributeSet(String printerName, int copies)
```


Δημιουργεί μια νέα παρουσία του `DocumentPrintAttributeSet`. Από προεπιλογή εκτυπώνονται όλες οι σελίδες του εγγράφου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| printerName | java.lang.String | Το όνομα του εκτυπωτή. |
| αντίτυπα | int | Ο αριθμός των αντιτύπων του εγγράφου που θα εκτυπωθούν. |

### DocumentPrintAttributeSet(String printerName) {#DocumentPrintAttributeSet-java.lang.String-}
```
public DocumentPrintAttributeSet(String printerName)
```


Δημιουργεί μια νέα παρουσία του `DocumentPrintAttributeSet`. Από προεπιλογή είναι το μόνο αντίτυπο κάθε σελίδας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| printerName | java.lang.String | Το όνομα του εκτυπωτή. |

### DocumentPrintAttributeSet() {#DocumentPrintAttributeSet--}
```
public DocumentPrintAttributeSet()
```


Δημιουργεί μια νέα παρουσία του `DocumentPrintAttributeSet`. Από προεπιλογή είναι το μόνο αντίτυπο κάθε σελίδας.

### getCopies() {#getCopies--}
```
public int getCopies()
```




**Returns:**
int
### getLandscape() {#getLandscape--}
```
public boolean getLandscape()
```




**Returns:**
boolean
### getPrinterName() {#getPrinterName--}
```
public String getPrinterName()
```




**Returns:**
java.lang.String
### setCollate(boolean value) {#setCollate-boolean-}
```
public void setCollate(boolean value)
```


Ορίζει μια τιμή που υποδεικνύει εάν το έγγραφο είναι συγκεντρωμένο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | true είναι ισοδύναμο με τη ρύθμιση SheetCollate.COLLATED false είναι ισοδύναμο με τη ρύθμιση SheetCollate.UNCOLLATED |

### setCopies(int value) {#setCopies-int-}
```
public void setCopies(int value)
```


Ορίζει τον αριθμό των αντιτύπων που θα εκτυπωθούν.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int | Ο αριθμός των αντιτύπων που θα εκτυπωθούν. |

### setDuplex(boolean value) {#setDuplex-boolean-}
```
public void setDuplex(boolean value)
```


Ορίζει τη ρύθμιση του εκτυπωτή για εκτύπωση διπλής όψης.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | true είναι ισοδύναμο με τη ρύθμιση Sides.DUPLEX false είναι ισοδύναμο με τη ρύθμιση Sides.ONE\_SIDED |

### setLandscape(boolean value) {#setLandscape-boolean-}
```
public void setLandscape(boolean value)
```


Ορίζει τον προσανατολισμό της σελίδας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean | true είναι ισοδύναμο με τη ρύθμιση OrientationRequested.LANDSCAPE false είναι ισοδύναμο με τη ρύθμιση OrientationRequested.PORTRAIT |

### setPrintRange(int page) {#setPrintRange-int-}
```
public void setPrintRange(int page)
```


Ορίζει τη μεμονωμένη σελίδα που θα εκτυπωθεί.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| σελίδα | int | Η σελίδα που θα εκτυπωθεί. |

### setPrintRange(int from, int to) {#setPrintRange-int-int-}
```
public void setPrintRange(int from, int to)
```


Ορίζει το εύρος σελίδων που θα εκτυπωθεί.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| από | int | Η πρώτη σελίδα. |
| προς | int | Η τελευταία σελίδα. |

### setPrinterName(String printerName) {#setPrinterName-java.lang.String-}
```
public void setPrinterName(String printerName)
```


Το όνομα του εκτυπωτή που θα χρησιμοποιηθεί.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| printerName | java.lang.String | Το όνομα του εκτυπωτή. |

### setPrinterName(String printerName, Locale locale) {#setPrinterName-java.lang.String-java.util.Locale-}
```
public void setPrinterName(String printerName, Locale locale)
```


Το όνομα του εκτυπωτή που θα χρησιμοποιηθεί.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| printerName | java.lang.String | Το όνομα του εκτυπωτή. |
| τοπική ρύθμιση | java.util.Locale | Η τοπική ρύθμιση του printerName. |

