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
| [DocumentPrintAttributeSet(int copies)](#DocumentPrintAttributeSet-int-) | Initializes a new instance of  DocumentPrintAttributeSet . |
| [DocumentPrintAttributeSet(String printerName, int copies)](#DocumentPrintAttributeSet-java.lang.String-int-) | Initializes a new instance of  DocumentPrintAttributeSet . |
| [DocumentPrintAttributeSet(String printerName)](#DocumentPrintAttributeSet-java.lang.String-) | Initializes a new instance of  DocumentPrintAttributeSet . |
| [DocumentPrintAttributeSet()](#DocumentPrintAttributeSet--) | Initializes a new instance of  DocumentPrintAttributeSet . |
## Methods

| Method | Description |
| --- | --- |
| [add(Attribute arg0)](#add-javax.print.attribute.Attribute-) |  |
| [addAll(AttributeSet arg0)](#addAll-javax.print.attribute.AttributeSet-) |  |
| [clear()](#clear--) |  |
| [containsKey(Class<?> arg0)](#containsKey-java.lang.Class----) |  |
| [containsValue(Attribute arg0)](#containsValue-javax.print.attribute.Attribute-) |  |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(Class<?> arg0)](#get-java.lang.Class----) |  |
| [getClass()](#getClass--) |  |
| [getCopies()](#getCopies--) |  |
| [getLandscape()](#getLandscape--) |  |
| [getPrinterName()](#getPrinterName--) |  |
| [hashCode()](#hashCode--) |  |
| [isEmpty()](#isEmpty--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(Class<?> arg0)](#remove-java.lang.Class----) |  |
| [remove(Attribute arg0)](#remove-javax.print.attribute.Attribute-) |  |
| [setCollate(boolean value)](#setCollate-boolean-) | Sets a value indicating whether document is collated. |
| [setCopies(int value)](#setCopies-int-) | Sets the number of copies to be printed. |
| [setDuplex(boolean value)](#setDuplex-boolean-) | Sets the printer setting for double-side printing. |
| [setLandscape(boolean value)](#setLandscape-boolean-) | Sets the orientation of the page. |
| [setPrintRange(int page)](#setPrintRange-int-) | Sets the single page to be printed. |
| [setPrintRange(int from, int to)](#setPrintRange-int-int-) | Sets the page range to be printed. |
| [setPrinterName(String printerName)](#setPrinterName-java.lang.String-) | The name of the printer to be used. |
| [setPrinterName(String printerName, Locale locale)](#setPrinterName-java.lang.String-java.util.Locale-) | The name of the printer to be used. |
| [size()](#size--) |  |
| [toArray()](#toArray--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### DocumentPrintAttributeSet(int copies) {#DocumentPrintAttributeSet-int-}
```
public DocumentPrintAttributeSet(int copies)
```


Initializes a new instance of  DocumentPrintAttributeSet . By default all document's pages are printed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| copies | int | The number of document's copies to be printed. |

### DocumentPrintAttributeSet(String printerName, int copies) {#DocumentPrintAttributeSet-java.lang.String-int-}
```
public DocumentPrintAttributeSet(String printerName, int copies)
```


Initializes a new instance of  DocumentPrintAttributeSet . By default all document's pages are printed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| printerName | java.lang.String | The name of the printer. |
| copies | int | The number of document's copies to be printed. |

### DocumentPrintAttributeSet(String printerName) {#DocumentPrintAttributeSet-java.lang.String-}
```
public DocumentPrintAttributeSet(String printerName)
```


Initializes a new instance of  DocumentPrintAttributeSet . By default the only copy of every page.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| printerName | java.lang.String | The name of the printer. |

### DocumentPrintAttributeSet() {#DocumentPrintAttributeSet--}
```
public DocumentPrintAttributeSet()
```


Initializes a new instance of  DocumentPrintAttributeSet . By default the only copy of every page.

### add(Attribute arg0) {#add-javax.print.attribute.Attribute-}
```
public boolean add(Attribute arg0)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | javax.print.attribute.Attribute |  |

**Returns:**
boolean
### addAll(AttributeSet arg0) {#addAll-javax.print.attribute.AttributeSet-}
```
public boolean addAll(AttributeSet arg0)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | javax.print.attribute.AttributeSet |  |

**Returns:**
boolean
### clear() {#clear--}
```
public void clear()
```




### containsKey(Class<?> arg0) {#containsKey-java.lang.Class----}
```
public boolean containsKey(Class<?> arg0)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Class<?> |  |

**Returns:**
boolean
### containsValue(Attribute arg0) {#containsValue-javax.print.attribute.Attribute-}
```
public boolean containsValue(Attribute arg0)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | javax.print.attribute.Attribute |  |

**Returns:**
boolean
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### get(Class<?> arg0) {#get-java.lang.Class----}
```
public Attribute get(Class<?> arg0)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Class<?> |  |

**Returns:**
javax.print.attribute.Attribute
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
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
### hashCode() {#hashCode--}
```
public int hashCode()
```




**Returns:**
int
### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```




**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### remove(Class<?> arg0) {#remove-java.lang.Class----}
```
public boolean remove(Class<?> arg0)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Class<?> |  |

**Returns:**
boolean
### remove(Attribute arg0) {#remove-javax.print.attribute.Attribute-}
```
public boolean remove(Attribute arg0)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | javax.print.attribute.Attribute |  |

**Returns:**
boolean
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

### size() {#size--}
```
public int size()
```




**Returns:**
int
### toArray() {#toArray--}
```
public Attribute[] toArray()
```




**Returns:**
javax.print.attribute.Attribute[]
### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final void wait(long arg0)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

