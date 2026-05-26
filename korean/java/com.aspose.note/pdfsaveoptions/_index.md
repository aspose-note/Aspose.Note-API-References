---
title: "PdfSaveOptions"
second_title: "Java용 Aspose.Note API 레퍼런스"
description: "문서 페이지를 PDF로 렌더링할 때 추가 옵션을 지정할 수 있습니다."
type: docs
weight: 77
url: /ko/java/com.aspose.note/pdfsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.SaveOptions](../../com.aspose.note/saveoptions)
```
public final class PdfSaveOptions extends SaveOptions
```

문서 페이지를 PDF로 렌더링할 때 추가 옵션을 지정할 수 있습니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [PdfSaveOptions()](#PdfSaveOptions--) | 새 `PdfSaveOptions` 클래스 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getImageCompression()](#getImageCompression--) | PDF 파일의 이미지에 적용되는 압축 유형을 가져옵니다. |
| [getJpegQuality()](#getJpegQuality--) | PDF 문서 내부 JPEG 이미지의 품질을 결정하는 값을 가져옵니다. |
| [getPageSettings()](#getPageSettings--) | 문서의 각 페이지에 대한 페이지 설정을 가져오거나 설정합니다. |
| [getPageSplittingAlgorithm()](#getPageSplittingAlgorithm--) | 페이지 분할에 사용되는 알고리즘을 가져오거나 설정합니다. |
| [setImageCompression(int value)](#setImageCompression-int-) | PDF 파일의 이미지에 적용되는 압축 유형을 설정합니다. |
| [setJpegQuality(int value)](#setJpegQuality-int-) | PDF 문서 내부 JPEG 이미지의 품질을 결정하는 값을 설정합니다. |
| [setPageSettings(PageSettings value)](#setPageSettings-com.aspose.note.PageSettings-) | 문서의 각 페이지에 대한 페이지 설정을 가져오거나 설정합니다. |
| [setPageSplittingAlgorithm(PageSplittingAlgorithm value)](#setPageSplittingAlgorithm-com.aspose.note.PageSplittingAlgorithm-) | 페이지 분할에 사용되는 알고리즘을 가져오거나 설정합니다. |
### PdfSaveOptions() {#PdfSaveOptions--}
```
public PdfSaveOptions()
```


새 `PdfSaveOptions` 클래스 인스턴스를 초기화합니다.

### getImageCompression() {#getImageCompression--}
```
public final int getImageCompression()
```


PDF 파일의 이미지에 적용되는 압축 유형을 가져옵니다.

**Returns:**
int
### getJpegQuality() {#getJpegQuality--}
```
public final int getJpegQuality()
```


PDF 문서 내부 JPEG 이미지의 품질을 결정하는 값을 가져옵니다. 이 값은 0에서 100 사이이며, 0은 최악의 품질이지만 최대 압축을 의미하고 100은 최고의 품질이지만 최소 압축을 의미합니다.

--------------------

기본값은 90입니다.

**Returns:**
int
### getPageSettings() {#getPageSettings--}
```
public PageSettings getPageSettings()
```


문서의 각 페이지에 대한 페이지 설정을 가져오거나 설정합니다. 기본값은 CurrentUICulture에 따라 달라지며, \*US 문화권은 레터 설정을, 다른 문화권은 A4 설정을 사용합니다.

**Returns:**
[PageSettings](../../com.aspose.note/pagesettings)
### getPageSplittingAlgorithm() {#getPageSplittingAlgorithm--}
```
public PageSplittingAlgorithm getPageSplittingAlgorithm()
```


페이지 분할에 사용되는 알고리즘을 가져오거나 설정합니다.

값: `PageSplittingAlgorithm`.

**Returns:**
[PageSplittingAlgorithm](../../com.aspose.note/pagesplittingalgorithm)
### setImageCompression(int value) {#setImageCompression-int-}
```
public final void setImageCompression(int value)
```


PDF 파일의 이미지에 적용되는 압축 유형을 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | int |  |

### setJpegQuality(int value) {#setJpegQuality-int-}
```
public final void setJpegQuality(int value)
```


PDF 문서 내부 JPEG 이미지의 품질을 결정하는 값을 설정합니다. 이 값은 0에서 100 사이이며, 0은 최악의 품질이지만 최대 압축을 의미하고 100은 최고의 품질이지만 최소 압축을 의미합니다.

--------------------

기본값은 90입니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | int |  |

### setPageSettings(PageSettings value) {#setPageSettings-com.aspose.note.PageSettings-}
```
public void setPageSettings(PageSettings value)
```


문서의 각 페이지에 대한 페이지 설정을 가져오거나 설정합니다. 기본값은 CurrentUICulture에 따라 달라지며, \*US 문화권은 레터 설정을, 다른 문화권은 A4 설정을 사용합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| value | [PageSettings](../../com.aspose.note/pagesettings) |  |

### setPageSplittingAlgorithm(PageSplittingAlgorithm value) {#setPageSplittingAlgorithm-com.aspose.note.PageSplittingAlgorithm-}
```
public void setPageSplittingAlgorithm(PageSplittingAlgorithm value)
```


페이지 분할에 사용되는 알고리즘을 가져오거나 설정합니다.

값: `PageSplittingAlgorithm`.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| value | [PageSplittingAlgorithm](../../com.aspose.note/pagesplittingalgorithm) |  |

