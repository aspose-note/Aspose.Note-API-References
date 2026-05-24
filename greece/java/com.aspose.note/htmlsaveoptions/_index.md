---
title: "HtmlSaveOptions"
second_title: "Aspose.Note για Java Αναφορά API"
description: "Επιτρέπει τον καθορισμό πρόσθετων επιλογών κατά την αποθήκευση του εγγράφου σε μορφή HTML."
type: docs
weight: 32
url: /el/java/com.aspose.note/htmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.SaveOptions](../../com.aspose.note/saveoptions)
```
public class HtmlSaveOptions extends SaveOptions
```

Επιτρέπει τον καθορισμό πρόσθετων επιλογών κατά την αποθήκευση του εγγράφου σε μορφή HTML.
## Κατασκευαστές

| Κατασκευαστής | Περιγραφή |
| --- | --- |
| [HtmlSaveOptions()](#HtmlSaveOptions--) | Αρχικοποιεί μια νέα παρουσία της κλάσης [HtmlSaveOptions](../../com.aspose.note/htmlsaveoptions). |
## Μέθοδοι

| Μέθοδος | Περιγραφή |
| --- | --- |
| [getCssPerPageGeneration()](#getCssPerPageGeneration--) | Λαμβάνει ή ορίζει αν το αρχείο StyleSheet θα δημιουργείται ξεχωριστά για κάθε νέα σελίδα. |
| [getCssSavingCallback()](#getCssSavingCallback--) | Λαμβάνει ή ορίζει την κλήση επιστροφής που καλείται για τη δημιουργία πόρου αποθήκευσης του CSS. |
| [getDocumentPerPageGeneration()](#getDocumentPerPageGeneration--) | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει αν η δημιουργία εγγράφου ανά σελίδα είναι ενεργοποιημένη. |
| [getExportCss()](#getExportCss--) | Λαμβάνει ή ορίζει τον τρόπο εξαγωγής του css. |
| [getExportFonts()](#getExportFonts--) | Λαμβάνει ή ορίζει τον τρόπο εξαγωγής των γραμματοσειρών. |
| [getExportImages()](#getExportImages--) | Λαμβάνει ή ορίζει τον τρόπο εξαγωγής των εικόνων. |
| [getFontFaceTypes()](#getFontFaceTypes--) | Λαμβάνει ή ορίζει τους τύπους γραμματοσειρών. |
| [getFontSavingCallback()](#getFontSavingCallback--) | Λαμβάνει ή ορίζει την κλήση επιστροφής που καλείται για τη δημιουργία πόρου αποθήκευσης της γραμματοσειράς. |
| [getImageSavingCallback()](#getImageSavingCallback--) | Λαμβάνει ή ορίζει την κλήση επιστροφής που καλείται για τη δημιουργία πόρου αποθήκευσης της εικόνας. |
| [getPageSavingCallback()](#getPageSavingCallback--) | Λαμβάνει ή ορίζει την κλήση επιστροφής που καλείται για τη δημιουργία πόρου αποθήκευσης της σελίδας. |
| [setCssPerPageGeneration(boolean value)](#setCssPerPageGeneration-boolean-) | Λαμβάνει ή ορίζει αν το αρχείο StyleSheet θα δημιουργείται ξεχωριστά για κάθε νέα σελίδα. |
| [setCssSavingCallback(ICssSavingCallback value)](#setCssSavingCallback-com.aspose.note.ICssSavingCallback-) | Λαμβάνει ή ορίζει την κλήση επιστροφής που καλείται για τη δημιουργία πόρου αποθήκευσης του CSS. |
| [setDocumentPerPageGeneration(boolean value)](#setDocumentPerPageGeneration-boolean-) | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει αν η δημιουργία εγγράφου ανά σελίδα είναι ενεργοποιημένη. |
| [setExportCss(int value)](#setExportCss-int-) | Λαμβάνει ή ορίζει τον τρόπο εξαγωγής του css. |
| [setExportFonts(int value)](#setExportFonts-int-) | Λαμβάνει ή ορίζει τον τρόπο εξαγωγής των γραμματοσειρών. |
| [setExportImages(int value)](#setExportImages-int-) | Λαμβάνει ή ορίζει τον τρόπο εξαγωγής των εικόνων. |
| [setFontFaceTypes(int value)](#setFontFaceTypes-int-) | Λαμβάνει ή ορίζει τους τύπους γραμματοσειρών. |
| [setFontSavingCallback(IFontSavingCallback value)](#setFontSavingCallback-com.aspose.note.IFontSavingCallback-) | Λαμβάνει ή ορίζει την κλήση επιστροφής που καλείται για τη δημιουργία πόρου αποθήκευσης της γραμματοσειράς. |
| [setImageSavingCallback(IImageSavingCallback value)](#setImageSavingCallback-com.aspose.note.IImageSavingCallback-) | Λαμβάνει ή ορίζει την κλήση επιστροφής που καλείται για τη δημιουργία πόρου αποθήκευσης της εικόνας. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.note.IPageSavingCallback-) | Λαμβάνει ή ορίζει την κλήση επιστροφής που καλείται για τη δημιουργία πόρου αποθήκευσης της σελίδας. |
### HtmlSaveOptions() {#HtmlSaveOptions--}
```
public HtmlSaveOptions()
```


Αρχικοποιεί μια νέα παρουσία της κλάσης [HtmlSaveOptions](../../com.aspose.note/htmlsaveoptions).

### getCssPerPageGeneration() {#getCssPerPageGeneration--}
```
public final boolean getCssPerPageGeneration()
```


Λαμβάνει ή ορίζει αν το αρχείο StyleSheet θα δημιουργείται ξεχωριστά για κάθε νέα σελίδα.

**Returns:**
boolean
### getCssSavingCallback() {#getCssSavingCallback--}
```
public final ICssSavingCallback getCssSavingCallback()
```


Λαμβάνει ή ορίζει την κλήση επιστροφής που καλείται για τη δημιουργία πόρου αποθήκευσης του CSS.

**Returns:**
[ICssSavingCallback](../../com.aspose.note/icsssavingcallback)
### getDocumentPerPageGeneration() {#getDocumentPerPageGeneration--}
```
public final boolean getDocumentPerPageGeneration()
```


Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει αν η δημιουργία εγγράφου ανά σελίδα είναι ενεργοποιημένη.

**Returns:**
boolean
### getExportCss() {#getExportCss--}
```
public final int getExportCss()
```


Λαμβάνει ή ορίζει τον τρόπο εξαγωγής του css.

**Returns:**
int
### getExportFonts() {#getExportFonts--}
```
public final int getExportFonts()
```


Λαμβάνει ή ορίζει τον τρόπο εξαγωγής των γραμματοσειρών.

**Returns:**
int
### getExportImages() {#getExportImages--}
```
public final int getExportImages()
```


Λαμβάνει ή ορίζει τον τρόπο εξαγωγής των εικόνων.

**Returns:**
int
### getFontFaceTypes() {#getFontFaceTypes--}
```
public final int getFontFaceTypes()
```


Λαμβάνει ή ορίζει τους τύπους γραμματοσειρών.

Τιμή: Οι τύποι γραμματοσειρών.

**Returns:**
int
### getFontSavingCallback() {#getFontSavingCallback--}
```
public final IFontSavingCallback getFontSavingCallback()
```


Λαμβάνει ή ορίζει την κλήση επιστροφής που καλείται για τη δημιουργία πόρου αποθήκευσης της γραμματοσειράς.

**Returns:**
[IFontSavingCallback](../../com.aspose.note/ifontsavingcallback)
### getImageSavingCallback() {#getImageSavingCallback--}
```
public final IImageSavingCallback getImageSavingCallback()
```


Λαμβάνει ή ορίζει την κλήση επιστροφής που καλείται για τη δημιουργία πόρου αποθήκευσης της εικόνας.

**Returns:**
[IImageSavingCallback](../../com.aspose.note/iimagesavingcallback)
### getPageSavingCallback() {#getPageSavingCallback--}
```
public final IPageSavingCallback getPageSavingCallback()
```


Λαμβάνει ή ορίζει την κλήση επιστροφής που καλείται για τη δημιουργία πόρου αποθήκευσης της σελίδας.

**Returns:**
[IPageSavingCallback](../../com.aspose.note/ipagesavingcallback)
### setCssPerPageGeneration(boolean value) {#setCssPerPageGeneration-boolean-}
```
public final void setCssPerPageGeneration(boolean value)
```


Λαμβάνει ή ορίζει αν το αρχείο StyleSheet θα δημιουργείται ξεχωριστά για κάθε νέα σελίδα.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean |  |

### setCssSavingCallback(ICssSavingCallback value) {#setCssSavingCallback-com.aspose.note.ICssSavingCallback-}
```
public final void setCssSavingCallback(ICssSavingCallback value)
```


Λαμβάνει ή ορίζει την κλήση επιστροφής που καλείται για τη δημιουργία πόρου αποθήκευσης του CSS.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [ICssSavingCallback](../../com.aspose.note/icsssavingcallback) |  |

### setDocumentPerPageGeneration(boolean value) {#setDocumentPerPageGeneration-boolean-}
```
public final void setDocumentPerPageGeneration(boolean value)
```


Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει αν η δημιουργία εγγράφου ανά σελίδα είναι ενεργοποιημένη.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | boolean |  |

### setExportCss(int value) {#setExportCss-int-}
```
public final void setExportCss(int value)
```


Λαμβάνει ή ορίζει τον τρόπο εξαγωγής του css.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int |  |

### setExportFonts(int value) {#setExportFonts-int-}
```
public final void setExportFonts(int value)
```


Λαμβάνει ή ορίζει τον τρόπο εξαγωγής των γραμματοσειρών.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int |  |

### setExportImages(int value) {#setExportImages-int-}
```
public final void setExportImages(int value)
```


Λαμβάνει ή ορίζει τον τρόπο εξαγωγής των εικόνων.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int |  |

### setFontFaceTypes(int value) {#setFontFaceTypes-int-}
```
public final void setFontFaceTypes(int value)
```


Λαμβάνει ή ορίζει τους τύπους γραμματοσειρών.

Τιμή: Οι τύποι γραμματοσειρών.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τιμή | int |  |

### setFontSavingCallback(IFontSavingCallback value) {#setFontSavingCallback-com.aspose.note.IFontSavingCallback-}
```
public final void setFontSavingCallback(IFontSavingCallback value)
```


Λαμβάνει ή ορίζει την κλήση επιστροφής που καλείται για τη δημιουργία πόρου αποθήκευσης της γραμματοσειράς.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [IFontSavingCallback](../../com.aspose.note/ifontsavingcallback) |  |

### setImageSavingCallback(IImageSavingCallback value) {#setImageSavingCallback-com.aspose.note.IImageSavingCallback-}
```
public final void setImageSavingCallback(IImageSavingCallback value)
```


Λαμβάνει ή ορίζει την κλήση επιστροφής που καλείται για τη δημιουργία πόρου αποθήκευσης της εικόνας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [IImageSavingCallback](../../com.aspose.note/iimagesavingcallback) |  |

### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.note.IPageSavingCallback-}
```
public final void setPageSavingCallback(IPageSavingCallback value)
```


Λαμβάνει ή ορίζει την κλήση επιστροφής που καλείται για τη δημιουργία πόρου αποθήκευσης της σελίδας.

**Parameters:**
| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.note/ipagesavingcallback) |  |

