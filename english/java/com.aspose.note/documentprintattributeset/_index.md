---
title: DocumentPrintAttributeSet
second_title: Aspose.Note for Java API Reference
description: Represents helper class with user-friednly interface to with AttributeSet.
type: docs
weight: 21
url: /java/com.aspose.note/documentprintattributeset/
---

**Inheritance:**
java.lang.Object, javax.print.attribute.HashAttributeSet
```
public final class DocumentPrintAttributeSet extends HashAttributeSet
```

Represents helper class with user-friednly interface to with AttributeSet.
## Constructors

| Constructor | Description |
| --- | --- |
| [DocumentPrintAttributeSet(int copies)](#DocumentPrintAttributeSet-int-) | Initializes a new instance of `DocumentPrintAttributeSet`. |
| [DocumentPrintAttributeSet(String printerName, int copies)](#DocumentPrintAttributeSet-java.lang.String-int-) | Initializes a new instance of `DocumentPrintAttributeSet`. |
| [DocumentPrintAttributeSet(String printerName)](#DocumentPrintAttributeSet-java.lang.String-) | Initializes a new instance of `DocumentPrintAttributeSet`. |
| [DocumentPrintAttributeSet()](#DocumentPrintAttributeSet--) | Initializes a new instance of `DocumentPrintAttributeSet`. |
## Methods

| Method | Description |
| --- | --- |
| [getCopies()](#getCopies--) |  |
| [getLandscape()](#getLandscape--) |  |
| [getPrinterName()](#getPrinterName--) |  |
| [setCollate(boolean value)](#setCollate-boolean-) | Sets a value indicating whether document is collated. |
| [setCopies(int value)](#setCopies-int-) | Sets the number of copies to be printed. |
| [setDuplex(boolean value)](#setDuplex-boolean-) | Sets the printer setting for double-side printing. |
| [setLandscape(boolean value)](#setLandscape-boolean-) | Sets the orientation of the page. |
| [setPrintRange(int page)](#setPrintRange-int-) | Sets the single page to be printed. |
| [setPrintRange(int from, int to)](#setPrintRange-int-int-) | Sets the page range to be printed. |
| [setPrinterName(String printerName)](#setPrinterName-java.lang.String-) | The name of the printer to be used. |
| [setPrinterName(String printerName, Locale locale)](#setPrinterName-java.lang.String-java.util.Locale-) | The name of the printer to be used. |
### DocumentPrintAttributeSet(int copies) {#DocumentPrintAttributeSet-int-}
```
public DocumentPrintAttributeSet(int copies)
```


Initializes a new instance of `DocumentPrintAttributeSet`. By default all document's pages are printed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| copies | int | The number of document's copies to be printed. |

### DocumentPrintAttributeSet(String printerName, int copies) {#DocumentPrintAttributeSet-java.lang.String-int-}
```
public DocumentPrintAttributeSet(String printerName, int copies)
```


Initializes a new instance of `DocumentPrintAttributeSet`. By default all document's pages are printed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| printerName | java.lang.String | The name of the printer. |
| copies | int | The number of document's copies to be printed. |

### DocumentPrintAttributeSet(String printerName) {#DocumentPrintAttributeSet-java.lang.String-}
```
public DocumentPrintAttributeSet(String printerName)
```


Initializes a new instance of `DocumentPrintAttributeSet`. By default the only copy of every page.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| printerName | java.lang.String | The name of the printer. |

### DocumentPrintAttributeSet() {#DocumentPrintAttributeSet--}
```
public DocumentPrintAttributeSet()
```


Initializes a new instance of `DocumentPrintAttributeSet`. By default the only copy of every page.

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


Sets a value indicating whether document is collated.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | true is equivalent to setting of SheetCollate.COLLATED false is equivalent to setting of SheetCollate.UNCOLLATED |

### setCopies(int value) {#setCopies-int-}
```
public void setCopies(int value)
```


Sets the number of copies to be printed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | The number of copies to be printed. |

### setDuplex(boolean value) {#setDuplex-boolean-}
```
public void setDuplex(boolean value)
```


Sets the printer setting for double-side printing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | true is equivalent to setting of Sides.DUPLEX false is equivalent to setting of Sides.ONE\_SIDED |

### setLandscape(boolean value) {#setLandscape-boolean-}
```
public void setLandscape(boolean value)
```


Sets the orientation of the page.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | true is equivalent to setting of OrientationRequested.LANDSCAPE false is equivalent to setting of OrientationRequested.PORTRAIT |

### setPrintRange(int page) {#setPrintRange-int-}
```
public void setPrintRange(int page)
```


Sets the single page to be printed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| page | int | The page to be printed. |

### setPrintRange(int from, int to) {#setPrintRange-int-int-}
```
public void setPrintRange(int from, int to)
```


Sets the page range to be printed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| from | int | The first page. |
| to | int | The last page. |

### setPrinterName(String printerName) {#setPrinterName-java.lang.String-}
```
public void setPrinterName(String printerName)
```


The name of the printer to be used.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| printerName | java.lang.String | The name of the printer. |

### setPrinterName(String printerName, Locale locale) {#setPrinterName-java.lang.String-java.util.Locale-}
```
public void setPrinterName(String printerName, Locale locale)
```


The name of the printer to be used.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| printerName | java.lang.String | The name of the printer. |
| locale | java.util.Locale | printerName's locale. |

