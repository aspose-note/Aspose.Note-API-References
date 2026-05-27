---
title: "ImageSaveOptions"
second_title: "Aspose.Note for Java API Referansı"
description: "Belge sayfalarını görüntülere render ederken ek seçenekler belirtmeye izin verir."
type: docs
weight: 35
url: /tr/java/com.aspose.note/imagesaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.SaveOptions](../../com.aspose.note/saveoptions)
```
public class ImageSaveOptions extends SaveOptions
```

Belge sayfalarını görüntülere render ederken ek seçenekler belirtmeye izin verir.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [ImageSaveOptions(int format)](#ImageSaveOptions-int-) | Yeni bir `ImageSaveOptions` sınıfı örneği başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getBinarizationOptions()](#getBinarizationOptions--) | Görüntünün ikilileştirilmesi için seçenekleri alır veya ayarlar. |
| [getColorMode()](#getColorMode--) | Çıktı görüntüsü için `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-)) alır veya ayarlar. |
| [getQuality()](#getQuality--) | Kaydedilen görüntünün kalitesini belirleyen bir değeri alır. |
| [getResolution()](#getResolution--) | Oluşturulan görüntüler için çözünürlüğü alır, inç başına nokta (dpi) cinsinden. |
| [getTiffCompression()](#getTiffCompression--) | Oluşturulan görüntüleri TIFF formatında kaydederken kullanılacak sıkıştırma türünü alır veya ayarlar. |
| [setBinarizationOptions(ImageBinarizationOptions value)](#setBinarizationOptions-com.aspose.note.ImageBinarizationOptions-) | Görüntünün ikilileştirilmesi için seçenekleri alır veya ayarlar. |
| [setColorMode(int value)](#setColorMode-int-) | Çıktı görüntüsü için `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-)) alır veya ayarlar. |
| [setQuality(int value)](#setQuality-int-) | Kaydedilen görüntünün kalitesini belirleyen bir değeri ayarlar. |
| [setResolution(float value)](#setResolution-float-) | Oluşturulan görüntüler için çözünürlüğü, inç başına nokta cinsinden ayarlar. |
| [setTiffCompression(int value)](#setTiffCompression-int-) | Oluşturulan görüntüleri TIFF formatında kaydederken kullanılacak sıkıştırma türünü alır veya ayarlar. |
### ImageSaveOptions(int format) {#ImageSaveOptions-int-}
```
public ImageSaveOptions(int format)
```


Yeni bir `ImageSaveOptions` sınıfı örneği başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| format | int | Belgenin kaydedildiği format. |

### getBinarizationOptions() {#getBinarizationOptions--}
```
public final ImageBinarizationOptions getBinarizationOptions()
```


Görüntünün ikilileştirilmesi için seçenekleri alır veya ayarlar.

**Returns:**
[ImageBinarizationOptions](../../com.aspose.note/imagebinarizationoptions)
### getColorMode() {#getColorMode--}
```
public final int getColorMode()
```


Çıktı görüntüsü için `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-)) alır veya ayarlar.

**Returns:**
int
### getQuality() {#getQuality--}
```
public final int getQuality()
```


Kaydedilen görüntünün kalitesini belirleyen bir değeri alır. Bu değer, codec'e System.Drawing.Imaging.Encoder.Quality parametresi olarak iletilir.

--------------------

Kalite kategorisi için kullanılabilir değer aralığı 0 ile 100 arasındadır. Belirtilen sayı ne kadar düşük olursa, sıkıştırma o kadar yüksek olur ve dolayısıyla görüntünün kalitesi o kadar düşük olur. Sıfır en düşük kaliteyi, 100 ise en yüksek kaliteyi verir. Varsayılan değer 90'dır.

**Returns:**
int
### getResolution() {#getResolution--}
```
public float getResolution()
```


Oluşturulan görüntüler için çözünürlüğü alır, inç başına nokta (dpi) cinsinden.

--------------------

Varsayılan değer 96'dır.

**Returns:**
float
### getTiffCompression() {#getTiffCompression--}
```
public final int getTiffCompression()
```


Oluşturulan görüntüleri TIFF formatında kaydederken kullanılacak sıkıştırma türünü alır veya ayarlar.

**Returns:**
int
### setBinarizationOptions(ImageBinarizationOptions value) {#setBinarizationOptions-com.aspose.note.ImageBinarizationOptions-}
```
public final void setBinarizationOptions(ImageBinarizationOptions value)
```


Görüntünün ikilileştirilmesi için seçenekleri alır veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [ImageBinarizationOptions](../../com.aspose.note/imagebinarizationoptions) |  |

### setColorMode(int value) {#setColorMode-int-}
```
public final void setColorMode(int value)
```


Çıktı görüntüsü için `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-)) alır veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setQuality(int value) {#setQuality-int-}
```
public final void setQuality(int value)
```


Kaydedilen görüntünün kalitesini belirleyen bir değeri ayarlar. Bu değer, codec'e System.Drawing.Imaging.Encoder.Quality parametresi olarak iletilir.

--------------------

Kalite kategorisi için kullanılabilir değer aralığı 0 ile 100 arasındadır. Belirtilen sayı ne kadar düşük olursa, sıkıştırma o kadar yüksek olur ve dolayısıyla görüntünün kalitesi o kadar düşük olur. Sıfır en düşük kaliteyi, 100 ise en yüksek kaliteyi verir. Varsayılan değer 90'dır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setResolution(float value) {#setResolution-float-}
```
public void setResolution(float value)
```


Oluşturulan görüntüler için çözünürlüğü, inç başına nokta cinsinden ayarlar.

--------------------

Varsayılan değer 90'dır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | float |  |

### setTiffCompression(int value) {#setTiffCompression-int-}
```
public final void setTiffCompression(int value)
```


Oluşturulan görüntüleri TIFF formatında kaydederken kullanılacak sıkıştırma türünü alır veya ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

