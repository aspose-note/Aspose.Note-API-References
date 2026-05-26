---
title: "DocumentPrintAttributeSet"
second_title: "Aspose.Note for Java API-referens"
description: "Representerar en hjälparklass med ett användarvänligt gränssnitt till AttributeSet."
type: docs
weight: 21
url: /sv/java/com.aspose.note/documentprintattributeset/
---

**Inheritance:**
java.lang.Object, javax.print.attribute.HashAttributeSet
```
public final class DocumentPrintAttributeSet extends HashAttributeSet
```

Representerar en hjälparklass med ett användarvänligt gränssnitt till AttributeSet.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [DocumentPrintAttributeSet(int copies)](#DocumentPrintAttributeSet-int-) | Initierar en ny instans av `DocumentPrintAttributeSet`. |
| [DocumentPrintAttributeSet(String printerName, int copies)](#DocumentPrintAttributeSet-java.lang.String-int-) | Initierar en ny instans av `DocumentPrintAttributeSet`. |
| [DocumentPrintAttributeSet(String printerName)](#DocumentPrintAttributeSet-java.lang.String-) | Initierar en ny instans av `DocumentPrintAttributeSet`. |
| [DocumentPrintAttributeSet()](#DocumentPrintAttributeSet--) | Initierar en ny instans av `DocumentPrintAttributeSet`. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getCopies()](#getCopies--) |  |
| [getLandscape()](#getLandscape--) |  |
| [getPrinterName()](#getPrinterName--) |  |
| [setCollate(boolean value)](#setCollate-boolean-) | Ställer in ett värde som indikerar om dokumentet är sammanställt. |
| [setCopies(int value)](#setCopies-int-) | Ställer in antalet kopior som ska skrivas ut. |
| [setDuplex(boolean value)](#setDuplex-boolean-) | Ställer in skrivarinställningen för dubbelsidig utskrift. |
| [setLandscape(boolean value)](#setLandscape-boolean-) | Ställer in sidans orientering. |
| [setPrintRange(int page)](#setPrintRange-int-) | Ställer in den enskilda sidan som ska skrivas ut. |
| [setPrintRange(int from, int to)](#setPrintRange-int-int-) | Ställer in sidintervallet som ska skrivas ut. |
| [setPrinterName(String printerName)](#setPrinterName-java.lang.String-) | Namnet på den skrivare som ska användas. |
| [setPrinterName(String printerName, Locale locale)](#setPrinterName-java.lang.String-java.util.Locale-) | Namnet på den skrivare som ska användas. |
### DocumentPrintAttributeSet(int copies) {#DocumentPrintAttributeSet-int-}
```
public DocumentPrintAttributeSet(int copies)
```


Initierar en ny instans av `DocumentPrintAttributeSet`. Som standard skrivs alla dokumentets sidor ut.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| kopior | int | Antalet kopior av dokumentet som ska skrivas ut. |

### DocumentPrintAttributeSet(String printerName, int copies) {#DocumentPrintAttributeSet-java.lang.String-int-}
```
public DocumentPrintAttributeSet(String printerName, int copies)
```


Initierar en ny instans av `DocumentPrintAttributeSet`. Som standard skrivs alla dokumentets sidor ut.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| printerName | java.lang.String | Namnet på skrivaren. |
| kopior | int | Antalet kopior av dokumentet som ska skrivas ut. |

### DocumentPrintAttributeSet(String printerName) {#DocumentPrintAttributeSet-java.lang.String-}
```
public DocumentPrintAttributeSet(String printerName)
```


Initierar en ny instans av `DocumentPrintAttributeSet`. Som standard är det endast en kopia av varje sida.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| printerName | java.lang.String | Namnet på skrivaren. |

### DocumentPrintAttributeSet() {#DocumentPrintAttributeSet--}
```
public DocumentPrintAttributeSet()
```


Initierar en ny instans av `DocumentPrintAttributeSet`. Som standard är det endast en kopia av varje sida.

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


Ställer in ett värde som indikerar om dokumentet är sammanställt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | true motsvarar inställningen SheetCollate.COLLATED false motsvarar inställningen SheetCollate.UNCOLLATED |

### setCopies(int value) {#setCopies-int-}
```
public void setCopies(int value)
```


Ställer in antalet kopior som ska skrivas ut.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int | Antalet kopior som ska skrivas ut. |

### setDuplex(boolean value) {#setDuplex-boolean-}
```
public void setDuplex(boolean value)
```


Ställer in skrivarinställningen för dubbelsidig utskrift.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | true motsvarar inställningen Sides.DUPLEX false motsvarar inställningen Sides.ONE\\_SIDED |

### setLandscape(boolean value) {#setLandscape-boolean-}
```
public void setLandscape(boolean value)
```


Ställer in sidans orientering.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | true motsvarar inställningen OrientationRequested.LANDSCAPE false motsvarar inställningen OrientationRequested.PORTRAIT |

### setPrintRange(int page) {#setPrintRange-int-}
```
public void setPrintRange(int page)
```


Ställer in den enskilda sidan som ska skrivas ut.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sida | int | Sidan som ska skrivas ut. |

### setPrintRange(int from, int to) {#setPrintRange-int-int-}
```
public void setPrintRange(int from, int to)
```


Ställer in sidintervallet som ska skrivas ut.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| från | int | Den första sidan. |
| till | int | Den sista sidan. |

### setPrinterName(String printerName) {#setPrinterName-java.lang.String-}
```
public void setPrinterName(String printerName)
```


Namnet på den skrivare som ska användas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| printerName | java.lang.String | Namnet på skrivaren. |

### setPrinterName(String printerName, Locale locale) {#setPrinterName-java.lang.String-java.util.Locale-}
```
public void setPrinterName(String printerName, Locale locale)
```


Namnet på den skrivare som ska användas.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| printerName | java.lang.String | Namnet på skrivaren. |
| lokal | java.util.Locale | printerName:s lokal. |

