---
title: "DocumentFontsSubsystem"
second_title: "Aspose.Note για Java Αναφορά API"
description: "Απλή υλοποίηση του Aspose.Note.Fonts.FontsSubsystem."
type: docs
weight: 10
url: /el/java/com.aspose.note.fonts/documentfontssubsystem/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.fonts.FontsSubsystem](../../com.aspose.note.fonts/fontssubsystem)
```
public class DocumentFontsSubsystem extends FontsSubsystem
```

Απλή υλοποίηση του Aspose.Note.Fonts.FontsSubsystem. Ανακτά το αντικείμενο FontFamily από το λειτουργικό σύστημα.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [DocumentFontsSubsystem(InputStream defaultFontStream, Map&lt;String,String&gt; fontsSubstitutions)](#DocumentFontsSubsystem-java.io.InputStream-java.util.Map-java.lang.String-java.lang.String--) | Αρχικοποιεί μια νέα παρουσία της κλάσης [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem). |
| [DocumentFontsSubsystem(InputStream defaultFontStream)](#DocumentFontsSubsystem-java.io.InputStream-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem). |
| [DocumentFontsSubsystem(String defaultFontFile, Map&lt;String,String&gt; fontsSubstitutions)](#DocumentFontsSubsystem-java.lang.String-java.util.Map-java.lang.String-java.lang.String--) | Αρχικοποιεί μια νέα παρουσία της κλάσης [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem). |
| [DocumentFontsSubsystem(String defaultFontFile)](#DocumentFontsSubsystem-java.lang.String-) | Αρχικοποιεί μια νέα παρουσία της κλάσης [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem). |
| [DocumentFontsSubsystem(Map&lt;String,String&gt; fontsSubstitutions)](#DocumentFontsSubsystem-java.util.Map-java.lang.String-java.lang.String--) | Αρχικοποιεί μια νέα παρουσία της κλάσης [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem). |
| [DocumentFontsSubsystem()](#DocumentFontsSubsystem--) | Αρχικοποιεί μια νέα παρουσία της κλάσης [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem). |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getDefault()](#getDefault--) | Λαμβάνει ή ορίζει το στατικό προεπιλεγμένο αντικείμενο. |
| [setDefault(DocumentFontsSubsystem value)](#setDefault-com.aspose.note.fonts.DocumentFontsSubsystem-) | Λαμβάνει ή ορίζει το στατικό προεπιλεγμένο αντικείμενο. |
| [usingDefaultFont(String defaultFontName)](#usingDefaultFont-java.lang.String-) | Δημιουργήστε νέο αντικείμενο DocumentFontsSubsystem χρησιμοποιώντας το καθορισμένο προεπιλεγμένο όνομα γραμματοσειράς. |
| [usingDefaultFont(String defaultFontName, Map&lt;String,String&gt; fontsSubstitutions)](#usingDefaultFont-java.lang.String-java.util.Map-java.lang.String-java.lang.String--) | Δημιουργήστε νέο αντικείμενο DocumentFontsSubsystem χρησιμοποιώντας το καθορισμένο προεπιλεγμένο όνομα γραμματοσειράς. |
| [usingDefaultFontFromFile(String filePath)](#usingDefaultFontFromFile-java.lang.String-) | Δημιουργήστε νέο αντικείμενο DocumentFontsSubsystem χρησιμοποιώντας το καθορισμένο προεπιλεγμένο όνομα γραμματοσειράς. |
| [usingDefaultFontFromFile(String filePath, Map&lt;String,String&gt; fontsSubstitutions)](#usingDefaultFontFromFile-java.lang.String-java.util.Map-java.lang.String-java.lang.String--) | Δημιουργήστε νέο αντικείμενο DocumentFontsSubsystem χρησιμοποιώντας μια γραμματοσειρά από το καθορισμένο αρχείο ως προεπιλεγμένη. |
| [usingDefaultFontFromStream(InputStream defaultFontStream)](#usingDefaultFontFromStream-java.io.InputStream-) | Δημιουργήστε νέο αντικείμενο DocumentFontsSubsystem χρησιμοποιώντας μια γραμματοσειρά από το καθορισμένο ρεύμα ως προεπιλεγμένη. |
| [usingDefaultFontFromStream(InputStream defaultFontStream, Map&lt;String,String&gt; fontsSubstitutions)](#usingDefaultFontFromStream-java.io.InputStream-java.util.Map-java.lang.String-java.lang.String--) | Δημιουργήστε νέο αντικείμενο DocumentFontsSubsystem χρησιμοποιώντας μια γραμματοσειρά από το καθορισμένο ρεύμα ως προεπιλεγμένη. |
### DocumentFontsSubsystem(InputStream defaultFontStream, Map&lt;String,String&gt; fontsSubstitutions) {#DocumentFontsSubsystem-java.io.InputStream-java.util.Map-java.lang.String-java.lang.String--}
```
public DocumentFontsSubsystem(InputStream defaultFontStream, Map<String,String> fontsSubstitutions)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| defaultFontStream | java.io.InputStream | Το ρεύμα που περιέχει την προεπιλεγμένη γραμματοσειρά. |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | Οι αντικαταστάσεις γραμματοσειρών. |

### DocumentFontsSubsystem(InputStream defaultFontStream) {#DocumentFontsSubsystem-java.io.InputStream-}
```
public DocumentFontsSubsystem(InputStream defaultFontStream)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| defaultFontStream | java.io.InputStream | Το ρεύμα που περιέχει την προεπιλεγμένη γραμματοσειρά. |

### DocumentFontsSubsystem(String defaultFontFile, Map&lt;String,String&gt; fontsSubstitutions) {#DocumentFontsSubsystem-java.lang.String-java.util.Map-java.lang.String-java.lang.String--}
```
public DocumentFontsSubsystem(String defaultFontFile, Map<String,String> fontsSubstitutions)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| defaultFontFile | java.lang.String | Η διαδρομή προς το αρχείο που περιέχει την προεπιλεγμένη γραμματοσειρά. |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | Οι αντικαταστάσεις γραμματοσειρών. |

### DocumentFontsSubsystem(String defaultFontFile) {#DocumentFontsSubsystem-java.lang.String-}
```
public DocumentFontsSubsystem(String defaultFontFile)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| defaultFontFile | java.lang.String | Η διαδρομή προς το αρχείο που περιέχει την προεπιλεγμένη γραμματοσειρά. |

### DocumentFontsSubsystem(Map&lt;String,String&gt; fontsSubstitutions) {#DocumentFontsSubsystem-java.util.Map-java.lang.String-java.lang.String--}
```
public DocumentFontsSubsystem(Map<String,String> fontsSubstitutions)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | Οι αντικαταστάσεις γραμματοσειρών. |

### DocumentFontsSubsystem() {#DocumentFontsSubsystem--}
```
public DocumentFontsSubsystem()
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).

### getDefault() {#getDefault--}
```
public static DocumentFontsSubsystem getDefault()
```


Λαμβάνει ή ορίζει το στατικό προεπιλεγμένο αντικείμενο.

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem)
### setDefault(DocumentFontsSubsystem value) {#setDefault-com.aspose.note.fonts.DocumentFontsSubsystem-}
```
public static void setDefault(DocumentFontsSubsystem value)
```


Λαμβάνει ή ορίζει το στατικό προεπιλεγμένο αντικείμενο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) |  |

### usingDefaultFont(String defaultFontName) {#usingDefaultFont-java.lang.String-}
```
public static DocumentFontsSubsystem usingDefaultFont(String defaultFontName)
```


Δημιουργήστε νέο αντικείμενο DocumentFontsSubsystem χρησιμοποιώντας το καθορισμένο προεπιλεγμένο όνομα γραμματοσειράς.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| defaultFontName | java.lang.String | Το προεπιλεγμένο όνομα γραμματοσειράς. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFont(String defaultFontName, Map&lt;String,String&gt; fontsSubstitutions) {#usingDefaultFont-java.lang.String-java.util.Map-java.lang.String-java.lang.String--}
```
public static DocumentFontsSubsystem usingDefaultFont(String defaultFontName, Map<String,String> fontsSubstitutions)
```


Δημιουργήστε νέο αντικείμενο DocumentFontsSubsystem χρησιμοποιώντας το καθορισμένο προεπιλεγμένο όνομα γραμματοσειράς.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| defaultFontName | java.lang.String | Το προεπιλεγμένο όνομα γραμματοσειράς. |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | Οι αντικαταστάσεις γραμματοσειρών. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFontFromFile(String filePath) {#usingDefaultFontFromFile-java.lang.String-}
```
public static DocumentFontsSubsystem usingDefaultFontFromFile(String filePath)
```


Δημιουργήστε νέο αντικείμενο DocumentFontsSubsystem χρησιμοποιώντας το καθορισμένο προεπιλεγμένο όνομα γραμματοσειράς.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| filePath | java.lang.String | Το αρχείο που περιέχει το προεπιλεγμένο όνομα γραμματοσειράς. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFontFromFile(String filePath, Map&lt;String,String&gt; fontsSubstitutions) {#usingDefaultFontFromFile-java.lang.String-java.util.Map-java.lang.String-java.lang.String--}
```
public static DocumentFontsSubsystem usingDefaultFontFromFile(String filePath, Map<String,String> fontsSubstitutions)
```


Δημιουργήστε νέο αντικείμενο DocumentFontsSubsystem χρησιμοποιώντας μια γραμματοσειρά από το καθορισμένο αρχείο ως προεπιλεγμένη.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| filePath | java.lang.String | Το αρχείο που περιέχει το προεπιλεγμένο όνομα γραμματοσειράς. |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | Οι αντικαταστάσεις γραμματοσειρών. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFontFromStream(InputStream defaultFontStream) {#usingDefaultFontFromStream-java.io.InputStream-}
```
public static DocumentFontsSubsystem usingDefaultFontFromStream(InputStream defaultFontStream)
```


Δημιουργήστε νέο αντικείμενο DocumentFontsSubsystem χρησιμοποιώντας μια γραμματοσειρά από το καθορισμένο ρεύμα ως προεπιλεγμένη.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| defaultFontStream | java.io.InputStream | Το ρεύμα που περιέχει το προεπιλεγμένο όνομα γραμματοσειράς. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFontFromStream(InputStream defaultFontStream, Map&lt;String,String&gt; fontsSubstitutions) {#usingDefaultFontFromStream-java.io.InputStream-java.util.Map-java.lang.String-java.lang.String--}
```
public static DocumentFontsSubsystem usingDefaultFontFromStream(InputStream defaultFontStream, Map<String,String> fontsSubstitutions)
```


Δημιουργήστε νέο αντικείμενο DocumentFontsSubsystem χρησιμοποιώντας μια γραμματοσειρά από το καθορισμένο ρεύμα ως προεπιλεγμένη.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| defaultFontStream | java.io.InputStream | Το ρεύμα που περιέχει το προεπιλεγμένο όνομα γραμματοσειράς. |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | Οι αντικαταστάσεις γραμματοσειρών. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
