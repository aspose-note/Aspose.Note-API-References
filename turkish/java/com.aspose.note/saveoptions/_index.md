---
title: "SaveOptions"
second_title: "Aspose.Note for Java API Referansı"
description: "Belirli bir format için belge kaydetme seçeneklerini temsil eden soyut bir temel sınıf."
type: docs
weight: 85
url: /tr/java/com.aspose.note/saveoptions/
---

**Inheritance:**
java.lang.Object
```
public abstract class SaveOptions
```

Belirli bir format için belge kaydetme seçeneklerini temsil eden soyut bir temel sınıf.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getFontsSubsystem()](#getFontsSubsystem--) | Kaydetme sırasında kullanılacak yazı tipi ayarlarını alır veya ayarlar. |
| [getPageCount()](#getPageCount--) | Kaydedilecek sayfa sayısını alır veya ayarlar. |
| [getPageIndex()](#getPageIndex--) | Kaydedilecek ilk sayfanın dizinini alır veya ayarlar. |
| [getSaveFormat()](#getSaveFormat--) | Belgenin kaydedileceği formatı alır veya ayarlar. |
| [setFontsSubsystem(FontsSubsystem value)](#setFontsSubsystem-com.aspose.note.fonts.FontsSubsystem-) | Kaydetme sırasında kullanılacak yazı tipi ayarlarını alır veya ayarlar. |
| [setPageCount(int value)](#setPageCount-int-) | Kaydedilecek sayfa sayısını alır veya ayarlar. |
| [setPageIndex(int value)](#setPageIndex-int-) | Kaydedilecek ilk sayfanın dizinini alır veya ayarlar. |
### getFontsSubsystem() {#getFontsSubsystem--}
```
public final FontsSubsystem getFontsSubsystem()
```


Kaydetme sırasında kullanılacak yazı tipi ayarlarını alır veya ayarlar.

**Returns:**
[FontsSubsystem](../../com.aspose.note.fonts/fontssubsystem)
### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


Kaydedilecek sayfa sayısını alır veya ayarlar. Varsayılan olarak \{@link int\#Int32Extensions.MaxValue\} olup, bu belgenin tüm sayfalarının işleneceği anlamına gelir.

**Returns:**
int
### getPageIndex() {#getPageIndex--}
```
public final int getPageIndex()
```


Kaydedilecek ilk sayfanın dizinini alır veya ayarlar. Varsayılan değer 0'dır.

**Returns:**
int
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Belgenin kaydedileceği formatı alır veya ayarlar.

**Returns:**
int
### setFontsSubsystem(FontsSubsystem value) {#setFontsSubsystem-com.aspose.note.fonts.FontsSubsystem-}
```
public final void setFontsSubsystem(FontsSubsystem value)
```


Kaydetme sırasında kullanılacak yazı tipi ayarlarını alır veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [FontsSubsystem](../../com.aspose.note.fonts/fontssubsystem) |  |

### setPageCount(int value) {#setPageCount-int-}
```
public final void setPageCount(int value)
```


Kaydedilecek sayfa sayısını alır veya ayarlar. Varsayılan olarak \{@link int\#Int32Extensions.MaxValue\} olup, bu belgenin tüm sayfalarının işleneceği anlamına gelir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setPageIndex(int value) {#setPageIndex-int-}
```
public final void setPageIndex(int value)
```


Kaydedilecek ilk sayfanın dizinini alır veya ayarlar. Varsayılan değer 0'dır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

