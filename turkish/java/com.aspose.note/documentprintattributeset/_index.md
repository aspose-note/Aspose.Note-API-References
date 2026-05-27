---
title: "DocumentPrintAttributeSet"
second_title: "Aspose.Note for Java API Referansı"
description: "AttributeSet ile kullanıcı dostu bir arayüze sahip yardımcı sınıfı temsil eder."
type: docs
weight: 21
url: /tr/java/com.aspose.note/documentprintattributeset/
---

**Inheritance:**
java.lang.Object, javax.print.attribute.HashAttributeSet
```
public final class DocumentPrintAttributeSet extends HashAttributeSet
```

AttributeSet ile kullanıcı dostu bir arayüze sahip yardımcı sınıfı temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [DocumentPrintAttributeSet(int copies)](#DocumentPrintAttributeSet-int-) | Yeni bir `DocumentPrintAttributeSet` örneği başlatır. |
| [DocumentPrintAttributeSet(String printerName, int copies)](#DocumentPrintAttributeSet-java.lang.String-int-) | Yeni bir `DocumentPrintAttributeSet` örneği başlatır. |
| [DocumentPrintAttributeSet(String printerName)](#DocumentPrintAttributeSet-java.lang.String-) | Yeni bir `DocumentPrintAttributeSet` örneği başlatır. |
| [DocumentPrintAttributeSet()](#DocumentPrintAttributeSet--) | Yeni bir `DocumentPrintAttributeSet` örneği başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getCopies()](#getCopies--) |  |
| [getLandscape()](#getLandscape--) |  |
| [getPrinterName()](#getPrinterName--) |  |
| [setCollate(boolean value)](#setCollate-boolean-) | Belgenin sıralı olup olmadığını gösteren bir değer ayarlar. |
| [setCopies(int value)](#setCopies-int-) | Yazdırılacak kopya sayısını ayarlar. |
| [setDuplex(boolean value)](#setDuplex-boolean-) | Çift taraflı baskı için yazıcı ayarını belirler. |
| [setLandscape(boolean value)](#setLandscape-boolean-) | Sayfanın yönünü ayarlar. |
| [setPrintRange(int page)](#setPrintRange-int-) | Yazdırılacak tek sayfayı ayarlar. |
| [setPrintRange(int from, int to)](#setPrintRange-int-int-) | Yazdırılacak sayfa aralığını ayarlar. |
| [setPrinterName(String printerName)](#setPrinterName-java.lang.String-) | Kullanılacak yazıcının adı. |
| [setPrinterName(String printerName, Locale locale)](#setPrinterName-java.lang.String-java.util.Locale-) | Kullanılacak yazıcının adı. |
### DocumentPrintAttributeSet(int copies) {#DocumentPrintAttributeSet-int-}
```
public DocumentPrintAttributeSet(int copies)
```


Yeni bir `DocumentPrintAttributeSet` örneği başlatır. Varsayılan olarak belgenin tüm sayfaları yazdırılır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| kopyalar | int | Yazdırılacak belgenin kopya sayısı. |

### DocumentPrintAttributeSet(String printerName, int copies) {#DocumentPrintAttributeSet-java.lang.String-int-}
```
public DocumentPrintAttributeSet(String printerName, int copies)
```


Yeni bir `DocumentPrintAttributeSet` örneği başlatır. Varsayılan olarak belgenin tüm sayfaları yazdırılır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| printerName | java.lang.String | Yazıcının adı. |
| kopyalar | int | Yazdırılacak belgenin kopya sayısı. |

### DocumentPrintAttributeSet(String printerName) {#DocumentPrintAttributeSet-java.lang.String-}
```
public DocumentPrintAttributeSet(String printerName)
```


Yeni bir `DocumentPrintAttributeSet` örneği başlatır. Varsayılan olarak her sayfanın tek kopyası.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| printerName | java.lang.String | Yazıcının adı. |

### DocumentPrintAttributeSet() {#DocumentPrintAttributeSet--}
```
public DocumentPrintAttributeSet()
```


Yeni bir `DocumentPrintAttributeSet` örneği başlatır. Varsayılan olarak her sayfanın tek kopyası.

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


Belgenin sıralı olup olmadığını gösteren bir değer ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | true, SheetCollate.COLLATED ayarına eşittir; false, SheetCollate.UNCOLLATED ayarına eşittir. |

### setCopies(int value) {#setCopies-int-}
```
public void setCopies(int value)
```


Yazdırılacak kopya sayısını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | Yazdırılacak kopya sayısı. |

### setDuplex(boolean value) {#setDuplex-boolean-}
```
public void setDuplex(boolean value)
```


Çift taraflı baskı için yazıcı ayarını belirler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | true, Sides.DUPLEX ayarına eşittir; false, Sides.ONE\_SIDED ayarına eşittir. |

### setLandscape(boolean value) {#setLandscape-boolean-}
```
public void setLandscape(boolean value)
```


Sayfanın yönünü ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | true, OrientationRequested.LANDSCAPE ayarına eşittir; false, OrientationRequested.PORTRAIT ayarına eşittir. |

### setPrintRange(int page) {#setPrintRange-int-}
```
public void setPrintRange(int page)
```


Yazdırılacak tek sayfayı ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sayfa | int | Yazdırılacak sayfa. |

### setPrintRange(int from, int to) {#setPrintRange-int-int-}
```
public void setPrintRange(int from, int to)
```


Yazdırılacak sayfa aralığını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| başlangıç | int | İlk sayfa. |
| bitiş | int | Son sayfa. |

### setPrinterName(String printerName) {#setPrinterName-java.lang.String-}
```
public void setPrinterName(String printerName)
```


Kullanılacak yazıcının adı.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| printerName | java.lang.String | Yazıcının adı. |

### setPrinterName(String printerName, Locale locale) {#setPrinterName-java.lang.String-java.util.Locale-}
```
public void setPrinterName(String printerName, Locale locale)
```


Kullanılacak yazıcının adı.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| printerName | java.lang.String | Yazıcının adı. |
| yerel | java.util.Locale | printerName'in yerel ayarı. |

