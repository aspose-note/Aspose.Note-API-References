---
title: "NumberList"
second_title: "Aspose.Note for Java API Referansı"
description: "Numaralı veya madde işaretli listeyi temsil eder."
type: docs
weight: 64
url: /tr/java/com.aspose.note/numberlist/
---

**Inheritance:**
java.lang.Object
```
public class NumberList
```

Numaralı veya madde işaretli listeyi temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [NumberList(String bulletedSymbol, String font, int fontSize)](#NumberList-java.lang.String-java.lang.String-int-) | Yeni bir `NumberList` sınıfı örneği başlatır. |
| [NumberList(String format, byte numberFormat, String font, int fontSize)](#NumberList-java.lang.String-byte-java.lang.String-int-) | Yeni bir `NumberList` sınıfı örneği başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(NumberList other)](#equals-com.aspose.note.NumberList-) | Belirtilen nesnenin mevcut nesneye eşit olup olmadığını belirler. |
| [equals(Object obj)](#equals-java.lang.Object-) | Belirtilen nesnenin mevcut nesneye eşit olup olmadığını belirler. |
| [getFont()](#getFont--) | Yazı tipinin adını alır veya ayarlar. |
| [getFontColor()](#getFontColor--) | Yazı tipi rengini alır veya ayarlar. |
| [getFontSize()](#getFontSize--) | Yazı tipi boyutunu alır veya ayarlar. |
| [getFormat()](#getFormat--) | Satır başlığının biçimini alır veya ayarlar. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Son değiştirilme zamanının değerini alır veya ayarlar. |
| [getNumberFormat()](#getNumberFormat--) | Otomatik numaralandırılmış nesneler grubunda kullanılan sayı biçimini alır veya ayarlar. |
| [getNumberedListHeader(int sequenceNumber)](#getNumberedListHeader-int-) | Numaralı liste başlığını alır. |
| [getRestart()](#getRestart--) | Liste öğesinin otomatik sayı değerini geçersiz kılan sayısal değeri alır veya ayarlar. |
| [hashCode()](#hashCode--) | Tür için bir karma işlevi olarak hizmet verir. |
| [isBold()](#isBold--) | Metin stilinin kalın olup olmadığını belirten bir değeri alır veya ayarlar. |
| [isItalic()](#isItalic--) | Metin stilinin italik olup olmadığını belirten bir değeri alır veya ayarlar. |
| [setBold(boolean value)](#setBold-boolean-) | Metin stilinin kalın olup olmadığını belirten bir değeri alır veya ayarlar. |
| [setFont(String value)](#setFont-java.lang.String-) | Yazı tipinin adını alır veya ayarlar. |
| [setFontColor(Color value)](#setFontColor-java.awt.Color-) | Yazı tipi rengini alır veya ayarlar. |
| [setFontSize(int value)](#setFontSize-int-) | Yazı tipi boyutunu alır veya ayarlar. |
| [setFormat(String value)](#setFormat-java.lang.String-) | Satır başlığının biçimini alır veya ayarlar. |
| [setItalic(boolean value)](#setItalic-boolean-) | Metin stilinin italik olup olmadığını belirten bir değeri alır veya ayarlar. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Son değiştirilme zamanının değerini alır veya ayarlar. |
| [setNumberFormat(Byte value)](#setNumberFormat-java.lang.Byte-) | Otomatik numaralandırılmış nesneler grubunda kullanılan sayı biçimini alır veya ayarlar. |
| [setRestart(int value)](#setRestart-int-) | Liste öğesinin otomatik sayı değerini geçersiz kılan sayısal değeri alır veya ayarlar. |
### NumberList(String bulletedSymbol, String font, int fontSize) {#NumberList-java.lang.String-java.lang.String-int-}
```
public NumberList(String bulletedSymbol, String font, int fontSize)
```


Yeni bir `NumberList` sınıfı örneği başlatır. Bu örnek işaretli bir listeyi temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| bulletedSymbol | java.lang.String | Bir madde işaretini temsil eden simge. |
| font | java.lang.String | Madde işareti için bir yazı tipi. |
| fontSize | int | Madde işareti için bir yazı tipi boyutu. |

### NumberList(String format, byte numberFormat, String font, int fontSize) {#NumberList-java.lang.String-byte-java.lang.String-int-}
```
public NumberList(String format, byte numberFormat, String font, int fontSize)
```


Yeni bir `NumberList` sınıfı örneği başlatır. Bu örnek numaralı bir listeyi temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| format | java.lang.String | Numaralı başlığın biçimi. |
| numberFormat | byte | Başlıkta sayının biçimi. |
| font | java.lang.String | Numaralı başlık için bir yazı tipi. |
| fontSize | int | Numaralı başlık için bir yazı tipi boyutu. |

### equals(NumberList other) {#equals-com.aspose.note.NumberList-}
```
public boolean equals(NumberList other)
```


Belirtilen nesnenin mevcut nesneye eşit olup olmadığını belirler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| other | [NumberList](../../com.aspose.note/numberlist) | Nesne. |

**Returns:**
boolean - Bu `bool`.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Belirtilen nesnenin mevcut nesneye eşit olup olmadığını belirler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| obj | java.lang.Object | Nesne. |

**Returns:**
boolean - Bu `bool`.
### getFont() {#getFont--}
```
public String getFont()
```


Yazı tipinin adını alır veya ayarlar.

**Returns:**
java.lang.String
### getFontColor() {#getFontColor--}
```
public Color getFontColor()
```


Yazı tipi rengini alır veya ayarlar.

**Returns:**
java.awt.Color
### getFontSize() {#getFontSize--}
```
public int getFontSize()
```


Yazı tipi boyutunu alır veya ayarlar.

**Returns:**
int
### getFormat() {#getFormat--}
```
public String getFormat()
```


Satır başlığının biçimini alır veya ayarlar. Madde işaretli listeler için bir madde işareti simgesi temsil eder.

**Returns:**
java.lang.String
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Son değiştirilme zamanının değerini alır veya ayarlar.

**Returns:**
java.util.Date
### getNumberFormat() {#getNumberFormat--}
```
public Byte getNumberFormat()
```


Otomatik numaralandırılmış nesneler grubunda kullanılan sayı biçimini alır veya ayarlar. Madde işaretli listeler için null olmalıdır.

**Returns:**
java.lang.Byte
### getNumberedListHeader(int sequenceNumber) {#getNumberedListHeader-int-}
```
public String getNumberedListHeader(int sequenceNumber)
```


Numaralı liste başlığını alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sequenceNumber | int | Numaralı listedeki sıra numarası. |

**Returns:**
java.lang.String - Belirtilen sıra numarasının dize temsili.
### getRestart() {#getRestart--}
```
public int getRestart()
```


Liste öğesinin otomatik sayı değerini geçersiz kılan sayısal değeri alır veya ayarlar.

**Returns:**
int
### hashCode() {#hashCode--}
```
public int hashCode()
```


Tür için bir karma işlevi olarak hizmet verir.

**Returns:**
int - Bu `int`.
### isBold() {#isBold--}
```
public boolean isBold()
```


Metin stilinin kalın olup olmadığını belirten bir değeri alır veya ayarlar.

**Returns:**
boolean
### isItalic() {#isItalic--}
```
public boolean isItalic()
```


Metin stilinin italik olup olmadığını belirten bir değeri alır veya ayarlar.

**Returns:**
boolean
### setBold(boolean value) {#setBold-boolean-}
```
public void setBold(boolean value)
```


Metin stilinin kalın olup olmadığını belirten bir değeri alır veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setFont(String value) {#setFont-java.lang.String-}
```
public void setFont(String value)
```


Yazı tipinin adını alır veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setFontColor(Color value) {#setFontColor-java.awt.Color-}
```
public void setFontColor(Color value)
```


Yazı tipi rengini alır veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.awt.Color |  |

### setFontSize(int value) {#setFontSize-int-}
```
public void setFontSize(int value)
```


Yazı tipi boyutunu alır veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setFormat(String value) {#setFormat-java.lang.String-}
```
public void setFormat(String value)
```


Satır başlığının biçimini alır veya ayarlar. Madde işaretli listeler için bir madde işareti simgesi temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setItalic(boolean value) {#setItalic-boolean-}
```
public void setItalic(boolean value)
```


Metin stilinin italik olup olmadığını belirten bir değeri alır veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Son değiştirilme zamanının değerini alır veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.Date |  |

### setNumberFormat(Byte value) {#setNumberFormat-java.lang.Byte-}
```
public void setNumberFormat(Byte value)
```


Otomatik numaralandırılmış nesneler grubunda kullanılan sayı biçimini alır veya ayarlar. Madde işaretli listeler için null olmalıdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.Byte |  |

### setRestart(int value) {#setRestart-int-}
```
public void setRestart(int value)
```


Liste öğesinin otomatik sayı değerini geçersiz kılan sayısal değeri alır veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

