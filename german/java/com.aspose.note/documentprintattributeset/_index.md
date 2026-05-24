---
title: "DocumentPrintAttributeSet"
second_title: "Aspose.Note für Java API-Referenz"
description: "Stellt eine Hilfsklasse mit benutzerfreundlicher Schnittstelle zu AttributeSet dar."
type: docs
weight: 21
url: /de/java/com.aspose.note/documentprintattributeset/
---

**Inheritance:**
java.lang.Object, javax.print.attribute.HashAttributeSet
```
public final class DocumentPrintAttributeSet extends HashAttributeSet
```

Stellt eine Hilfsklasse mit benutzerfreundlicher Schnittstelle zu AttributeSet dar.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [DocumentPrintAttributeSet(int copies)](#DocumentPrintAttributeSet-int-) | Initialisiert eine neue Instanz von `DocumentPrintAttributeSet`. |
| [DocumentPrintAttributeSet(String printerName, int copies)](#DocumentPrintAttributeSet-java.lang.String-int-) | Initialisiert eine neue Instanz von `DocumentPrintAttributeSet`. |
| [DocumentPrintAttributeSet(String printerName)](#DocumentPrintAttributeSet-java.lang.String-) | Initialisiert eine neue Instanz von `DocumentPrintAttributeSet`. |
| [DocumentPrintAttributeSet()](#DocumentPrintAttributeSet--) | Initialisiert eine neue Instanz von `DocumentPrintAttributeSet`. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getCopies()](#getCopies--) |  |
| [getLandscape()](#getLandscape--) |  |
| [getPrinterName()](#getPrinterName--) |  |
| [setCollate(boolean value)](#setCollate-boolean-) | Legt einen Wert fest, der angibt, ob das Dokument collated ist. |
| [setCopies(int value)](#setCopies-int-) | Legt die Anzahl der zu druckenden Kopien fest. |
| [setDuplex(boolean value)](#setDuplex-boolean-) | Legt die Druckereinstellung für doppelseitiges Drucken fest. |
| [setLandscape(boolean value)](#setLandscape-boolean-) | Legt die Ausrichtung der Seite fest. |
| [setPrintRange(int page)](#setPrintRange-int-) | Legt die einzelne zu druckende Seite fest. |
| [setPrintRange(int from, int to)](#setPrintRange-int-int-) | Legt den zu druckenden Seitenbereich fest. |
| [setPrinterName(String printerName)](#setPrinterName-java.lang.String-) | Der Name des zu verwendenden Druckers. |
| [setPrinterName(String printerName, Locale locale)](#setPrinterName-java.lang.String-java.util.Locale-) | Der Name des zu verwendenden Druckers. |
### DocumentPrintAttributeSet(int copies) {#DocumentPrintAttributeSet-int-}
```
public DocumentPrintAttributeSet(int copies)
```


Initialisiert eine neue Instanz von `DocumentPrintAttributeSet`. Standardmäßig werden alle Seiten des Dokuments gedruckt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Kopien | int | Die Anzahl der zu druckenden Kopien des Dokuments. |

### DocumentPrintAttributeSet(String printerName, int copies) {#DocumentPrintAttributeSet-java.lang.String-int-}
```
public DocumentPrintAttributeSet(String printerName, int copies)
```


Initialisiert eine neue Instanz von `DocumentPrintAttributeSet`. Standardmäßig werden alle Seiten des Dokuments gedruckt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| printerName | java.lang.String | Der Name des Druckers. |
| Kopien | int | Die Anzahl der zu druckenden Kopien des Dokuments. |

### DocumentPrintAttributeSet(String printerName) {#DocumentPrintAttributeSet-java.lang.String-}
```
public DocumentPrintAttributeSet(String printerName)
```


Initialisiert eine neue Instanz von `DocumentPrintAttributeSet`. Standardmäßig wird nur eine Kopie jeder Seite gedruckt.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| printerName | java.lang.String | Der Name des Druckers. |

### DocumentPrintAttributeSet() {#DocumentPrintAttributeSet--}
```
public DocumentPrintAttributeSet()
```


Initialisiert eine neue Instanz von `DocumentPrintAttributeSet`. Standardmäßig wird nur eine Kopie jeder Seite gedruckt.

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


Legt einen Wert fest, der angibt, ob das Dokument collated ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | true entspricht der Einstellung SheetCollate.COLLATED, false entspricht der Einstellung SheetCollate.UNCOLLATED |

### setCopies(int value) {#setCopies-int-}
```
public void setCopies(int value)
```


Legt die Anzahl der zu druckenden Kopien fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int | Die Anzahl der zu druckenden Kopien. |

### setDuplex(boolean value) {#setDuplex-boolean-}
```
public void setDuplex(boolean value)
```


Legt die Druckereinstellung für doppelseitiges Drucken fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | true entspricht der Einstellung Sides.DUPLEX, false entspricht der Einstellung Sides.ONE\_SIDED |

### setLandscape(boolean value) {#setLandscape-boolean-}
```
public void setLandscape(boolean value)
```


Legt die Ausrichtung der Seite fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | true entspricht der Einstellung OrientationRequested.LANDSCAPE, false entspricht der Einstellung OrientationRequested.PORTRAIT |

### setPrintRange(int page) {#setPrintRange-int-}
```
public void setPrintRange(int page)
```


Legt die einzelne zu druckende Seite fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Seite | int | Die zu druckende Seite. |

### setPrintRange(int from, int to) {#setPrintRange-int-int-}
```
public void setPrintRange(int from, int to)
```


Legt den zu druckenden Seitenbereich fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| von | int | Die erste Seite. |
| bis | int | Die letzte Seite. |

### setPrinterName(String printerName) {#setPrinterName-java.lang.String-}
```
public void setPrinterName(String printerName)
```


Der Name des zu verwendenden Druckers.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| printerName | java.lang.String | Der Name des Druckers. |

### setPrinterName(String printerName, Locale locale) {#setPrinterName-java.lang.String-java.util.Locale-}
```
public void setPrinterName(String printerName, Locale locale)
```


Der Name des zu verwendenden Druckers.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| printerName | java.lang.String | Der Name des Druckers. |
| Locale | java.util.Locale | Die Locale von printerName. |

