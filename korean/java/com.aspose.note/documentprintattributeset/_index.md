---
title: "DocumentPrintAttributeSet"
second_title: "Java용 Aspose.Note API 레퍼런스"
description: "AttributeSet과 함께 사용자 친화적인 인터페이스를 제공하는 도우미 클래스를 나타냅니다."
type: docs
weight: 21
url: /ko/java/com.aspose.note/documentprintattributeset/
---

**Inheritance:**
java.lang.Object, javax.print.attribute.HashAttributeSet
```
public final class DocumentPrintAttributeSet extends HashAttributeSet
```

AttributeSet과 함께 사용자 친화적인 인터페이스를 제공하는 도우미 클래스를 나타냅니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [DocumentPrintAttributeSet(int copies)](#DocumentPrintAttributeSet-int-) | 새 인스턴스 `DocumentPrintAttributeSet`를 초기화합니다. |
| [DocumentPrintAttributeSet(String printerName, int copies)](#DocumentPrintAttributeSet-java.lang.String-int-) | 새 인스턴스 `DocumentPrintAttributeSet`를 초기화합니다. |
| [DocumentPrintAttributeSet(String printerName)](#DocumentPrintAttributeSet-java.lang.String-) | 새 인스턴스 `DocumentPrintAttributeSet`를 초기화합니다. |
| [DocumentPrintAttributeSet()](#DocumentPrintAttributeSet--) | 새 인스턴스 `DocumentPrintAttributeSet`를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getCopies()](#getCopies--) |  |
| [getLandscape()](#getLandscape--) |  |
| [getPrinterName()](#getPrinterName--) |  |
| [setCollate(boolean value)](#setCollate-boolean-) | 문서가 정렬되는지 여부를 나타내는 값을 설정합니다. |
| [setCopies(int value)](#setCopies-int-) | 인쇄할 복사본 수를 설정합니다. |
| [setDuplex(boolean value)](#setDuplex-boolean-) | 양면 인쇄를 위한 프린터 설정을 설정합니다. |
| [setLandscape(boolean value)](#setLandscape-boolean-) | 페이지 방향을 설정합니다. |
| [setPrintRange(int page)](#setPrintRange-int-) | 인쇄할 단일 페이지를 설정합니다. |
| [setPrintRange(int from, int to)](#setPrintRange-int-int-) | 인쇄할 페이지 범위를 설정합니다. |
| [setPrinterName(String printerName)](#setPrinterName-java.lang.String-) | 사용할 프린터의 이름입니다. |
| [setPrinterName(String printerName, Locale locale)](#setPrinterName-java.lang.String-java.util.Locale-) | 사용할 프린터의 이름입니다. |
### DocumentPrintAttributeSet(int copies) {#DocumentPrintAttributeSet-int-}
```
public DocumentPrintAttributeSet(int copies)
```


새 인스턴스 `DocumentPrintAttributeSet`를 초기화합니다. 기본적으로 문서의 모든 페이지가 인쇄됩니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 복사본 | int | 인쇄할 문서 복사본 수입니다. |

### DocumentPrintAttributeSet(String printerName, int copies) {#DocumentPrintAttributeSet-java.lang.String-int-}
```
public DocumentPrintAttributeSet(String printerName, int copies)
```


새 인스턴스 `DocumentPrintAttributeSet`를 초기화합니다. 기본적으로 문서의 모든 페이지가 인쇄됩니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| printerName | java.lang.String | 프린터 이름입니다. |
| 복사본 | int | 인쇄할 문서 복사본 수입니다. |

### DocumentPrintAttributeSet(String printerName) {#DocumentPrintAttributeSet-java.lang.String-}
```
public DocumentPrintAttributeSet(String printerName)
```


새 인스턴스 `DocumentPrintAttributeSet`를 초기화합니다. 기본적으로 각 페이지당 한 부만 인쇄됩니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| printerName | java.lang.String | 프린터 이름입니다. |

### DocumentPrintAttributeSet() {#DocumentPrintAttributeSet--}
```
public DocumentPrintAttributeSet()
```


새 인스턴스 `DocumentPrintAttributeSet`를 초기화합니다. 기본적으로 각 페이지당 한 부만 인쇄됩니다.

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


문서가 정렬되는지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | boolean | true는 SheetCollate.COLLATED 설정과 동일하고 false는 SheetCollate.UNCOLLATED 설정과 동일합니다. |

### setCopies(int value) {#setCopies-int-}
```
public void setCopies(int value)
```


인쇄할 복사본 수를 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | int | 인쇄할 복사본 수입니다. |

### setDuplex(boolean value) {#setDuplex-boolean-}
```
public void setDuplex(boolean value)
```


양면 인쇄를 위한 프린터 설정을 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | boolean | true는 Sides.DUPLEX 설정과 동일하고 false는 Sides.ONE\_SIDED 설정과 동일합니다. |

### setLandscape(boolean value) {#setLandscape-boolean-}
```
public void setLandscape(boolean value)
```


페이지 방향을 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | boolean | true는 OrientationRequested.LANDSCAPE 설정과 동일하고 false는 OrientationRequested.PORTRAIT 설정과 동일합니다. |

### setPrintRange(int page) {#setPrintRange-int-}
```
public void setPrintRange(int page)
```


인쇄할 단일 페이지를 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 페이지 | int | 인쇄할 페이지입니다. |

### setPrintRange(int from, int to) {#setPrintRange-int-int-}
```
public void setPrintRange(int from, int to)
```


인쇄할 페이지 범위를 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 부터 | int | 첫 번째 페이지입니다. |
| 까지 | int | 마지막 페이지. |

### setPrinterName(String printerName) {#setPrinterName-java.lang.String-}
```
public void setPrinterName(String printerName)
```


사용할 프린터의 이름입니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| printerName | java.lang.String | 프린터 이름입니다. |

### setPrinterName(String printerName, Locale locale) {#setPrinterName-java.lang.String-java.util.Locale-}
```
public void setPrinterName(String printerName, Locale locale)
```


사용할 프린터의 이름입니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| printerName | java.lang.String | 프린터 이름입니다. |
| locale | java.util.Locale | printerName의 로케일. |

