---
title: "DocumentPrintAttributeSet"
second_title: "Aspose.Note for Java API-referentie"
description: "Stelt een hulpprogrammaklasse met een gebruiksvriendelijke interface naar AttributeSet voor."
type: docs
weight: 21
url: /nl/java/com.aspose.note/documentprintattributeset/
---

**Inheritance:**
java.lang.Object, javax.print.attribute.HashAttributeSet
```
public final class DocumentPrintAttributeSet extends HashAttributeSet
```

Stelt een hulpprogrammaklasse met een gebruiksvriendelijke interface naar AttributeSet voor.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [DocumentPrintAttributeSet(int copies)](#DocumentPrintAttributeSet-int-) | Initialiseert een nieuw exemplaar van `DocumentPrintAttributeSet`. |
| [DocumentPrintAttributeSet(String printerName, int copies)](#DocumentPrintAttributeSet-java.lang.String-int-) | Initialiseert een nieuw exemplaar van `DocumentPrintAttributeSet`. |
| [DocumentPrintAttributeSet(String printerName)](#DocumentPrintAttributeSet-java.lang.String-) | Initialiseert een nieuw exemplaar van `DocumentPrintAttributeSet`. |
| [DocumentPrintAttributeSet()](#DocumentPrintAttributeSet--) | Initialiseert een nieuw exemplaar van `DocumentPrintAttributeSet`. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getCopies()](#getCopies--) |  |
| [getLandscape()](#getLandscape--) |  |
| [getPrinterName()](#getPrinterName--) |  |
| [setCollate(boolean value)](#setCollate-boolean-) | Stelt een waarde in die aangeeft of het document is gecollateerd. |
| [setCopies(int value)](#setCopies-int-) | Stelt het aantal exemplaren in dat moet worden afgedrukt. |
| [setDuplex(boolean value)](#setDuplex-boolean-) | Stelt de printerinstelling in voor dubbelzijdig afdrukken. |
| [setLandscape(boolean value)](#setLandscape-boolean-) | Stelt de oriëntatie van de pagina in. |
| [setPrintRange(int page)](#setPrintRange-int-) | Stelt de enkele pagina in die moet worden afgedrukt. |
| [setPrintRange(int from, int to)](#setPrintRange-int-int-) | Stelt het paginabereik in dat moet worden afgedrukt. |
| [setPrinterName(String printerName)](#setPrinterName-java.lang.String-) | De naam van de te gebruiken printer. |
| [setPrinterName(String printerName, Locale locale)](#setPrinterName-java.lang.String-java.util.Locale-) | De naam van de te gebruiken printer. |
### DocumentPrintAttributeSet(int copies) {#DocumentPrintAttributeSet-int-}
```
public DocumentPrintAttributeSet(int copies)
```


Initialiseert een nieuw exemplaar van `DocumentPrintAttributeSet`. Standaard worden alle pagina's van het document afgedrukt.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| copies | int | Het aantal exemplaren van het document dat moet worden afgedrukt. |

### DocumentPrintAttributeSet(String printerName, int copies) {#DocumentPrintAttributeSet-java.lang.String-int-}
```
public DocumentPrintAttributeSet(String printerName, int copies)
```


Initialiseert een nieuw exemplaar van `DocumentPrintAttributeSet`. Standaard worden alle pagina's van het document afgedrukt.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| printerName | java.lang.String | De naam van de printer. |
| copies | int | Het aantal exemplaren van het document dat moet worden afgedrukt. |

### DocumentPrintAttributeSet(String printerName) {#DocumentPrintAttributeSet-java.lang.String-}
```
public DocumentPrintAttributeSet(String printerName)
```


Initialiseert een nieuw exemplaar van `DocumentPrintAttributeSet`. Standaard is er slechts één exemplaar van elke pagina.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| printerName | java.lang.String | De naam van de printer. |

### DocumentPrintAttributeSet() {#DocumentPrintAttributeSet--}
```
public DocumentPrintAttributeSet()
```


Initialiseert een nieuw exemplaar van `DocumentPrintAttributeSet`. Standaard is er slechts één exemplaar van elke pagina.

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


Stelt een waarde in die aangeeft of het document is gecollateerd.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | true is equivalent aan de instelling van SheetCollate.COLLATED false is equivalent aan de instelling van SheetCollate.UNCOLLATED |

### setCopies(int value) {#setCopies-int-}
```
public void setCopies(int value)
```


Stelt het aantal exemplaren in dat moet worden afgedrukt.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | int | Het aantal exemplaren dat moet worden afgedrukt. |

### setDuplex(boolean value) {#setDuplex-boolean-}
```
public void setDuplex(boolean value)
```


Stelt de printerinstelling in voor dubbelzijdig afdrukken.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | true is equivalent aan de instelling van Sides.DUPLEX false is equivalent aan de instelling van Sides.ONE\_SIDED |

### setLandscape(boolean value) {#setLandscape-boolean-}
```
public void setLandscape(boolean value)
```


Stelt de oriëntatie van de pagina in.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | true is equivalent aan de instelling van OrientationRequested.LANDSCAPE false is equivalent aan de instelling van OrientationRequested.PORTRAIT |

### setPrintRange(int page) {#setPrintRange-int-}
```
public void setPrintRange(int page)
```


Stelt de enkele pagina in die moet worden afgedrukt.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pagina | int | De pagina die moet worden afgedrukt. |

### setPrintRange(int from, int to) {#setPrintRange-int-int-}
```
public void setPrintRange(int from, int to)
```


Stelt het paginabereik in dat moet worden afgedrukt.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| van | int | De eerste pagina. |
| tot | int | De laatste pagina. |

### setPrinterName(String printerName) {#setPrinterName-java.lang.String-}
```
public void setPrinterName(String printerName)
```


De naam van de te gebruiken printer.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| printerName | java.lang.String | De naam van de printer. |

### setPrinterName(String printerName, Locale locale) {#setPrinterName-java.lang.String-java.util.Locale-}
```
public void setPrinterName(String printerName, Locale locale)
```


De naam van de te gebruiken printer.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| printerName | java.lang.String | De naam van de printer. |
| locale | java.util.Locale | locale van printerName. |

