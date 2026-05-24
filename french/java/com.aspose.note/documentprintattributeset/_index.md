---
title: "DocumentPrintAttributeSet"
second_title: "Référence d'API Aspose.Note pour Java"
description: "Représente une classe d'assistance avec une interface conviviale pour AttributeSet."
type: docs
weight: 21
url: /fr/java/com.aspose.note/documentprintattributeset/
---

**Inheritance:**
java.lang.Object, javax.print.attribute.HashAttributeSet
```
public final class DocumentPrintAttributeSet extends HashAttributeSet
```

Représente une classe d'assistance avec une interface conviviale pour AttributeSet.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [DocumentPrintAttributeSet(int copies)](#DocumentPrintAttributeSet-int-) | Initialise une nouvelle instance de `DocumentPrintAttributeSet`. |
| [DocumentPrintAttributeSet(String printerName, int copies)](#DocumentPrintAttributeSet-java.lang.String-int-) | Initialise une nouvelle instance de `DocumentPrintAttributeSet`. |
| [DocumentPrintAttributeSet(String printerName)](#DocumentPrintAttributeSet-java.lang.String-) | Initialise une nouvelle instance de `DocumentPrintAttributeSet`. |
| [DocumentPrintAttributeSet()](#DocumentPrintAttributeSet--) | Initialise une nouvelle instance de `DocumentPrintAttributeSet`. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getCopies()](#getCopies--) |  |
| [getLandscape()](#getLandscape--) |  |
| [getPrinterName()](#getPrinterName--) |  |
| [setCollate(boolean value)](#setCollate-boolean-) | Définit une valeur indiquant si le document est assemblé. |
| [setCopies(int value)](#setCopies-int-) | Définit le nombre de copies à imprimer. |
| [setDuplex(boolean value)](#setDuplex-boolean-) | Définit le paramètre d’imprimante pour l’impression recto verso. |
| [setLandscape(boolean value)](#setLandscape-boolean-) | Définit l’orientation de la page. |
| [setPrintRange(int page)](#setPrintRange-int-) | Définit la page unique à imprimer. |
| [setPrintRange(int from, int to)](#setPrintRange-int-int-) | Définit la plage de pages à imprimer. |
| [setPrinterName(String printerName)](#setPrinterName-java.lang.String-) | Le nom de l’imprimante à utiliser. |
| [setPrinterName(String printerName, Locale locale)](#setPrinterName-java.lang.String-java.util.Locale-) | Le nom de l’imprimante à utiliser. |
### DocumentPrintAttributeSet(int copies) {#DocumentPrintAttributeSet-int-}
```
public DocumentPrintAttributeSet(int copies)
```


Initialise une nouvelle instance de `DocumentPrintAttributeSet`. Par défaut, toutes les pages du document sont imprimées.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| copies | int | Le nombre de copies du document à imprimer. |

### DocumentPrintAttributeSet(String printerName, int copies) {#DocumentPrintAttributeSet-java.lang.String-int-}
```
public DocumentPrintAttributeSet(String printerName, int copies)
```


Initialise une nouvelle instance de `DocumentPrintAttributeSet`. Par défaut, toutes les pages du document sont imprimées.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| printerName | java.lang.String | Le nom de l’imprimante. |
| copies | int | Le nombre de copies du document à imprimer. |

### DocumentPrintAttributeSet(String printerName) {#DocumentPrintAttributeSet-java.lang.String-}
```
public DocumentPrintAttributeSet(String printerName)
```


Initialise une nouvelle instance de `DocumentPrintAttributeSet`. Par défaut, une seule copie de chaque page.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| printerName | java.lang.String | Le nom de l’imprimante. |

### DocumentPrintAttributeSet() {#DocumentPrintAttributeSet--}
```
public DocumentPrintAttributeSet()
```


Initialise une nouvelle instance de `DocumentPrintAttributeSet`. Par défaut, une seule copie de chaque page.

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


Définit une valeur indiquant si le document est assemblé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean | true équivaut au paramètre SheetCollate.COLLATED, false équivaut au paramètre SheetCollate.UNCOLLATED |

### setCopies(int value) {#setCopies-int-}
```
public void setCopies(int value)
```


Définit le nombre de copies à imprimer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | Le nombre de copies à imprimer. |

### setDuplex(boolean value) {#setDuplex-boolean-}
```
public void setDuplex(boolean value)
```


Définit le paramètre d’imprimante pour l’impression recto verso.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean | true équivaut au paramètre Sides.DUPLEX, false équivaut au paramètre Sides.ONE\_SIDED |

### setLandscape(boolean value) {#setLandscape-boolean-}
```
public void setLandscape(boolean value)
```


Définit l’orientation de la page.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | boolean | true équivaut au paramètre OrientationRequested.LANDSCAPE, false équivaut au paramètre OrientationRequested.PORTRAIT |

### setPrintRange(int page) {#setPrintRange-int-}
```
public void setPrintRange(int page)
```


Définit la page unique à imprimer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| page | int | La page à imprimer. |

### setPrintRange(int from, int to) {#setPrintRange-int-int-}
```
public void setPrintRange(int from, int to)
```


Définit la plage de pages à imprimer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| de | int | La première page. |
| à | int | La dernière page. |

### setPrinterName(String printerName) {#setPrinterName-java.lang.String-}
```
public void setPrinterName(String printerName)
```


Le nom de l’imprimante à utiliser.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| printerName | java.lang.String | Le nom de l’imprimante. |

### setPrinterName(String printerName, Locale locale) {#setPrinterName-java.lang.String-java.util.Locale-}
```
public void setPrinterName(String printerName, Locale locale)
```


Le nom de l’imprimante à utiliser.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| printerName | java.lang.String | Le nom de l’imprimante. |
| locale | java.util.Locale | locale de printerName. |

