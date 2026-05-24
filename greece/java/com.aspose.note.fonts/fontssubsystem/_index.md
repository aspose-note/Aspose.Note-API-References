---
title: "FontsSubsystem"
second_title: "Aspose.Note για Java Αναφορά API"
description: "Βασική κλάση που υλοποιεί τη διεπαφή com.aspose.note.IFontsSubsystem."
type: docs
weight: 11
url: /el/java/com.aspose.note.fonts/fontssubsystem/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.note.fonts.IFontsSubsystem](../../com.aspose.note.fonts/ifontssubsystem)
```
public abstract class FontsSubsystem implements IFontsSubsystem
```

Βασική κλάση που υλοποιεί τη διεπαφή com.aspose.note.IFontsSubsystem. Παρέχει λειτουργικότητα για την προεπιλεγμένη γραμματοσειρά και τις αντικαταστάσεις γραμματοσειρών. Υπερκαλύψτε τη προστατευμένη μέθοδο com.aspose.note.FontsSubsystem.fetchFontFamily σε μια κληρονομημένη κλάση για να υλοποιήσετε τη λογική ανάκτησης του αντικειμένου Font.
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [addFont(InputStream stream)](#addFont-java.io.InputStream-) | Προσθέτει τη γραμματοσειρά. |
| [addFont(String file)](#addFont-java.lang.String-) | Προσθέτει τη γραμματοσειρά. |
| [addFontSubstitution(String substituted, String substitution)](#addFontSubstitution-java.lang.String-java.lang.String-) | Προσθέτει αντικατάσταση γραμματοσειράς. |
| [getDefaultFont()](#getDefaultFont--) | Λαμβάνει την προεπιλεγμένη γραμματοσειρά. |
| [getFontFamily(String fontName)](#getFontFamily-java.lang.String-) | Λαμβάνει τη γραμματοσειρά. |
| [loadFontsFromFolder(String folder)](#loadFontsFromFolder-java.lang.String-) | Φορτώνει όλες τις γραμματοσειρές TrueType από τον καθορισμένο φάκελο στη εσωτερική συλλογή. |
### addFont(InputStream stream) {#addFont-java.io.InputStream-}
```
public final void addFont(InputStream stream)
```


Προσθέτει τη γραμματοσειρά.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ροή | java.io.InputStream | Η ροή που περιέχει τη γραμματοσειρά. |

### addFont(String file) {#addFont-java.lang.String-}
```
public final void addFont(String file)
```


Προσθέτει τη γραμματοσειρά.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| αρχείο | java.lang.String | Η διαδρομή προς το αρχείο που περιέχει τη γραμματοσειρά. |

### addFontSubstitution(String substituted, String substitution) {#addFontSubstitution-java.lang.String-java.lang.String-}
```
public final void addFontSubstitution(String substituted, String substitution)
```


Προσθέτει αντικατάσταση γραμματοσειράς.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| αντικαταστάτη | java.lang.String | Το όνομα της αντικατασταθείσας γραμματοσειράς. |
| αντικατάσταση | java.lang.String | Το όνομα της γραμματοσειράς αντικατάστασης. |

### getDefaultFont() {#getDefaultFont--}
```
public Font getDefaultFont()
```


Λαμβάνει την προεπιλεγμένη γραμματοσειρά.

**Returns:**
java.awt.Font
### getFontFamily(String fontName) {#getFontFamily-java.lang.String-}
```
public Font getFontFamily(String fontName)
```


Λαμβάνει τη γραμματοσειρά.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fontName | java.lang.String | Το όνομα γραμματοσειράς. |

**Returns:**
java.awt.Font - Η γραμματοσειρά.
### loadFontsFromFolder(String folder) {#loadFontsFromFolder-java.lang.String-}
```
public final void loadFontsFromFolder(String folder)
```


Φορτώνει όλες τις γραμματοσειρές TrueType από τον καθορισμένο φάκελο στη εσωτερική συλλογή.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| φάκελος | java.lang.String | Ο φάκελος που περιέχει γραμματοσειρές. |

