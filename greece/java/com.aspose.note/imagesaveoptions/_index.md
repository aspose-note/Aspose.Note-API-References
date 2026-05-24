---
title: "ImageSaveOptions"
second_title: "Aspose.Note για Java Αναφορά API"
description: "Επιτρέπει τον καθορισμό πρόσθετων επιλογών κατά την απόδοση των σελίδων του εγγράφου σε εικόνες."
type: docs
weight: 35
url: /el/java/com.aspose.note/imagesaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.SaveOptions](../../com.aspose.note/saveoptions)
```
public class ImageSaveOptions extends SaveOptions
```

Επιτρέπει τον καθορισμό πρόσθετων επιλογών κατά την απόδοση των σελίδων του εγγράφου σε εικόνες.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [ImageSaveOptions(int format)](#ImageSaveOptions-int-) | Αρχικοποιεί μια νέα παρουσία της κλάσης `ImageSaveOptions`. |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getBinarizationOptions()](#getBinarizationOptions--) | Λαμβάνει ή ορίζει επιλογές για τη δυαδικοποίηση της εικόνας. |
| [getColorMode()](#getColorMode--) | Λαμβάνει ή ορίζει το `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-)) για την εικόνα εξόδου. |
| [getQuality()](#getQuality--) | Λαμβάνει μια τιμή που καθορίζει την ποιότητα της αποθηκευμένης εικόνας. |
| [getResolution()](#getResolution--) | Λαμβάνει την ανάλυση για τις παραγόμενες εικόνες, σε κουκκίδες ανά ίντσα. |
| [getTiffCompression()](#getTiffCompression--) | Λαμβάνει ή ορίζει τον τύπο συμπίεσης που θα χρησιμοποιηθεί κατά την αποθήκευση των παραγόμενων εικόνων σε μορφή TIFF. |
| [setBinarizationOptions(ImageBinarizationOptions value)](#setBinarizationOptions-com.aspose.note.ImageBinarizationOptions-) | Λαμβάνει ή ορίζει επιλογές για τη δυαδικοποίηση της εικόνας. |
| [setColorMode(int value)](#setColorMode-int-) | Λαμβάνει ή ορίζει το `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-)) για την εικόνα εξόδου. |
| [setQuality(int value)](#setQuality-int-) | Ορίζει μια τιμή που καθορίζει την ποιότητα της αποθηκευμένης εικόνας. |
| [setResolution(float value)](#setResolution-float-) | Ορίζει την ανάλυση για τις παραγόμενες εικόνες, σε κουκκίδες ανά ίντσα. |
| [setTiffCompression(int value)](#setTiffCompression-int-) | Λαμβάνει ή ορίζει τον τύπο συμπίεσης που θα χρησιμοποιηθεί κατά την αποθήκευση των παραγόμενων εικόνων σε μορφή TIFF. |
### ImageSaveOptions(int format) {#ImageSaveOptions-int-}
```
public ImageSaveOptions(int format)
```


Αρχικοποιεί μια νέα παρουσία της κλάσης `ImageSaveOptions`.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| format | int | Η μορφή στην οποία αποθηκεύεται το έγγραφο. |

### getBinarizationOptions() {#getBinarizationOptions--}
```
public final ImageBinarizationOptions getBinarizationOptions()
```


Λαμβάνει ή ορίζει επιλογές για τη δυαδικοποίηση της εικόνας.

**Returns:**
[ImageBinarizationOptions](../../com.aspose.note/imagebinarizationoptions)
### getColorMode() {#getColorMode--}
```
public final int getColorMode()
```


Λαμβάνει ή ορίζει το `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-)) για την εικόνα εξόδου.

**Returns:**
int
### getQuality() {#getQuality--}
```
public final int getQuality()
```


Λαμβάνει μια τιμή που καθορίζει την ποιότητα της αποθηκευμένης εικόνας. Αυτή η τιμή περνάει στον κωδικοποιητή ως παράμετρο System.Drawing.Imaging.Encoder.Quality.

--------------------

Το εύρος των χρήσιμων τιμών για την κατηγορία ποιότητας είναι από 0 έως 100. Όσο χαμηλότερος είναι ο καθορισμένος αριθμός, τόσο μεγαλύτερη είναι η συμπίεση και, κατά συνέπεια, τόσο χαμηλότερη η ποιότητα της εικόνας. Το μηδέν θα σας δώσει την χαμηλότερη ποιότητα εικόνας και το 100 τη μέγιστη. Η προεπιλεγμένη τιμή είναι 90.

**Returns:**
int
### getResolution() {#getResolution--}
```
public float getResolution()
```


Λαμβάνει την ανάλυση για τις παραγόμενες εικόνες, σε κουκκίδες ανά ίντσα.

--------------------

Η προεπιλεγμένη τιμή είναι 96.

**Returns:**
float
### getTiffCompression() {#getTiffCompression--}
```
public final int getTiffCompression()
```


Λαμβάνει ή ορίζει τον τύπο συμπίεσης που θα χρησιμοποιηθεί κατά την αποθήκευση των παραγόμενων εικόνων σε μορφή TIFF.

**Returns:**
int
### setBinarizationOptions(ImageBinarizationOptions value) {#setBinarizationOptions-com.aspose.note.ImageBinarizationOptions-}
```
public final void setBinarizationOptions(ImageBinarizationOptions value)
```


Λαμβάνει ή ορίζει επιλογές για τη δυαδικοποίηση της εικόνας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [ImageBinarizationOptions](../../com.aspose.note/imagebinarizationoptions) |  |

### setColorMode(int value) {#setColorMode-int-}
```
public final void setColorMode(int value)
```


Λαμβάνει ή ορίζει το `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-)) για την εικόνα εξόδου.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int |  |

### setQuality(int value) {#setQuality-int-}
```
public final void setQuality(int value)
```


Ορίζει μια τιμή που καθορίζει την ποιότητα της αποθηκευμένης εικόνας. Αυτή η τιμή περνάει στον κωδικοποιητή ως παράμετρο System.Drawing.Imaging.Encoder.Quality.

--------------------

Το εύρος των χρήσιμων τιμών για την κατηγορία ποιότητας είναι από 0 έως 100. Όσο χαμηλότερος είναι ο καθορισμένος αριθμός, τόσο μεγαλύτερη είναι η συμπίεση και, κατά συνέπεια, τόσο χαμηλότερη η ποιότητα της εικόνας. Το μηδέν θα σας δώσει την χαμηλότερη ποιότητα εικόνας και το 100 τη μέγιστη. Η προεπιλεγμένη τιμή είναι 90.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int |  |

### setResolution(float value) {#setResolution-float-}
```
public void setResolution(float value)
```


Ορίζει την ανάλυση για τις παραγόμενες εικόνες, σε κουκκίδες ανά ίντσα.

--------------------

Η προεπιλεγμένη τιμή είναι 90.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | float |  |

### setTiffCompression(int value) {#setTiffCompression-int-}
```
public final void setTiffCompression(int value)
```


Λαμβάνει ή ορίζει τον τύπο συμπίεσης που θα χρησιμοποιηθεί κατά την αποθήκευση των παραγόμενων εικόνων σε μορφή TIFF.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int |  |

