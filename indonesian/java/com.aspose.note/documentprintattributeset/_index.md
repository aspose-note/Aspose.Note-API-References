---
title: "DocumentPrintAttributeSet"
second_title: "Referensi API Aspose.Note untuk Java"
description: "Mewakili kelas pembantu dengan antarmuka ramah pengguna untuk AttributeSet."
type: docs
weight: 21
url: /id/java/com.aspose.note/documentprintattributeset/
---

**Inheritance:**
java.lang.Object, javax.print.attribute.HashAttributeSet
```
public final class DocumentPrintAttributeSet extends HashAttributeSet
```

Mewakili kelas pembantu dengan antarmuka ramah pengguna untuk AttributeSet.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [DocumentPrintAttributeSet(int copies)](#DocumentPrintAttributeSet-int-) | Menginisialisasi instance baru dari `DocumentPrintAttributeSet`. |
| [DocumentPrintAttributeSet(String printerName, int copies)](#DocumentPrintAttributeSet-java.lang.String-int-) | Menginisialisasi instance baru dari `DocumentPrintAttributeSet`. |
| [DocumentPrintAttributeSet(String printerName)](#DocumentPrintAttributeSet-java.lang.String-) | Menginisialisasi instance baru dari `DocumentPrintAttributeSet`. |
| [DocumentPrintAttributeSet()](#DocumentPrintAttributeSet--) | Menginisialisasi instance baru dari `DocumentPrintAttributeSet`. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getCopies()](#getCopies--) |  |
| [getLandscape()](#getLandscape--) |  |
| [getPrinterName()](#getPrinterName--) |  |
| [setCollate(boolean value)](#setCollate-boolean-) | Mengatur nilai yang menunjukkan apakah dokumen diatur berurutan. |
| [setCopies(int value)](#setCopies-int-) | Mengatur jumlah salinan yang akan dicetak. |
| [setDuplex(boolean value)](#setDuplex-boolean-) | Mengatur pengaturan printer untuk pencetakan dua sisi. |
| [setLandscape(boolean value)](#setLandscape-boolean-) | Mengatur orientasi halaman. |
| [setPrintRange(int page)](#setPrintRange-int-) | Mengatur halaman tunggal yang akan dicetak. |
| [setPrintRange(int from, int to)](#setPrintRange-int-int-) | Mengatur rentang halaman yang akan dicetak. |
| [setPrinterName(String printerName)](#setPrinterName-java.lang.String-) | Nama printer yang akan digunakan. |
| [setPrinterName(String printerName, Locale locale)](#setPrinterName-java.lang.String-java.util.Locale-) | Nama printer yang akan digunakan. |
### DocumentPrintAttributeSet(int copies) {#DocumentPrintAttributeSet-int-}
```
public DocumentPrintAttributeSet(int copies)
```


Menginisialisasi instance baru dari `DocumentPrintAttributeSet`. Secara default semua halaman dokumen dicetak.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| salinan | int | Jumlah salinan dokumen yang akan dicetak. |

### DocumentPrintAttributeSet(String printerName, int copies) {#DocumentPrintAttributeSet-java.lang.String-int-}
```
public DocumentPrintAttributeSet(String printerName, int copies)
```


Menginisialisasi instance baru dari `DocumentPrintAttributeSet`. Secara default semua halaman dokumen dicetak.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| printerName | java.lang.String | Nama printer. |
| salinan | int | Jumlah salinan dokumen yang akan dicetak. |

### DocumentPrintAttributeSet(String printerName) {#DocumentPrintAttributeSet-java.lang.String-}
```
public DocumentPrintAttributeSet(String printerName)
```


Menginisialisasi instance baru dari `DocumentPrintAttributeSet`. Secara default hanya satu salinan setiap halaman.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| printerName | java.lang.String | Nama printer. |

### DocumentPrintAttributeSet() {#DocumentPrintAttributeSet--}
```
public DocumentPrintAttributeSet()
```


Menginisialisasi instance baru dari `DocumentPrintAttributeSet`. Secara default hanya satu salinan setiap halaman.

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


Mengatur nilai yang menunjukkan apakah dokumen diatur berurutan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | true setara dengan pengaturan SheetCollate.COLLATED false setara dengan pengaturan SheetCollate.UNCOLLATED |

### setCopies(int value) {#setCopies-int-}
```
public void setCopies(int value)
```


Mengatur jumlah salinan yang akan dicetak.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int | Jumlah salinan yang akan dicetak. |

### setDuplex(boolean value) {#setDuplex-boolean-}
```
public void setDuplex(boolean value)
```


Mengatur pengaturan printer untuk pencetakan dua sisi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | true setara dengan pengaturan Sides.DUPLEX false setara dengan pengaturan Sides.ONE\\_SIDED |

### setLandscape(boolean value) {#setLandscape-boolean-}
```
public void setLandscape(boolean value)
```


Mengatur orientasi halaman.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean | true setara dengan pengaturan OrientationRequested.LANDSCAPE false setara dengan pengaturan OrientationRequested.PORTRAIT |

### setPrintRange(int page) {#setPrintRange-int-}
```
public void setPrintRange(int page)
```


Mengatur halaman tunggal yang akan dicetak.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| halaman | int | Halaman yang akan dicetak. |

### setPrintRange(int from, int to) {#setPrintRange-int-int-}
```
public void setPrintRange(int from, int to)
```


Mengatur rentang halaman yang akan dicetak.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| dari | int | Halaman pertama. |
| ke | int | Halaman terakhir. |

### setPrinterName(String printerName) {#setPrinterName-java.lang.String-}
```
public void setPrinterName(String printerName)
```


Nama printer yang akan digunakan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| printerName | java.lang.String | Nama printer. |

### setPrinterName(String printerName, Locale locale) {#setPrinterName-java.lang.String-java.util.Locale-}
```
public void setPrinterName(String printerName, Locale locale)
```


Nama printer yang akan digunakan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| printerName | java.lang.String | Nama printer. |
| lokal | java.util.Locale | lokal printerName. |

