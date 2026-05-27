---
title: "RichText"
second_title: "Aspose.Note for Java API Referansı"
description: "Zengin metni temsil eder."
type: docs
weight: 82
url: /tr/java/com.aspose.note/richtext/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node)

**All Implemented Interfaces:**
[com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode), [com.aspose.note.ITaggable](../../com.aspose.note/itaggable), com.aspose.ms.System.Collections.Generic.IGenericEnumerable
```
public class RichText extends Node implements IOutlineElementChildNode, ITaggable, System.Collections.Generic.IGenericEnumerable<Character>
```

Zengin metni temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [RichText()](#RichText--) | [RichText](../../com.aspose.note/richtext) sınıfının yeni bir örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Düğümün ziyaretçisini kabul eder. |
| [append(String value)](#append-java.lang.String-) | Son metin aralığına bir dize ekler. |
| [append(String value, TextStyle style)](#append-java.lang.String-com.aspose.note.TextStyle-) | Bir dizeyi sona ekler. |
| [appendFront(String value)](#appendFront-java.lang.String-) | Bir dizeyi ilk metin aralığının önüne ekler. |
| [appendFront(String value, TextStyle style)](#appendFront-java.lang.String-com.aspose.note.TextStyle-) | Bir dizeyi önüne ekler. |
| [clear()](#clear--) | Bu örneğin içeriğini temizler. |
| [getAlignment()](#getAlignment--) | Hizalamayı alır. |
| [getLastModifiedTime()](#getLastModifiedTime--) | Son değiştirilme zamanını alır. |
| [getLength()](#getLength--) |  |
| [getLineSpacing()](#getLineSpacing--) | Satır aralığını alır. |
| [getParagraphStyle()](#getParagraphStyle--) | Paragraf stilini alır. |
| [getSpaceAfter()](#getSpaceAfter--) | Sonrasındaki minimum boşluk miktarını alır. |
| [getSpaceBefore()](#getSpaceBefore--) | Öncesindeki minimum boşluk miktarını alır. |
| [getStyles()](#getStyles--) | Stilleri alır. |
| [getTags()](#getTags--) | Bir paragrafın tüm etiketlerinin listesini alır. |
| [getText()](#getText--) | Metni alır. |
| [getTextRuns()](#getTextRuns--) |  |
| [indexOf(char value)](#indexOf-char-) | Bu dizede belirtilen Unicode karakterinin ilk oluşumunun sıfır tabanlı dizinini döndürür. |
| [indexOf(char value, int startIndex)](#indexOf-char-int-) | Bu dizede belirtilen Unicode karakterinin ilk oluşumunun sıfır tabanlı dizinini döndürür. |
| [indexOf(char value, int startIndex, int count)](#indexOf-char-int-int-) | Bu örnekte belirtilen karakterin ilk oluşumunun sıfır tabanlı dizinini döndürür. |
| [indexOf(String value)](#indexOf-java.lang.String-) | Bu örnekte belirtilen dizenin ilk oluşumunun sıfır tabanlı dizinini döndürür. |
| [indexOf(String value, int startIndex)](#indexOf-java.lang.String-int-) | Bu örnekte belirtilen dizenin ilk oluşumunun sıfır tabanlı dizinini döndürür. |
| [indexOf(String value, int startIndex, int count)](#indexOf-java.lang.String-int-int-) | Bu örnekte belirtilen dizenin ilk oluşumunun sıfır tabanlı dizinini döndürür. |
| [indexOf(String value, int startIndex, int count, short comparisonType)](#indexOf-java.lang.String-int-int-short-) | Mevcut örnekte belirtilen dizenin ilk oluşumunun sıfır tabanlı dizinini döndürür. |
| [indexOf(String value, short comparisonType)](#indexOf-java.lang.String-short-) | Mevcut örnekte belirtilen dizenin ilk oluşumunun sıfır tabanlı dizinini döndürür. |
| [indexOf_Rename_Namesake(String value, int startIndex, short comparisonType)](#indexOf-Rename-Namesake-java.lang.String-int-short-) | Mevcut örnekte belirtilen dizenin ilk oluşumunun sıfır tabanlı dizinini döndürür. |
| [insert(int startIndex, String value)](#insert-int-java.lang.String-) | Bu örnekte belirtilen bir diziyi belirtilen indeks konumuna ekler. |
| [insert(int startIndex, String value, TextStyle style)](#insert-int-java.lang.String-com.aspose.note.TextStyle-) | Bu örnekte belirtilen bir diziyi belirtilen stil ile belirtilen indeks konumuna ekler. |
| [iterator()](#iterator--) |  |
| [remove(int startIndex)](#remove-int-) | Mevcut örnekteki tüm karakterleri, belirtilen konumdan başlayarak son konuma kadar kaldırır. |
| [remove(int startIndex, int count)](#remove-int-int-) | Mevcut örnekte belirtilen konumdan başlayarak belirtilen sayıda karakteri kaldırır. |
| [replace(char oldChar, char newChar)](#replace-char-char-) | Bu örnekte belirtilen bir Unicode karakterinin tüm oluşumlarını başka bir belirtilen Unicode karakteriyle değiştirir. |
| [replace(String oldValue, String newValue)](#replace-java.lang.String-java.lang.String-) | Mevcut örnekte belirtilen bir dizenin tüm oluşumlarını başka bir belirtilen dizeyle değiştirir. |
| [replace(String oldValue, String newValue, TextStyle style)](#replace-java.lang.String-java.lang.String-com.aspose.note.TextStyle-) | Mevcut örnekte belirtilen bir dizenin tüm oluşumlarını belirtilen stil içinde başka bir belirtilen dizeyle değiştirir. |
| [setAlignment(int value)](#setAlignment-int-) | Hizalamayı ayarlar. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | Son değiştirilme zamanını ayarlar. |
| [setLineSpacing(float value)](#setLineSpacing-float-) |  |
| [setLineSpacing(Float value)](#setLineSpacing-java.lang.Float-) | Satır aralığını ayarlar. |
| [setParagraphStyle(ParagraphStyle value)](#setParagraphStyle-com.aspose.note.ParagraphStyle-) | Paragraf stilini ayarlar. |
| [setSpaceAfter(float value)](#setSpaceAfter-float-) |  |
| [setSpaceAfter(Float value)](#setSpaceAfter-java.lang.Float-) | Sonrasındaki minimum boşluk miktarını ayarlar. |
| [setSpaceBefore(float value)](#setSpaceBefore-float-) |  |
| [setSpaceBefore(Float value)](#setSpaceBefore-java.lang.Float-) | Öncesindeki minimum boşluk miktarını ayarlar. |
| [setText(String value)](#setText-java.lang.String-) | Metni ayarlar. |
| [trim()](#trim--) | Baş ve sondaki tüm boşluk karakterlerini kaldırır. |
| [trim(char trimChar)](#trim-char-) | Bir karakterin baş ve sondaki tüm örneklerini kaldırır. |
| [trim(char[] trimChars)](#trim-char...-) | Dizide belirtilen bir karakter kümesinin baş ve sondaki tüm oluşumlarını kaldırır. |
| [trimEnd()](#trimEnd--) | Sondaki tüm boşluk karakterlerini kaldırır. |
| [trimEnd(char trimChar)](#trimEnd-char-) | Bir karakterin sondaki tüm oluşumlarını kaldırır. |
| [trimEnd(char[] trimChars)](#trimEnd-char...-) | Dizide belirtilen bir karakter kümesinin sondaki tüm oluşumlarını kaldırır. |
| [trimStart()](#trimStart--) | Başdaki tüm boşluk karakterlerini kaldırır. |
| [trimStart(char trimChar)](#trimStart-char-) | Belirtilen bir karakterin başdaki tüm oluşumlarını kaldırır. |
| [trimStart(char[] trimChars)](#trimStart-char...-) | Dizide belirtilen bir karakter kümesinin başdaki tüm oluşumlarını kaldırır. |
### RichText() {#RichText--}
```
public RichText()
```


[RichText](../../com.aspose.note/richtext) sınıfının yeni bir örneğini başlatır.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Düğümün ziyaretçisini kabul eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | [DocumentVisitor](../../com.aspose.note/documentvisitor) sınıfından türetilen bir sınıfın nesnesi. |

### append(String value) {#append-java.lang.String-}
```
public RichText append(String value)
```


Son metin aralığına bir dize ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | Eklenen değer. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### append(String value, TextStyle style) {#append-java.lang.String-com.aspose.note.TextStyle-}
```
public final RichText append(String value, TextStyle style)
```


Bir dizeyi sona ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | Eklenen değer. |
| style | [TextStyle](../../com.aspose.note/textstyle) | Eklenen dize stilı. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### appendFront(String value) {#appendFront-java.lang.String-}
```
public RichText appendFront(String value)
```


Bir dizeyi ilk metin aralığının önüne ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | Eklenen değer. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### appendFront(String value, TextStyle style) {#appendFront-java.lang.String-com.aspose.note.TextStyle-}
```
public RichText appendFront(String value, TextStyle style)
```


Bir dizeyi önüne ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | Eklenen değer. |
| style | [TextStyle](../../com.aspose.note/textstyle) | Eklenen dize stilı. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### clear() {#clear--}
```
public final RichText clear()
```


Bu örneğin içeriğini temizler.

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### getAlignment() {#getAlignment--}
```
public int getAlignment()
```


Hizalamayı alır.

**Returns:**
int
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


Son değiştirilme zamanını alır.

**Returns:**
java.util.Date
### getLength() {#getLength--}
```
public final int getLength()
```




**Returns:**
int
### getLineSpacing() {#getLineSpacing--}
```
public Float getLineSpacing()
```


Satır aralığını alır.

**Returns:**
java.lang.Float
### getParagraphStyle() {#getParagraphStyle--}
```
public final ParagraphStyle getParagraphStyle()
```


Paragraf stilini alır. Bu ayarlar, [getStyles](../../com.aspose.note/richtext\#getStyles) koleksiyonunda eşleşen bir TextStyle nesnesi yoksa veya bu nesne gerekli ayarı belirtmezse kullanılır.

**Returns:**
[ParagraphStyle](../../com.aspose.note/paragraphstyle)
### getSpaceAfter() {#getSpaceAfter--}
```
public Float getSpaceAfter()
```


Sonrasındaki minimum boşluk miktarını alır.

**Returns:**
java.lang.Float
### getSpaceBefore() {#getSpaceBefore--}
```
public Float getSpaceBefore()
```


Öncesindeki minimum boşluk miktarını alır.

**Returns:**
java.lang.Float
### getStyles() {#getStyles--}
```
public System.Collections.Generic.IGenericEnumerable<TextStyle> getStyles()
```


Stilleri alır.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerable&lt;com.aspose.note.TextStyle&gt;
### getTags() {#getTags--}
```
public final System.Collections.Generic.List<ITag> getTags()
```


Bir paragrafın tüm etiketlerinin listesini alır.

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.note.ITag&gt;
### getText() {#getText--}
```
public final String getText()
```


Metni alır. Dize, değer 10 (satır beslemesi) olan herhangi bir karakter içermemelidir.

**Returns:**
java.lang.String
### getTextRuns() {#getTextRuns--}
```
public final System.Collections.Generic.IGenericEnumerable<TextRun> getTextRuns()
```




**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerable&lt;com.aspose.note.TextRun&gt;
### indexOf(char value) {#indexOf-char-}
```
public final int indexOf(char value)
```


Bu dizede belirtilen Unicode karakterinin ilk oluşumunun sıfır tabanlı dizinini döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | char | Değer. |

**Returns:**
int - Bu `int`.
### indexOf(char value, int startIndex) {#indexOf-char-int-}
```
public final int indexOf(char value, int startIndex)
```


Bu dizede belirtilen Unicode karakterinin ilk oluşumunun sıfır tabanlı indeksini döndürür. Arama, belirtilen bir karakter konumunda başlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | char | Değer. |
| startIndex | int | Aramanın başlangıç konumu |

**Returns:**
int - Bu `int`.
### indexOf(char value, int startIndex, int count) {#indexOf-char-int-int-}
```
public final int indexOf(char value, int startIndex, int count)
```


Bu örnekte belirtilen karakterin ilk oluşumunun sıfır tabanlı indeksini döndürür. Arama, belirtilen bir karakter konumunda başlar ve belirtilen sayıda karakter konumunu inceler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | char | Değer. |
| startIndex | int | Aramanın başlangıç konumu |
| count | int | Sayım. |

**Returns:**
int - Bu `int`.
### indexOf(String value) {#indexOf-java.lang.String-}
```
public final int indexOf(String value)
```


Bu örnekte belirtilen dizenin ilk oluşumunun sıfır tabanlı dizinini döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | Değer. |

**Returns:**
int - Bu `int`.
### indexOf(String value, int startIndex) {#indexOf-java.lang.String-int-}
```
public final int indexOf(String value, int startIndex)
```


Bu örnekte belirtilen dizeyin ilk oluşumunun sıfır tabanlı indeksini döndürür. Arama, belirtilen bir karakter konumundan başlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | Değer. |
| startIndex | int | Aramanın başlangıç konumu |

**Returns:**
int - Bu `int`.
### indexOf(String value, int startIndex, int count) {#indexOf-java.lang.String-int-int-}
```
public final int indexOf(String value, int startIndex, int count)
```


Bu örnekte belirtilen dizeyin ilk oluşumunun sıfır tabanlı indeksini döndürür. Arama, belirtilen bir karakter konumundan başlar ve belirtilen sayıda karakter konumunu inceler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | Değer. |
| startIndex | int | Aramanın başlangıç konumu |
| count | int | Sayım. |

**Returns:**
int - Bu `int`.
### indexOf(String value, int startIndex, int count, short comparisonType) {#indexOf-java.lang.String-int-int-short-}
```
public final int indexOf(String value, int startIndex, int count, short comparisonType)
```


Mevcut örnekte belirtilen dizenin ilk oluşumunun sıfır tabanlı dizinini döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | Değer. |
| startIndex | int | Aramanın başlangıç konumu |
| count | int | Sayım. |
| comparisonType | short | Belirtilen dize için kullanılacak arama türü |

**Returns:**
int - Bu `int`.
### indexOf(String value, short comparisonType) {#indexOf-java.lang.String-short-}
```
public final int indexOf(String value, short comparisonType)
```


Mevcut örnekte belirtilen dizeyin ilk oluşumunun sıfır tabanlı indeksini döndürür. Bir parametre, belirtilen dize için kullanılacak arama türünü belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | Değer. |
| comparisonType | short | Belirtilen dize için kullanılacak arama türü |

**Returns:**
int - Bu `int`.
### indexOf_Rename_Namesake(String value, int startIndex, short comparisonType) {#indexOf-Rename-Namesake-java.lang.String-int-short-}
```
public final int indexOf_Rename_Namesake(String value, int startIndex, short comparisonType)
```


Mevcut örnekte belirtilen dizeyin ilk oluşumunun sıfır tabanlı indeksini döndürür. Parametreler, mevcut dizedeki arama başlangıç konumunu ve belirtilen dize için kullanılacak arama türünü belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | Değer. |
| startIndex | int | Aramanın başlangıç konumu |
| comparisonType | short | Belirtilen dize için kullanılacak arama türü |

**Returns:**
int - Bu `int`.
### insert(int startIndex, String value) {#insert-int-java.lang.String-}
```
public final RichText insert(int startIndex, String value)
```


Bu örnekte belirtilen bir diziyi belirtilen indeks konumuna ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startIndex | int | Başlangıç indeksi. |
| değer | java.lang.String | Değer. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### insert(int startIndex, String value, TextStyle style) {#insert-int-java.lang.String-com.aspose.note.TextStyle-}
```
public final RichText insert(int startIndex, String value, TextStyle style)
```


Bu örnekte belirtilen bir diziyi belirtilen stil ile belirtilen indeks konumuna ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startIndex | int | Başlangıç indeksi. |
| değer | java.lang.String | Değer. |
| style | [TextStyle](../../com.aspose.note/textstyle) | Stil. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<Character> iterator()
```




**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;java.lang.Character&gt;
### remove(int startIndex) {#remove-int-}
```
public final RichText remove(int startIndex)
```


Mevcut örnekteki tüm karakterleri, belirtilen konumdan başlayarak son konuma kadar kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startIndex | int | Başlangıç indeksi. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### remove(int startIndex, int count) {#remove-int-int-}
```
public final RichText remove(int startIndex, int count)
```


Mevcut örnekte belirtilen konumdan başlayarak belirtilen sayıda karakteri kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startIndex | int | Başlangıç indeksi. |
| count | int | Sayım. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### replace(char oldChar, char newChar) {#replace-char-char-}
```
public final RichText replace(char oldChar, char newChar)
```


Bu örnekte belirtilen bir Unicode karakterinin tüm oluşumlarını başka bir belirtilen Unicode karakteriyle değiştirir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| oldChar | char | Eski karakter. |
| newChar | char | Yeni karakter. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### replace(String oldValue, String newValue) {#replace-java.lang.String-java.lang.String-}
```
public final RichText replace(String oldValue, String newValue)
```


Mevcut örnekte belirtilen bir dizenin tüm oluşumlarını başka bir belirtilen dizeyle değiştirir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| oldValue | java.lang.String | Eski değer. |
| newValue | java.lang.String | Yeni değer. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### replace(String oldValue, String newValue, TextStyle style) {#replace-java.lang.String-java.lang.String-com.aspose.note.TextStyle-}
```
public final RichText replace(String oldValue, String newValue, TextStyle style)
```


Mevcut örnekte belirtilen bir dizenin tüm oluşumlarını belirtilen stil içinde başka bir belirtilen dizeyle değiştirir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| oldValue | java.lang.String | Eski değer. |
| newValue | java.lang.String | Yeni değer. |
| style | [TextStyle](../../com.aspose.note/textstyle) | Yeni değerin stili. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### setAlignment(int value) {#setAlignment-int-}
```
public void setAlignment(int value)
```


Hizalamayı ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


Son değiştirilme zamanını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.Date |  |

### setLineSpacing(float value) {#setLineSpacing-float-}
```
public void setLineSpacing(float value)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | float |  |

### setLineSpacing(Float value) {#setLineSpacing-java.lang.Float-}
```
public void setLineSpacing(Float value)
```


Satır aralığını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.Float |  |

### setParagraphStyle(ParagraphStyle value) {#setParagraphStyle-com.aspose.note.ParagraphStyle-}
```
public final void setParagraphStyle(ParagraphStyle value)
```


Paragraf stilini ayarlar. Bu ayarlar, [getStyles](../../com.aspose.note/richtext\#getStyles) koleksiyonunda eşleşen bir TextStyle nesnesi bulunmadığında veya bu nesne gerekli bir ayarı belirtmediğinde kullanılır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [ParagraphStyle](../../com.aspose.note/paragraphstyle) |  |

### setSpaceAfter(float value) {#setSpaceAfter-float-}
```
public void setSpaceAfter(float value)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | float |  |

### setSpaceAfter(Float value) {#setSpaceAfter-java.lang.Float-}
```
public void setSpaceAfter(Float value)
```


Sonrasındaki minimum boşluk miktarını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.Float |  |

### setSpaceBefore(float value) {#setSpaceBefore-float-}
```
public void setSpaceBefore(float value)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | float |  |

### setSpaceBefore(Float value) {#setSpaceBefore-java.lang.Float-}
```
public void setSpaceBefore(Float value)
```


Öncesindeki minimum boşluk miktarını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.Float |  |

### setText(String value) {#setText-java.lang.String-}
```
public final void setText(String value)
```


Metni ayarlar. Dize, değer 10 (satır beslemesi) olan hiçbir karakter içermemelidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### trim() {#trim--}
```
public final RichText trim()
```


Baş ve sondaki tüm boşluk karakterlerini kaldırır.

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trim(char trimChar) {#trim-char-}
```
public final RichText trim(char trimChar)
```


Bir karakterin baş ve sondaki tüm örneklerini kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| trimChar | char | Kırpma karakteri. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trim(char[] trimChars) {#trim-char...-}
```
public final RichText trim(char[] trimChars)
```


Dizide belirtilen bir karakter kümesinin baş ve sondaki tüm oluşumlarını kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| trimChars | char[] | Kesme karakterleri. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimEnd() {#trimEnd--}
```
public final RichText trimEnd()
```


Sondaki tüm boşluk karakterlerini kaldırır.

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimEnd(char trimChar) {#trimEnd-char-}
```
public final RichText trimEnd(char trimChar)
```


Bir karakterin sondaki tüm oluşumlarını kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| trimChar | char | Kırpma karakteri. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimEnd(char[] trimChars) {#trimEnd-char...-}
```
public final RichText trimEnd(char[] trimChars)
```


Dizide belirtilen bir karakter kümesinin sondaki tüm oluşumlarını kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| trimChars | char[] | Kesme karakterleri. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimStart() {#trimStart--}
```
public final RichText trimStart()
```


Başdaki tüm boşluk karakterlerini kaldırır.

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimStart(char trimChar) {#trimStart-char-}
```
public final RichText trimStart(char trimChar)
```


Belirtilen bir karakterin başdaki tüm oluşumlarını kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| trimChar | char | Kırpma karakteri. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimStart(char[] trimChars) {#trimStart-char...-}
```
public final RichText trimStart(char[] trimChars)
```


Dizide belirtilen bir karakter kümesinin başdaki tüm oluşumlarını kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| trimChars | char[] | Kesme karakterleri. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
