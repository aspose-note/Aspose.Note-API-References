---
title: "License"
second_title: "Aspose.Note για Java Αναφορά API"
description: "Παρέχει μεθόδους για την άδεια του στοιχείου."
type: docs
weight: 44
url: /el/java/com.aspose.note/license/
---

**Inheritance:**
java.lang.Object
```
public class License
```

Παρέχει μεθόδους για την άδεια του στοιχείου.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [License()](#License--) | Αρχικοποιεί μια νέα παρουσία αυτής της κλάσης. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [resetThreadContext()](#resetThreadContext--) | Επαναφέρει ένα πλαίσιο άδειας για το τρέχον νήμα. |
| [setLicense(File licenseFile)](#setLicense-java.io.File-) | Παρέχει άδεια στο στοιχείο. |
| [setLicense(InputStream stream)](#setLicense-java.io.InputStream-) | Παρέχει άδεια στο στοιχείο. |
| [setLicense(String licenseName)](#setLicense-java.lang.String-) | Παρέχει άδεια στο στοιχείο. |
| [setThreadContext(InputStream stream)](#setThreadContext-java.io.InputStream-) | Ορίζει ένα πλαίσιο άδειας για το τρέχον νήμα. |
### License() {#License--}
```
public License()
```


Αρχικοποιεί μια νέα παρουσία αυτής της κλάσης.

### resetThreadContext() {#resetThreadContext--}
```
public static void resetThreadContext()
```


Επαναφέρει ένα πλαίσιο άδειας για το τρέχον νήμα.

### setLicense(File licenseFile) {#setLicense-java.io.File-}
```
public void setLicense(File licenseFile)
```


Παρέχει άδεια στο στοιχείο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| licenseFile | java.io.File | Αρχείο άδειας`System.IO.FileInfo`. |

### setLicense(InputStream stream) {#setLicense-java.io.InputStream-}
```
public final void setLicense(InputStream stream)
```


Παρέχει άδεια στο στοιχείο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | ροή | java.io.InputStream | Μία ροή που περιέχει την άδεια. |

--------------------

`

Χρησιμοποιήστε αυτή τη μέθοδο για να φορτώσετε μια άδεια από μια ροή.

`

`void setLicense(java.io.InputStream stream)` |

### setLicense(String licenseName) {#setLicense-java.lang.String-}
```
public final void setLicense(String licenseName)
```


Παρέχει άδεια στο στοιχείο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
|  | licenseName | java.lang.String | Μπορεί να είναι πλήρες ή σύντομο όνομα αρχείου` ή όνομα ενσωματωμένου πόρου`. Χρησιμοποιήστε μια κενή συμβολοσειρά για να μεταβείτε σε λειτουργία αξιολόγησης. |

--------------------

`

Προσπαθεί να βρει την άδεια στις ακόλουθες τοποθεσίες:

` `

1. Ρητή διαδρομή.

` `

2. Ο φάκελος που περιέχει το assembly του συστατικού Aspose.

3. Ο φάκελος που περιέχει το assembly κλήσης του πελάτη.

4. Ο φάκελος που περιέχει το assembly εισόδου (εκκίνησης).

5. Ένας ενσωματωμένος πόρος στο assembly κλήσης του πελάτη.

**Note:**On the .NET Compact Framework, tries to find the license only in these locations:

1. Ρητή διαδρομή.

2. Ένας ενσωματωμένος πόρος στο assembly κλήσης του πελάτη.

` `

2. Ο φάκελος που περιέχει το αρχείο JAR του συστατικού Aspose.

3. Ο φάκελος που περιέχει το αρχείο JAR κλήσης του πελάτη.

` |

### setThreadContext(InputStream stream) {#setThreadContext-java.io.InputStream-}
```
public static void setThreadContext(InputStream stream)
```


Ορίζει ένα πλαίσιο άδειας για το τρέχον νήμα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ροή | java.io.InputStream | Μία ροή που περιέχει την άδεια. |

