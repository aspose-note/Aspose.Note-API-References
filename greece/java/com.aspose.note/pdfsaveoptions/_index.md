---
title: "PdfSaveOptions"
second_title: "Aspose.Note για Java Αναφορά API"
description: "Επιτρέπει τον καθορισμό πρόσθετων επιλογών κατά την απόδοση των σελίδων του εγγράφου σε PDF."
type: docs
weight: 77
url: /el/java/com.aspose.note/pdfsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.SaveOptions](../../com.aspose.note/saveoptions)
```
public final class PdfSaveOptions extends SaveOptions
```

Επιτρέπει τον καθορισμό πρόσθετων επιλογών κατά την απόδοση των σελίδων του εγγράφου σε PDF.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [PdfSaveOptions()](#PdfSaveOptions--) | Αρχικοποιεί μια νέα παρουσία της κλάσης `PdfSaveOptions`. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getImageCompression()](#getImageCompression--) | Λαμβάνει τον τύπο συμπίεσης που εφαρμόζεται στις εικόνες του αρχείου PDF. |
| [getJpegQuality()](#getJpegQuality--) | Λαμβάνει μια τιμή που καθορίζει την ποιότητα των εικόνων JPEG μέσα στο έγγραφο PDF. |
| [getPageSettings()](#getPageSettings--) | Λαμβάνει ή ορίζει τις ρυθμίσεις σελίδας για κάθε σελίδα στο έγγραφο. |
| [getPageSplittingAlgorithm()](#getPageSplittingAlgorithm--) | Λαμβάνει ή ορίζει τον αλγόριθμο που χρησιμοποιείται για το διαχωρισμό σελίδων. |
| [setImageCompression(int value)](#setImageCompression-int-) | Ορίζει τον τύπο συμπίεσης που εφαρμόζεται στις εικόνες του αρχείου PDF. |
| [setJpegQuality(int value)](#setJpegQuality-int-) | Ορίζει μια τιμή που καθορίζει την ποιότητα των εικόνων JPEG μέσα στο έγγραφο PDF. |
| [setPageSettings(PageSettings value)](#setPageSettings-com.aspose.note.PageSettings-) | Λαμβάνει ή ορίζει τις ρυθμίσεις σελίδας για κάθε σελίδα στο έγγραφο. |
| [setPageSplittingAlgorithm(PageSplittingAlgorithm value)](#setPageSplittingAlgorithm-com.aspose.note.PageSplittingAlgorithm-) | Λαμβάνει ή ορίζει τον αλγόριθμο που χρησιμοποιείται για το διαχωρισμό σελίδων. |
### PdfSaveOptions() {#PdfSaveOptions--}
```
public PdfSaveOptions()
```


Αρχικοποιεί μια νέα παρουσία της κλάσης `PdfSaveOptions`.

### getImageCompression() {#getImageCompression--}
```
public final int getImageCompression()
```


Λαμβάνει τον τύπο συμπίεσης που εφαρμόζεται στις εικόνες του αρχείου PDF.

**Returns:**
int
### getJpegQuality() {#getJpegQuality--}
```
public final int getJpegQuality()
```


Λαμβάνει μια τιμή που καθορίζει την ποιότητα των εικόνων JPEG μέσα στο έγγραφο PDF. Η τιμή μπορεί να κυμαίνεται από 0 έως 100, όπου το 0 σημαίνει τη χειρότερη ποιότητα αλλά μέγιστη συμπίεση και το 100 σημαίνει την καλύτερη ποιότητα αλλά ελάχιστη συμπίεση.

--------------------

Η προεπιλεγμένη τιμή είναι 90.

**Returns:**
int
### getPageSettings() {#getPageSettings--}
```
public PageSettings getPageSettings()
```


Λαμβάνει ή ορίζει τις ρυθμίσεις σελίδας για κάθε σελίδα στο έγγραφο. Από προεπιλογή εξαρτάται από το CurrentUICulture, \\*US πολιτισμοί έχουν ρύθμιση letter, άλλοι έχουν ρυθμίσεις A4.

**Returns:**
[PageSettings](../../com.aspose.note/pagesettings)
### getPageSplittingAlgorithm() {#getPageSplittingAlgorithm--}
```
public PageSplittingAlgorithm getPageSplittingAlgorithm()
```


Λαμβάνει ή ορίζει τον αλγόριθμο που χρησιμοποιείται για το διαχωρισμό σελίδων.

Τιμή: Το `PageSplittingAlgorithm`.

**Returns:**
[PageSplittingAlgorithm](../../com.aspose.note/pagesplittingalgorithm)
### setImageCompression(int value) {#setImageCompression-int-}
```
public final void setImageCompression(int value)
```


Ορίζει τον τύπο συμπίεσης που εφαρμόζεται στις εικόνες του αρχείου PDF.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int |  |

### setJpegQuality(int value) {#setJpegQuality-int-}
```
public final void setJpegQuality(int value)
```


Ορίζει μια τιμή που καθορίζει την ποιότητα των εικόνων JPEG μέσα στο έγγραφο PDF. Η τιμή μπορεί να κυμαίνεται από 0 έως 100, όπου το 0 σημαίνει τη χειρότερη ποιότητα αλλά μέγιστη συμπίεση και το 100 σημαίνει την καλύτερη ποιότητα αλλά ελάχιστη συμπίεση.

--------------------

Η προεπιλεγμένη τιμή είναι 90.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int |  |

### setPageSettings(PageSettings value) {#setPageSettings-com.aspose.note.PageSettings-}
```
public void setPageSettings(PageSettings value)
```


Λαμβάνει ή ορίζει τις ρυθμίσεις σελίδας για κάθε σελίδα στο έγγραφο. Από προεπιλογή εξαρτάται από το CurrentUICulture, \\*US πολιτισμοί έχουν ρύθμιση letter, άλλοι έχουν ρυθμίσεις A4.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [PageSettings](../../com.aspose.note/pagesettings) |  |

### setPageSplittingAlgorithm(PageSplittingAlgorithm value) {#setPageSplittingAlgorithm-com.aspose.note.PageSplittingAlgorithm-}
```
public void setPageSplittingAlgorithm(PageSplittingAlgorithm value)
```


Λαμβάνει ή ορίζει τον αλγόριθμο που χρησιμοποιείται για το διαχωρισμό σελίδων.

Τιμή: Το `PageSplittingAlgorithm`.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [PageSplittingAlgorithm](../../com.aspose.note/pagesplittingalgorithm) |  |

