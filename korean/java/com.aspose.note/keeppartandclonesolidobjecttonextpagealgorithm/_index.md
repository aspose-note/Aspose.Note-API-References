---
title: "KeepPartAndCloneSolidObjectToNextPageAlgorithm"
second_title: "Java용 Aspose.Note API 레퍼런스"
description: "객체의 상단 부분을 페이지 하단에 추가하고, 원본 페이지에 맞지 않을 경우 전체 객체를 다음 페이지에 복제합니다."
type: docs
weight: 42
url: /ko/java/com.aspose.note/keeppartandclonesolidobjecttonextpagealgorithm/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.PageSplittingAlgorithm](../../com.aspose.note/pagesplittingalgorithm)
```
public class KeepPartAndCloneSolidObjectToNextPageAlgorithm extends PageSplittingAlgorithm
```

객체의 상단 부분을 페이지 하단에 추가하고, 원본 페이지에 맞지 않을 경우 전체 객체를 다음 페이지에 복제합니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [KeepPartAndCloneSolidObjectToNextPageAlgorithm()](#KeepPartAndCloneSolidObjectToNextPageAlgorithm--) | `KeepPartAndCloneSolidObjectToNextPageAlgorithm` 클래스를 새 인스턴스로 초기화하며, 복제된 부분의 기본 높이 제한을 사용합니다. |
| [KeepPartAndCloneSolidObjectToNextPageAlgorithm(float heightLimitOfClonedPart)](#KeepPartAndCloneSolidObjectToNextPageAlgorithm-float-) | `KeepPartAndCloneSolidObjectToNextPageAlgorithm` 클래스를 새 인스턴스로 초기화하며, 복제된 부분의 특정 높이 제한을 사용합니다. |
## 필드

| 필드 | 설명 |
| --- | --- |
| [DEFAULT_HEIGHT_LIMIT_OF_CLONED_PART](#DEFAULT-HEIGHT-LIMIT-OF-CLONED-PART) | 복제된 부분의 기본 최대 크기입니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getHeightLimitOfClonedPart()](#getHeightLimitOfClonedPart--) | 복제된 부분의 높이 제한을 가져옵니다. |
### KeepPartAndCloneSolidObjectToNextPageAlgorithm() {#KeepPartAndCloneSolidObjectToNextPageAlgorithm--}
```
public KeepPartAndCloneSolidObjectToNextPageAlgorithm()
```


`KeepPartAndCloneSolidObjectToNextPageAlgorithm` 클래스를 새 인스턴스로 초기화하며, 복제된 부분의 기본 높이 제한을 사용합니다.

### KeepPartAndCloneSolidObjectToNextPageAlgorithm(float heightLimitOfClonedPart) {#KeepPartAndCloneSolidObjectToNextPageAlgorithm-float-}
```
public KeepPartAndCloneSolidObjectToNextPageAlgorithm(float heightLimitOfClonedPart)
```


`KeepPartAndCloneSolidObjectToNextPageAlgorithm` 클래스를 새 인스턴스로 초기화하며, 복제된 부분의 특정 높이 제한을 사용합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| heightLimitOfClonedPart | float | 복제된 부분의 최대 높이. |

### DEFAULT_HEIGHT_LIMIT_OF_CLONED_PART {#DEFAULT-HEIGHT-LIMIT-OF-CLONED-PART}
```
public static final float DEFAULT_HEIGHT_LIMIT_OF_CLONED_PART
```


복제된 부분의 기본 최대 크기입니다.

### getHeightLimitOfClonedPart() {#getHeightLimitOfClonedPart--}
```
public float getHeightLimitOfClonedPart()
```


복제된 부분의 높이 제한을 가져옵니다.

**Returns:**
float
