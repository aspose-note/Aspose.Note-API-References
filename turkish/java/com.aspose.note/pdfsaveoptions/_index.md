---
title: "PdfSaveOptions"
second_title: "Aspose.Note for Java API Referansı"
description: "Belge sayfalarını PDF'ye render ederken ek seçenekler belirtmeye izin verir."
type: docs
weight: 77
url: /tr/java/com.aspose.note/pdfsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.SaveOptions](../../com.aspose.note/saveoptions)
```
public final class PdfSaveOptions extends SaveOptions
```

Belge sayfalarını PDF'ye render ederken ek seçenekler belirtmeye izin verir.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [PdfSaveOptions()](#PdfSaveOptions--) | Yeni bir `PdfSaveOptions` sınıfının örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getImageCompression()](#getImageCompression--) | PDF dosyasındaki görüntülere uygulanan sıkıştırma türünü alır. |
| [getJpegQuality()](#getJpegQuality--) | PDF belgesi içindeki JPEG görüntülerinin kalitesini belirleyen bir değeri alır. |
| [getPageSettings()](#getPageSettings--) | Belgedeki her sayfa için sayfa ayarlarını alır veya ayarlar. |
| [getPageSplittingAlgorithm()](#getPageSplittingAlgorithm--) | Sayfa bölme için kullanılan algoritmayı alır veya ayarlar. |
| [setImageCompression(int value)](#setImageCompression-int-) | PDF dosyasındaki görüntülere uygulanan sıkıştırma türünü ayarlar. |
| [setJpegQuality(int value)](#setJpegQuality-int-) | PDF belgesi içindeki JPEG görüntülerinin kalitesini belirleyen bir değeri ayarlar. |
| [setPageSettings(PageSettings value)](#setPageSettings-com.aspose.note.PageSettings-) | Belgedeki her sayfa için sayfa ayarlarını alır veya ayarlar. |
| [setPageSplittingAlgorithm(PageSplittingAlgorithm value)](#setPageSplittingAlgorithm-com.aspose.note.PageSplittingAlgorithm-) | Sayfa bölme için kullanılan algoritmayı alır veya ayarlar. |
### PdfSaveOptions() {#PdfSaveOptions--}
```
public PdfSaveOptions()
```


Yeni bir `PdfSaveOptions` sınıfının örneğini başlatır.

### getImageCompression() {#getImageCompression--}
```
public final int getImageCompression()
```


PDF dosyasındaki görüntülere uygulanan sıkıştırma türünü alır.

**Returns:**
int
### getJpegQuality() {#getJpegQuality--}
```
public final int getJpegQuality()
```


PDF belgesi içindeki JPEG görüntülerinin kalitesini belirleyen bir değeri alır. Değer 0 ile 100 arasında değişebilir; 0 en düşük kaliteyi ancak maksimum sıkıştırmayı, 100 ise en yüksek kaliteyi ancak minimum sıkıştırmayı ifade eder.

--------------------

Varsayılan değer 90'dır.

**Returns:**
int
### getPageSettings() {#getPageSettings--}
```
public PageSettings getPageSettings()
```


Belgedeki her sayfa için sayfa ayarlarını alır veya ayarlar. Varsayılan olarak CurrentUICulture'a bağlıdır, \*US kültürleri letter ayarına, diğerleri A4 ayarına sahiptir.

**Returns:**
[PageSettings](../../com.aspose.note/pagesettings)
### getPageSplittingAlgorithm() {#getPageSplittingAlgorithm--}
```
public PageSplittingAlgorithm getPageSplittingAlgorithm()
```


Sayfa bölme için kullanılan algoritmayı alır veya ayarlar.

Değer: `PageSplittingAlgorithm`.

**Returns:**
[PageSplittingAlgorithm](../../com.aspose.note/pagesplittingalgorithm)
### setImageCompression(int value) {#setImageCompression-int-}
```
public final void setImageCompression(int value)
```


PDF dosyasındaki görüntülere uygulanan sıkıştırma türünü ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setJpegQuality(int value) {#setJpegQuality-int-}
```
public final void setJpegQuality(int value)
```


PDF belgesi içindeki JPEG görüntülerinin kalitesini belirleyen bir değeri ayarlar. Değer 0 ile 100 arasında değişebilir; 0 en düşük kaliteyi ancak maksimum sıkıştırmayı, 100 ise en yüksek kaliteyi ancak minimum sıkıştırmayı ifade eder.

--------------------

Varsayılan değer 90'dır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setPageSettings(PageSettings value) {#setPageSettings-com.aspose.note.PageSettings-}
```
public void setPageSettings(PageSettings value)
```


Belgedeki her sayfa için sayfa ayarlarını alır veya ayarlar. Varsayılan olarak CurrentUICulture'a bağlıdır, \*US kültürleri letter ayarına, diğerleri A4 ayarına sahiptir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [PageSettings](../../com.aspose.note/pagesettings) |  |

### setPageSplittingAlgorithm(PageSplittingAlgorithm value) {#setPageSplittingAlgorithm-com.aspose.note.PageSplittingAlgorithm-}
```
public void setPageSplittingAlgorithm(PageSplittingAlgorithm value)
```


Sayfa bölme için kullanılan algoritmayı alır veya ayarlar.

Değer: `PageSplittingAlgorithm`.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [PageSplittingAlgorithm](../../com.aspose.note/pagesplittingalgorithm) |  |

