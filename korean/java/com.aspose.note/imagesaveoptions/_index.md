---
title: "ImageSaveOptions"
second_title: "Java용 Aspose.Note API 레퍼런스"
description: "문서 페이지를 이미지로 렌더링할 때 추가 옵션을 지정할 수 있습니다."
type: docs
weight: 35
url: /ko/java/com.aspose.note/imagesaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.SaveOptions](../../com.aspose.note/saveoptions)
```
public class ImageSaveOptions extends SaveOptions
```

문서 페이지를 이미지로 렌더링할 때 추가 옵션을 지정할 수 있습니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [ImageSaveOptions(int format)](#ImageSaveOptions-int-) | 새 `ImageSaveOptions` 클래스 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getBinarizationOptions()](#getBinarizationOptions--) | 이미지 이진화 옵션을 가져오거나 설정합니다. |
| [getColorMode()](#getColorMode--) | 출력 이미지에 대한 `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-))을 가져오거나 설정합니다. |
| [getQuality()](#getQuality--) | 저장된 이미지 품질을 결정하는 값을 가져옵니다. |
| [getResolution()](#getResolution--) | 생성된 이미지의 해상도를 DPI(인치당 도트) 단위로 가져옵니다. |
| [getTiffCompression()](#getTiffCompression--) | 생성된 이미지를 TIFF 형식으로 저장할 때 사용할 압축 유형을 가져오거나 설정합니다. |
| [setBinarizationOptions(ImageBinarizationOptions value)](#setBinarizationOptions-com.aspose.note.ImageBinarizationOptions-) | 이미지 이진화 옵션을 가져오거나 설정합니다. |
| [setColorMode(int value)](#setColorMode-int-) | 출력 이미지에 대한 `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-))을 가져오거나 설정합니다. |
| [setQuality(int value)](#setQuality-int-) | 저장된 이미지의 품질을 결정하는 값을 설정합니다. |
| [setResolution(float value)](#setResolution-float-) | 생성된 이미지의 해상도를 인치당 도트(dpi) 단위로 설정합니다. |
| [setTiffCompression(int value)](#setTiffCompression-int-) | 생성된 이미지를 TIFF 형식으로 저장할 때 사용할 압축 유형을 가져오거나 설정합니다. |
### ImageSaveOptions(int format) {#ImageSaveOptions-int-}
```
public ImageSaveOptions(int format)
```


새 `ImageSaveOptions` 클래스 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| format | int | 문서가 저장되는 형식입니다. |

### getBinarizationOptions() {#getBinarizationOptions--}
```
public final ImageBinarizationOptions getBinarizationOptions()
```


이미지 이진화 옵션을 가져오거나 설정합니다.

**Returns:**
[ImageBinarizationOptions](../../com.aspose.note/imagebinarizationoptions)
### getColorMode() {#getColorMode--}
```
public final int getColorMode()
```


출력 이미지에 대한 `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-))을 가져오거나 설정합니다.

**Returns:**
int
### getQuality() {#getQuality--}
```
public final int getQuality()
```


저장된 이미지의 품질을 결정하는 값을 가져옵니다. 이 값은 System.Drawing.Imaging.Encoder.Quality 매개변수로 코덱에 전달됩니다.

--------------------

품질 범주의 유용한 값 범위는 0에서 100까지입니다. 지정된 숫자가 낮을수록 압축이 높아지고 그에 따라 이미지 품질이 낮아집니다. 0은 가장 낮은 품질의 이미지를, 100은 가장 높은 품질의 이미지를 제공합니다. 기본값은 90입니다.

**Returns:**
int
### getResolution() {#getResolution--}
```
public float getResolution()
```


생성된 이미지의 해상도를 DPI(인치당 도트) 단위로 가져옵니다.

--------------------

기본값은 96입니다.

**Returns:**
float
### getTiffCompression() {#getTiffCompression--}
```
public final int getTiffCompression()
```


생성된 이미지를 TIFF 형식으로 저장할 때 사용할 압축 유형을 가져오거나 설정합니다.

**Returns:**
int
### setBinarizationOptions(ImageBinarizationOptions value) {#setBinarizationOptions-com.aspose.note.ImageBinarizationOptions-}
```
public final void setBinarizationOptions(ImageBinarizationOptions value)
```


이미지 이진화 옵션을 가져오거나 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| value | [ImageBinarizationOptions](../../com.aspose.note/imagebinarizationoptions) |  |

### setColorMode(int value) {#setColorMode-int-}
```
public final void setColorMode(int value)
```


출력 이미지에 대한 `ColorMode`([getColorMode](../../com.aspose.note/imagesaveoptions\#getColorMode--)/[setColorMode(int)](../../com.aspose.note/imagesaveoptions\#setColorMode-int-))을 가져오거나 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | int |  |

### setQuality(int value) {#setQuality-int-}
```
public final void setQuality(int value)
```


저장된 이미지의 품질을 결정하는 값을 설정합니다. 이 값은 System.Drawing.Imaging.Encoder.Quality 매개변수로 코덱에 전달됩니다.

--------------------

품질 범주의 유용한 값 범위는 0에서 100까지입니다. 지정된 숫자가 낮을수록 압축이 높아지고 그에 따라 이미지 품질이 낮아집니다. 0은 가장 낮은 품질의 이미지를, 100은 가장 높은 품질의 이미지를 제공합니다. 기본값은 90입니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | int |  |

### setResolution(float value) {#setResolution-float-}
```
public void setResolution(float value)
```


생성된 이미지의 해상도를 인치당 도트(dpi) 단위로 설정합니다.

--------------------

기본값은 90입니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | float |  |

### setTiffCompression(int value) {#setTiffCompression-int-}
```
public final void setTiffCompression(int value)
```


생성된 이미지를 TIFF 형식으로 저장할 때 사용할 압축 유형을 가져오거나 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | int |  |

