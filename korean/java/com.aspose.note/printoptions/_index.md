---
title: "PrintOptions"
second_title: "Java용 Aspose.Note API 레퍼런스"
description: "문서를 인쇄할 때 사용되는 옵션입니다."
type: docs
weight: 78
url: /ko/java/com.aspose.note/printoptions/
---

**Inheritance:**
java.lang.Object
```
public class PrintOptions
```

문서를 인쇄할 때 사용되는 옵션입니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [PrintOptions()](#PrintOptions--) | `PrintOptions` 클래스의 새 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getDocumentName()](#getDocumentName--) | 문서를 인쇄하는 동안 표시할 문서 이름을 가져오거나 설정합니다(예: 인쇄 상태 대화 상자 또는 프린터 대기열). |
| [getPageSplittingAlgorithm()](#getPageSplittingAlgorithm--) | 페이지 분할에 사용되는 알고리즘을 가져오거나 설정합니다. |
| [getPrinterSettings()](#getPrinterSettings--) | 프린터 설정을 가져오거나 설정합니다. |
| [getResolution()](#getResolution--) | 생성된 이미지의 해상도를 인치당 도트 수(DPI)로 가져오거나 설정합니다. |
| [setDocumentName(String value)](#setDocumentName-java.lang.String-) | 문서를 인쇄하는 동안 표시할 문서 이름을 가져오거나 설정합니다(예: 인쇄 상태 대화 상자 또는 프린터 대기열). |
| [setPageSplittingAlgorithm(PageSplittingAlgorithm value)](#setPageSplittingAlgorithm-com.aspose.note.PageSplittingAlgorithm-) | 페이지 분할에 사용되는 알고리즘을 가져오거나 설정합니다. |
| [setPrinterSettings(AttributeSet value)](#setPrinterSettings-javax.print.attribute.AttributeSet-) | 프린터 설정을 가져오거나 설정합니다. |
| [setResolution(float value)](#setResolution-float-) | 생성된 이미지의 해상도를 인치당 도트 수(DPI)로 가져오거나 설정합니다. |
### PrintOptions() {#PrintOptions--}
```
public PrintOptions()
```


`PrintOptions` 클래스의 새 인스턴스를 초기화합니다.

### getDocumentName() {#getDocumentName--}
```
public String getDocumentName()
```


문서를 인쇄하는 동안 표시할 문서 이름을 가져오거나 설정합니다(예: 인쇄 상태 대화 상자 또는 프린터 대기열).

**Returns:**
java.lang.String
### getPageSplittingAlgorithm() {#getPageSplittingAlgorithm--}
```
public PageSplittingAlgorithm getPageSplittingAlgorithm()
```


페이지 분할에 사용되는 알고리즘을 가져오거나 설정합니다.

값: `PageSplittingAlgorithm`.

**Returns:**
[PageSplittingAlgorithm](../../com.aspose.note/pagesplittingalgorithm)
### getPrinterSettings() {#getPrinterSettings--}
```
public AttributeSet getPrinterSettings()
```


프린터 설정을 가져오거나 설정합니다.

**Returns:**
javax.print.attribute.AttributeSet
### getResolution() {#getResolution--}
```
public float getResolution()
```


생성된 이미지의 해상도를 인치당 도트 수(DPI)로 가져오거나 설정합니다.

--------------------

기본값은 96입니다.

**Returns:**
float
### setDocumentName(String value) {#setDocumentName-java.lang.String-}
```
public void setDocumentName(String value)
```


문서를 인쇄하는 동안 표시할 문서 이름을 가져오거나 설정합니다(예: 인쇄 상태 대화 상자 또는 프린터 대기열).

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String |  |

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

### setPrinterSettings(AttributeSet value) {#setPrinterSettings-javax.print.attribute.AttributeSet-}
```
public void setPrinterSettings(AttributeSet value)
```


프린터 설정을 가져오거나 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | javax.print.attribute.AttributeSet |  |

### setResolution(float value) {#setResolution-float-}
```
public void setResolution(float value)
```


생성된 이미지의 해상도를 인치당 도트 수(DPI)로 가져오거나 설정합니다.

--------------------

기본값은 96입니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | float |  |

