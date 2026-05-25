---
title: "NumberList"
second_title: "Referensi API Aspose.Note untuk Java"
description: "Mewakili daftar bernomor atau berpoin."
type: docs
weight: 64
url: /id/java/com.aspose.note/numberlist/
---

**Inheritance:**
java.lang.Object
```
public class NumberList
```

Mewakili daftar bernomor atau berpoin.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [NumberList(String bulletedSymbol, String font, int fontSize)](#NumberList-java.lang.String-java.lang.String-int-) | Menginisialisasi sebuah instance baru dari kelas `NumberList`. |
| [NumberList(String format, byte numberFormat, String font, int fontSize)](#NumberList-java.lang.String-byte-java.lang.String-int-) | Menginisialisasi sebuah instance baru dari kelas `NumberList`. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [equals(NumberList other)](#equals-com.aspose.note.NumberList-) | Menentukan apakah objek yang ditentukan sama dengan objek saat ini. |
| [equals(Object obj)](#equals-java.lang.Object-) | Menentukan apakah objek yang ditentukan sama dengan objek saat ini. |
| [getFont()](#getFont--) | Mendapatkan atau mengatur nama font. |
| [getFontColor()](#getFontColor--) | Mendapatkan atau mengatur warna font. |
| [getFontSize()](#getFontSize--) | Mendapatkan atau mengatur ukuran font. |
| [getFormat()](#getFormat--) | Mendapatkan atau mengatur format header baris. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Mendapatkan atau mengatur waktu terakhir dimodifikasi. |
| [getNumberFormat()](#getNumberFormat--) | Mendapatkan atau mengatur format nomor yang digunakan untuk sekelompok objek yang diberi nomor secara otomatis. |
| [getNumberedListHeader(int sequenceNumber)](#getNumberedListHeader-int-) | Mendapatkan header daftar bernomor. |
| [getRestart()](#getRestart--) | Mendapatkan atau mengatur nilai numerik yang menggantikan nilai nomor otomatis dari item daftar. |
| [hashCode()](#hashCode--) | Berfungsi sebagai fungsi hash untuk tipe tersebut. |
| [isBold()](#isBold--) | Mendapatkan atau mengatur nilai yang menunjukkan apakah gaya teks tebal. |
| [isItalic()](#isItalic--) | Mendapatkan atau mengatur nilai yang menunjukkan apakah gaya teks miring. |
| [setBold(boolean value)](#setBold-boolean-) | Mendapatkan atau mengatur nilai yang menunjukkan apakah gaya teks tebal. |
| [setFont(String value)](#setFont-java.lang.String-) | Mendapatkan atau mengatur nama font. |
| [setFontColor(Color value)](#setFontColor-java.awt.Color-) | Mendapatkan atau mengatur warna font. |
| [setFontSize(int value)](#setFontSize-int-) | Mendapatkan atau mengatur ukuran font. |
| [setFormat(String value)](#setFormat-java.lang.String-) | Mendapatkan atau mengatur format header baris. |
| [setItalic(boolean value)](#setItalic-boolean-) | Mendapatkan atau mengatur nilai yang menunjukkan apakah gaya teks miring. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Mendapatkan atau mengatur waktu terakhir dimodifikasi. |
| [setNumberFormat(Byte value)](#setNumberFormat-java.lang.Byte-) | Mendapatkan atau mengatur format nomor yang digunakan untuk sekelompok objek yang diberi nomor secara otomatis. |
| [setRestart(int value)](#setRestart-int-) | Mendapatkan atau mengatur nilai numerik yang menggantikan nilai nomor otomatis dari item daftar. |
### NumberList(String bulletedSymbol, String font, int fontSize) {#NumberList-java.lang.String-java.lang.String-int-}
```
public NumberList(String bulletedSymbol, String font, int fontSize)
```


Menginisialisasi sebuah instance baru dari kelas `NumberList`. Instance ini mewakili daftar berpoin.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| bulletedSymbol | java.lang.String | Sebuah simbol yang mewakili bullet. |
| font | java.lang.String | Font untuk bullet. |
| fontSize | int | Ukuran font untuk bullet. |

### NumberList(String format, byte numberFormat, String font, int fontSize) {#NumberList-java.lang.String-byte-java.lang.String-int-}
```
public NumberList(String format, byte numberFormat, String font, int fontSize)
```


Menginisialisasi sebuah instance baru dari kelas `NumberList`. Instance ini mewakili daftar bernomor.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| format | java.lang.String | Format header bernomor. |
| numberFormat | byte | Format angka di header. |
| font | java.lang.String | Font untuk header bernomor. |
| fontSize | int | Ukuran font untuk header bernomor. |

### equals(NumberList other) {#equals-com.aspose.note.NumberList-}
```
public boolean equals(NumberList other)
```


Menentukan apakah objek yang ditentukan sama dengan objek saat ini.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| other | [NumberList](../../com.aspose.note/numberlist) | Objek tersebut. |

**Returns:**
boolean - `bool`.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Menentukan apakah objek yang ditentukan sama dengan objek saat ini.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| obj | java.lang.Object | Objek tersebut. |

**Returns:**
boolean - `bool`.
### getFont() {#getFont--}
```
public String getFont()
```


Mendapatkan atau mengatur nama font.

**Returns:**
java.lang.String
### getFontColor() {#getFontColor--}
```
public Color getFontColor()
```


Mendapatkan atau mengatur warna font.

**Returns:**
java.awt.Color
### getFontSize() {#getFontSize--}
```
public int getFontSize()
```


Mendapatkan atau mengatur ukuran font.

**Returns:**
int
### getFormat() {#getFormat--}
```
public String getFormat()
```


Mendapatkan atau mengatur format header baris. Untuk daftar berpoin mewakili simbol bullet.

**Returns:**
java.lang.String
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Mendapatkan atau mengatur waktu terakhir dimodifikasi.

**Returns:**
java.util.Date
### getNumberFormat() {#getNumberFormat--}
```
public Byte getNumberFormat()
```


Mendapatkan atau mengatur format nomor yang digunakan untuk sekelompok objek yang diberi nomor secara otomatis. Harus null untuk daftar berpoin.

**Returns:**
java.lang.Byte
### getNumberedListHeader(int sequenceNumber) {#getNumberedListHeader-int-}
```
public String getNumberedListHeader(int sequenceNumber)
```


Mendapatkan header daftar bernomor.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| sequenceNumber | int | Nomor urut dalam daftar bernomor. |

**Returns:**
java.lang.String - Representasi string dari nomor urut yang ditentukan.
### getRestart() {#getRestart--}
```
public int getRestart()
```


Mendapatkan atau mengatur nilai numerik yang menggantikan nilai nomor otomatis dari item daftar.

**Returns:**
int
### hashCode() {#hashCode--}
```
public int hashCode()
```


Berfungsi sebagai fungsi hash untuk tipe tersebut.

**Returns:**
int - `int`.
### isBold() {#isBold--}
```
public boolean isBold()
```


Mendapatkan atau mengatur nilai yang menunjukkan apakah gaya teks tebal.

**Returns:**
boolean
### isItalic() {#isItalic--}
```
public boolean isItalic()
```


Mendapatkan atau mengatur nilai yang menunjukkan apakah gaya teks miring.

**Returns:**
boolean
### setBold(boolean value) {#setBold-boolean-}
```
public void setBold(boolean value)
```


Mendapatkan atau mengatur nilai yang menunjukkan apakah gaya teks tebal.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean |  |

### setFont(String value) {#setFont-java.lang.String-}
```
public void setFont(String value)
```


Mendapatkan atau mengatur nama font.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String |  |

### setFontColor(Color value) {#setFontColor-java.awt.Color-}
```
public void setFontColor(Color value)
```


Mendapatkan atau mengatur warna font.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.awt.Color |  |

### setFontSize(int value) {#setFontSize-int-}
```
public void setFontSize(int value)
```


Mendapatkan atau mengatur ukuran font.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int |  |

### setFormat(String value) {#setFormat-java.lang.String-}
```
public void setFormat(String value)
```


Mendapatkan atau mengatur format header baris. Untuk daftar berpoin mewakili simbol bullet.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String |  |

### setItalic(boolean value) {#setItalic-boolean-}
```
public void setItalic(boolean value)
```


Mendapatkan atau mengatur nilai yang menunjukkan apakah gaya teks miring.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | boolean |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Mendapatkan atau mengatur waktu terakhir dimodifikasi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.util.Date |  |

### setNumberFormat(Byte value) {#setNumberFormat-java.lang.Byte-}
```
public void setNumberFormat(Byte value)
```


Mendapatkan atau mengatur format nomor yang digunakan untuk sekelompok objek yang diberi nomor secara otomatis. Harus null untuk daftar berpoin.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.Byte |  |

### setRestart(int value) {#setRestart-int-}
```
public void setRestart(int value)
```


Mendapatkan atau mengatur nilai numerik yang menggantikan nilai nomor otomatis dari item daftar.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | int |  |

