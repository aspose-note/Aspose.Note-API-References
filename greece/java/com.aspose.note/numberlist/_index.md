---
title: "NumberList"
second_title: "Aspose.Note για Java Αναφορά API"
description: "Αντιπροσωπεύει τη αριθμημένη ή κουκίδωση λίστα."
type: docs
weight: 64
url: /el/java/com.aspose.note/numberlist/
---

**Inheritance:**
java.lang.Object
```
public class NumberList
```

Αντιπροσωπεύει τη αριθμημένη ή κουκίδωση λίστα.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [NumberList(String bulletedSymbol, String font, int fontSize)](#NumberList-java.lang.String-java.lang.String-int-) | Αρχικοποιεί ένα νέο παράδειγμα της κλάσης `NumberList`. |
| [NumberList(String format, byte numberFormat, String font, int fontSize)](#NumberList-java.lang.String-byte-java.lang.String-int-) | Αρχικοποιεί ένα νέο παράδειγμα της κλάσης `NumberList`. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [equals(NumberList other)](#equals-com.aspose.note.NumberList-) | Καθορίζει εάν το καθορισμένο αντικείμενο είναι ίσο με το τρέχον αντικείμενο. |
| [equals(Object obj)](#equals-java.lang.Object-) | Καθορίζει εάν το καθορισμένο αντικείμενο είναι ίσο με το τρέχον αντικείμενο. |
| [getFont()](#getFont--) | Λαμβάνει ή ορίζει το όνομα της γραμματοσειράς. |
| [getFontColor()](#getFontColor--) | Λαμβάνει ή ορίζει το χρώμα γραμματοσειράς. |
| [getFontSize()](#getFontSize--) | Λαμβάνει ή ορίζει το μέγεθος γραμματοσειράς. |
| [getFormat()](#getFormat--) | Λαμβάνει ή ορίζει τη μορφή της κεφαλίδας γραμμής. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Λαμβάνει ή ορίζει την τελευταία τροποποιημένη ώρα. |
| [getNumberFormat()](#getNumberFormat--) | Λαμβάνει ή ορίζει τη μορφή αριθμού που χρησιμοποιείται για μια ομάδα αυτόματα αριθμημένων αντικειμένων. |
| [getNumberedListHeader(int sequenceNumber)](#getNumberedListHeader-int-) | Λαμβάνει την κεφαλίδα της αριθμημένης λίστας. |
| [getRestart()](#getRestart--) | Λαμβάνει ή ορίζει την αριθμητική τιμή που αντικαθιστά την αυτόματη αριθμητική τιμή του στοιχείου λίστας. |
| [hashCode()](#hashCode--) | Λειτουργεί ως συνάρτηση κατακερματισμού για τον τύπο. |
| [isBold()](#isBold--) | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει αν το στυλ κειμένου είναι έντονο. |
| [isItalic()](#isItalic--) | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει αν το στυλ κειμένου είναι πλάγιο. |
| [setBold(boolean value)](#setBold-boolean-) | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει αν το στυλ κειμένου είναι έντονο. |
| [setFont(String value)](#setFont-java.lang.String-) | Λαμβάνει ή ορίζει το όνομα της γραμματοσειράς. |
| [setFontColor(Color value)](#setFontColor-java.awt.Color-) | Λαμβάνει ή ορίζει το χρώμα γραμματοσειράς. |
| [setFontSize(int value)](#setFontSize-int-) | Λαμβάνει ή ορίζει το μέγεθος γραμματοσειράς. |
| [setFormat(String value)](#setFormat-java.lang.String-) | Λαμβάνει ή ορίζει τη μορφή της κεφαλίδας γραμμής. |
| [setItalic(boolean value)](#setItalic-boolean-) | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει αν το στυλ κειμένου είναι πλάγιο. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Λαμβάνει ή ορίζει την τελευταία τροποποιημένη ώρα. |
| [setNumberFormat(Byte value)](#setNumberFormat-java.lang.Byte-) | Λαμβάνει ή ορίζει τη μορφή αριθμού που χρησιμοποιείται για μια ομάδα αυτόματα αριθμημένων αντικειμένων. |
| [setRestart(int value)](#setRestart-int-) | Λαμβάνει ή ορίζει την αριθμητική τιμή που αντικαθιστά την αυτόματη αριθμητική τιμή του στοιχείου λίστας. |
### NumberList(String bulletedSymbol, String font, int fontSize) {#NumberList-java.lang.String-java.lang.String-int-}
```
public NumberList(String bulletedSymbol, String font, int fontSize)
```


Αρχικοποιεί ένα νέο παράδειγμα της κλάσης `NumberList`. Αυτό το παράδειγμα αντιπροσωπεύει μια λίστα με κουκκίδες.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| bulletedSymbol | java.lang.String | Ένα σύμβολο που αντιπροσωπεύει μια κουκκίδα. |
| font | java.lang.String | Μια γραμματοσειρά για την κουκκίδα. |
| fontSize | int | Μέγεθος γραμματοσειράς για την κουκκίδα. |

### NumberList(String format, byte numberFormat, String font, int fontSize) {#NumberList-java.lang.String-byte-java.lang.String-int-}
```
public NumberList(String format, byte numberFormat, String font, int fontSize)
```


Αρχικοποιεί ένα νέο παράδειγμα της κλάσης `NumberList`. Αυτό το παράδειγμα αντιπροσωπεύει μια αριθμημένη λίστα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| format | java.lang.String | Η μορφή της αριθμημένης κεφαλίδας. |
| numberFormat | byte | Η μορφή του αριθμού στην κεφαλίδα. |
| font | java.lang.String | Μια γραμματοσειρά για την αριθμημένη κεφαλίδα. |
| fontSize | int | Μέγεθος γραμματοσειράς για την αριθμημένη κεφαλίδα. |

### equals(NumberList other) {#equals-com.aspose.note.NumberList-}
```
public boolean equals(NumberList other)
```


Καθορίζει εάν το καθορισμένο αντικείμενο είναι ίσο με το τρέχον αντικείμενο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| other | [NumberList](../../com.aspose.note/numberlist) | Το αντικείμενο. |

**Returns:**
boolean - Το `bool`.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Καθορίζει εάν το καθορισμένο αντικείμενο είναι ίσο με το τρέχον αντικείμενο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| obj | java.lang.Object | Το αντικείμενο. |

**Returns:**
boolean - Το `bool`.
### getFont() {#getFont--}
```
public String getFont()
```


Λαμβάνει ή ορίζει το όνομα της γραμματοσειράς.

**Returns:**
java.lang.String
### getFontColor() {#getFontColor--}
```
public Color getFontColor()
```


Λαμβάνει ή ορίζει το χρώμα γραμματοσειράς.

**Returns:**
java.awt.Color
### getFontSize() {#getFontSize--}
```
public int getFontSize()
```


Λαμβάνει ή ορίζει το μέγεθος γραμματοσειράς.

**Returns:**
int
### getFormat() {#getFormat--}
```
public String getFormat()
```


Λαμβάνει ή ορίζει τη μορφή της κεφαλίδας γραμμής. Για λίστες με κουκκίδες αντιπροσωπεύει ένα σύμβολο κουκκίδας.

**Returns:**
java.lang.String
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Λαμβάνει ή ορίζει την τελευταία τροποποιημένη ώρα.

**Returns:**
java.util.Date
### getNumberFormat() {#getNumberFormat--}
```
public Byte getNumberFormat()
```


Λαμβάνει ή ορίζει τη μορφή αριθμού που χρησιμοποιείται για μια ομάδα αυτόματα αριθμημένων αντικειμένων. Θα πρέπει να είναι null για λίστες με κουκκίδες.

**Returns:**
java.lang.Byte
### getNumberedListHeader(int sequenceNumber) {#getNumberedListHeader-int-}
```
public String getNumberedListHeader(int sequenceNumber)
```


Λαμβάνει την κεφαλίδα της αριθμημένης λίστας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| sequenceNumber | int | Ο αριθμός ακολουθίας στη αριθμημένη λίστα. |

**Returns:**
java.lang.String - Μια αναπαράσταση συμβολοσειράς του καθορισμένου αριθμού ακολουθίας.
### getRestart() {#getRestart--}
```
public int getRestart()
```


Λαμβάνει ή ορίζει την αριθμητική τιμή που αντικαθιστά την αυτόματη αριθμητική τιμή του στοιχείου λίστας.

**Returns:**
int
### hashCode() {#hashCode--}
```
public int hashCode()
```


Λειτουργεί ως συνάρτηση κατακερματισμού για τον τύπο.

**Returns:**
int - Το `int`.
### isBold() {#isBold--}
```
public boolean isBold()
```


Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει αν το στυλ κειμένου είναι έντονο.

**Returns:**
boolean
### isItalic() {#isItalic--}
```
public boolean isItalic()
```


Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει αν το στυλ κειμένου είναι πλάγιο.

**Returns:**
boolean
### setBold(boolean value) {#setBold-boolean-}
```
public void setBold(boolean value)
```


Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει αν το στυλ κειμένου είναι έντονο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean |  |

### setFont(String value) {#setFont-java.lang.String-}
```
public void setFont(String value)
```


Λαμβάνει ή ορίζει το όνομα της γραμματοσειράς.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String |  |

### setFontColor(Color value) {#setFontColor-java.awt.Color-}
```
public void setFontColor(Color value)
```


Λαμβάνει ή ορίζει το χρώμα γραμματοσειράς.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.awt.Color |  |

### setFontSize(int value) {#setFontSize-int-}
```
public void setFontSize(int value)
```


Λαμβάνει ή ορίζει το μέγεθος γραμματοσειράς.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int |  |

### setFormat(String value) {#setFormat-java.lang.String-}
```
public void setFormat(String value)
```


Λαμβάνει ή ορίζει τη μορφή της κεφαλίδας γραμμής. Για λίστες με κουκκίδες αντιπροσωπεύει ένα σύμβολο κουκκίδας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.String |  |

### setItalic(boolean value) {#setItalic-boolean-}
```
public void setItalic(boolean value)
```


Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει αν το στυλ κειμένου είναι πλάγιο.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Λαμβάνει ή ορίζει την τελευταία τροποποιημένη ώρα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.util.Date |  |

### setNumberFormat(Byte value) {#setNumberFormat-java.lang.Byte-}
```
public void setNumberFormat(Byte value)
```


Λαμβάνει ή ορίζει τη μορφή αριθμού που χρησιμοποιείται για μια ομάδα αυτόματα αριθμημένων αντικειμένων. Θα πρέπει να είναι null για λίστες με κουκκίδες.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | java.lang.Byte |  |

### setRestart(int value) {#setRestart-int-}
```
public void setRestart(int value)
```


Λαμβάνει ή ορίζει την αριθμητική τιμή που αντικαθιστά την αυτόματη αριθμητική τιμή του στοιχείου λίστας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int |  |

