---
title: "DocumentPrintAttributeSet"
second_title: "Referencia de API de Aspose.Note para Java"
description: "Representa una clase auxiliar con una interfaz fácil de usar con AttributeSet."
type: docs
weight: 21
url: /es/java/com.aspose.note/documentprintattributeset/
---

**Inheritance:**
java.lang.Object, javax.print.attribute.HashAttributeSet
```
public final class DocumentPrintAttributeSet extends HashAttributeSet
```

Representa una clase auxiliar con una interfaz fácil de usar con AttributeSet.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [DocumentPrintAttributeSet(int copies)](#DocumentPrintAttributeSet-int-) | Inicializa una nueva instancia de `DocumentPrintAttributeSet`. |
| [DocumentPrintAttributeSet(String printerName, int copies)](#DocumentPrintAttributeSet-java.lang.String-int-) | Inicializa una nueva instancia de `DocumentPrintAttributeSet`. |
| [DocumentPrintAttributeSet(String printerName)](#DocumentPrintAttributeSet-java.lang.String-) | Inicializa una nueva instancia de `DocumentPrintAttributeSet`. |
| [DocumentPrintAttributeSet()](#DocumentPrintAttributeSet--) | Inicializa una nueva instancia de `DocumentPrintAttributeSet`. |
## Métodos

| Método | Descripción |
| --- | --- |
| [getCopies()](#getCopies--) |  |
| [getLandscape()](#getLandscape--) |  |
| [getPrinterName()](#getPrinterName--) |  |
| [setCollate(boolean value)](#setCollate-boolean-) | Establece un valor que indica si el documento está encuadernado. |
| [setCopies(int value)](#setCopies-int-) | Establece el número de copias a imprimir. |
| [setDuplex(boolean value)](#setDuplex-boolean-) | Establece la configuración de la impresora para impresión a doble cara. |
| [setLandscape(boolean value)](#setLandscape-boolean-) | Establece la orientación de la página. |
| [setPrintRange(int page)](#setPrintRange-int-) | Establece la página única que se imprimirá. |
| [setPrintRange(int from, int to)](#setPrintRange-int-int-) | Establece el rango de páginas que se imprimirá. |
| [setPrinterName(String printerName)](#setPrinterName-java.lang.String-) | El nombre de la impresora a utilizar. |
| [setPrinterName(String printerName, Locale locale)](#setPrinterName-java.lang.String-java.util.Locale-) | El nombre de la impresora a utilizar. |
### DocumentPrintAttributeSet(int copies) {#DocumentPrintAttributeSet-int-}
```
public DocumentPrintAttributeSet(int copies)
```


Inicializa una nueva instancia de `DocumentPrintAttributeSet`. Por defecto se imprimen todas las páginas del documento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| copias | int | El número de copias del documento que se imprimirán. |

### DocumentPrintAttributeSet(String printerName, int copies) {#DocumentPrintAttributeSet-java.lang.String-int-}
```
public DocumentPrintAttributeSet(String printerName, int copies)
```


Inicializa una nueva instancia de `DocumentPrintAttributeSet`. Por defecto se imprimen todas las páginas del documento.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| printerName | java.lang.String | El nombre de la impresora. |
| copias | int | El número de copias del documento que se imprimirán. |

### DocumentPrintAttributeSet(String printerName) {#DocumentPrintAttributeSet-java.lang.String-}
```
public DocumentPrintAttributeSet(String printerName)
```


Inicializa una nueva instancia de `DocumentPrintAttributeSet`. Por defecto, solo hay una copia de cada página.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| printerName | java.lang.String | El nombre de la impresora. |

### DocumentPrintAttributeSet() {#DocumentPrintAttributeSet--}
```
public DocumentPrintAttributeSet()
```


Inicializa una nueva instancia de `DocumentPrintAttributeSet`. Por defecto, solo hay una copia de cada página.

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


Establece un valor que indica si el documento está encuadernado.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | true es equivalente a la configuración de SheetCollate.COLLATED false es equivalente a la configuración de SheetCollate.UNCOLLATED |

### setCopies(int value) {#setCopies-int-}
```
public void setCopies(int value)
```


Establece el número de copias a imprimir.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | El número de copias a imprimir. |

### setDuplex(boolean value) {#setDuplex-boolean-}
```
public void setDuplex(boolean value)
```


Establece la configuración de la impresora para impresión a doble cara.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | true es equivalente a la configuración de Sides.DUPLEX false es equivalente a la configuración de Sides.ONE\_SIDED |

### setLandscape(boolean value) {#setLandscape-boolean-}
```
public void setLandscape(boolean value)
```


Establece la orientación de la página.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | boolean | true es equivalente a la configuración de OrientationRequested.LANDSCAPE false es equivalente a la configuración de OrientationRequested.PORTRAIT |

### setPrintRange(int page) {#setPrintRange-int-}
```
public void setPrintRange(int page)
```


Establece la página única que se imprimirá.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| página | int | La página que se imprimirá. |

### setPrintRange(int from, int to) {#setPrintRange-int-int-}
```
public void setPrintRange(int from, int to)
```


Establece el rango de páginas que se imprimirá.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| desde | int | La primera página. |
| hasta | int | La última página. |

### setPrinterName(String printerName) {#setPrinterName-java.lang.String-}
```
public void setPrinterName(String printerName)
```


El nombre de la impresora a utilizar.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| printerName | java.lang.String | El nombre de la impresora. |

### setPrinterName(String printerName, Locale locale) {#setPrinterName-java.lang.String-java.util.Locale-}
```
public void setPrinterName(String printerName, Locale locale)
```


El nombre de la impresora a utilizar.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| printerName | java.lang.String | El nombre de la impresora. |
| configuración regional | java.util.Locale | configuración regional de printerName. |

