---
title: "DocumentPrintAttributeSet"
second_title: "Riferimento API di Aspose.Note per Java"
description: "Rappresenta una classe di supporto con interfaccia user‑friendly per AttributeSet."
type: docs
weight: 21
url: /it/java/com.aspose.note/documentprintattributeset/
---

**Inheritance:**
java.lang.Object, javax.print.attribute.HashAttributeSet
```
public final class DocumentPrintAttributeSet extends HashAttributeSet
```

Rappresenta una classe di supporto con interfaccia user‑friendly per AttributeSet.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [DocumentPrintAttributeSet(int copies)](#DocumentPrintAttributeSet-int-) | Inizializza una nuova istanza di `DocumentPrintAttributeSet`. |
| [DocumentPrintAttributeSet(String printerName, int copies)](#DocumentPrintAttributeSet-java.lang.String-int-) | Inizializza una nuova istanza di `DocumentPrintAttributeSet`. |
| [DocumentPrintAttributeSet(String printerName)](#DocumentPrintAttributeSet-java.lang.String-) | Inizializza una nuova istanza di `DocumentPrintAttributeSet`. |
| [DocumentPrintAttributeSet()](#DocumentPrintAttributeSet--) | Inizializza una nuova istanza di `DocumentPrintAttributeSet`. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getCopies()](#getCopies--) |  |
| [getLandscape()](#getLandscape--) |  |
| [getPrinterName()](#getPrinterName--) |  |
| [setCollate(boolean value)](#setCollate-boolean-) | Imposta un valore che indica se il documento è raggruppato. |
| [setCopies(int value)](#setCopies-int-) | Imposta il numero di copie da stampare. |
| [setDuplex(boolean value)](#setDuplex-boolean-) | Imposta l'opzione della stampante per la stampa fronte/retro. |
| [setLandscape(boolean value)](#setLandscape-boolean-) | Imposta l'orientamento della pagina. |
| [setPrintRange(int page)](#setPrintRange-int-) | Imposta la singola pagina da stampare. |
| [setPrintRange(int from, int to)](#setPrintRange-int-int-) | Imposta l'intervallo di pagine da stampare. |
| [setPrinterName(String printerName)](#setPrinterName-java.lang.String-) | Il nome della stampante da utilizzare. |
| [setPrinterName(String printerName, Locale locale)](#setPrinterName-java.lang.String-java.util.Locale-) | Il nome della stampante da utilizzare. |
### DocumentPrintAttributeSet(int copies) {#DocumentPrintAttributeSet-int-}
```
public DocumentPrintAttributeSet(int copies)
```


Inizializza una nuova istanza di `DocumentPrintAttributeSet`. Per impostazione predefinita vengono stampate tutte le pagine del documento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| copie | int | Il numero di copie del documento da stampare. |

### DocumentPrintAttributeSet(String printerName, int copies) {#DocumentPrintAttributeSet-java.lang.String-int-}
```
public DocumentPrintAttributeSet(String printerName, int copies)
```


Inizializza una nuova istanza di `DocumentPrintAttributeSet`. Per impostazione predefinita vengono stampate tutte le pagine del documento.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| printerName | java.lang.String | Il nome della stampante. |
| copie | int | Il numero di copie del documento da stampare. |

### DocumentPrintAttributeSet(String printerName) {#DocumentPrintAttributeSet-java.lang.String-}
```
public DocumentPrintAttributeSet(String printerName)
```


Inizializza una nuova istanza di `DocumentPrintAttributeSet`. Per impostazione predefinita è presente una sola copia di ogni pagina.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| printerName | java.lang.String | Il nome della stampante. |

### DocumentPrintAttributeSet() {#DocumentPrintAttributeSet--}
```
public DocumentPrintAttributeSet()
```


Inizializza una nuova istanza di `DocumentPrintAttributeSet`. Per impostazione predefinita è presente una sola copia di ogni pagina.

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


Imposta un valore che indica se il documento è raggruppato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | true è equivalente all'impostazione di SheetCollate.COLLATED false è equivalente all'impostazione di SheetCollate.UNCOLLATED |

### setCopies(int value) {#setCopies-int-}
```
public void setCopies(int value)
```


Imposta il numero di copie da stampare.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int | Il numero di copie da stampare. |

### setDuplex(boolean value) {#setDuplex-boolean-}
```
public void setDuplex(boolean value)
```


Imposta l'opzione della stampante per la stampa fronte/retro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | true è equivalente all'impostazione di Sides.DUPLEX false è equivalente all'impostazione di Sides.ONE\\_SIDED |

### setLandscape(boolean value) {#setLandscape-boolean-}
```
public void setLandscape(boolean value)
```


Imposta l'orientamento della pagina.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean | true è equivalente all'impostazione di OrientationRequested.LANDSCAPE false è equivalente all'impostazione di OrientationRequested.PORTRAIT |

### setPrintRange(int page) {#setPrintRange-int-}
```
public void setPrintRange(int page)
```


Imposta la singola pagina da stampare.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pagina | int | La pagina da stampare. |

### setPrintRange(int from, int to) {#setPrintRange-int-int-}
```
public void setPrintRange(int from, int to)
```


Imposta l'intervallo di pagine da stampare.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| da | int | La prima pagina. |
| a | int | L'ultima pagina. |

### setPrinterName(String printerName) {#setPrinterName-java.lang.String-}
```
public void setPrinterName(String printerName)
```


Il nome della stampante da utilizzare.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| printerName | java.lang.String | Il nome della stampante. |

### setPrinterName(String printerName, Locale locale) {#setPrinterName-java.lang.String-java.util.Locale-}
```
public void setPrinterName(String printerName, Locale locale)
```


Il nome della stampante da utilizzare.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| printerName | java.lang.String | Il nome della stampante. |
| locale | java.util.Locale | locale di printerName. |

