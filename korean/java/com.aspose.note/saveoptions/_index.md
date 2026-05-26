---
title: "SaveOptions"
second_title: "Java용 Aspose.Note API 레퍼런스"
description: "특정 형식에 대한 문서 저장 옵션을 나타내는 추상 기본 클래스입니다."
type: docs
weight: 85
url: /ko/java/com.aspose.note/saveoptions/
---

**Inheritance:**
java.lang.Object
```
public abstract class SaveOptions
```

특정 형식에 대한 문서 저장 옵션을 나타내는 추상 기본 클래스입니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getFontsSubsystem()](#getFontsSubsystem--) | 저장 시 사용할 글꼴 설정을 가져오거나 설정합니다. |
| [getPageCount()](#getPageCount--) | 저장할 페이지 수를 가져오거나 설정합니다. |
| [getPageIndex()](#getPageIndex--) | 저장할 첫 번째 페이지의 인덱스를 가져오거나 설정합니다. |
| [getSaveFormat()](#getSaveFormat--) | 문서가 저장되는 형식을 가져오거나 설정합니다. |
| [setFontsSubsystem(FontsSubsystem value)](#setFontsSubsystem-com.aspose.note.fonts.FontsSubsystem-) | 저장 시 사용할 글꼴 설정을 가져오거나 설정합니다. |
| [setPageCount(int value)](#setPageCount-int-) | 저장할 페이지 수를 가져오거나 설정합니다. |
| [setPageIndex(int value)](#setPageIndex-int-) | 저장할 첫 번째 페이지의 인덱스를 가져오거나 설정합니다. |
### getFontsSubsystem() {#getFontsSubsystem--}
```
public final FontsSubsystem getFontsSubsystem()
```


저장 시 사용할 글꼴 설정을 가져오거나 설정합니다.

**Returns:**
[FontsSubsystem](../../com.aspose.note.fonts/fontssubsystem)
### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


저장할 페이지 수를 가져오거나 설정합니다. 기본값은 \{@link int\#Int32Extensions.MaxValue\}이며, 이는 문서의 모든 페이지가 렌더링됨을 의미합니다.

**Returns:**
int
### getPageIndex() {#getPageIndex--}
```
public final int getPageIndex()
```


저장할 첫 번째 페이지의 인덱스를 가져오거나 설정합니다. 기본값은 0입니다.

**Returns:**
int
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


문서가 저장되는 형식을 가져오거나 설정합니다.

**Returns:**
int
### setFontsSubsystem(FontsSubsystem value) {#setFontsSubsystem-com.aspose.note.fonts.FontsSubsystem-}
```
public final void setFontsSubsystem(FontsSubsystem value)
```


저장 시 사용할 글꼴 설정을 가져오거나 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| value | [FontsSubsystem](../../com.aspose.note.fonts/fontssubsystem) |  |

### setPageCount(int value) {#setPageCount-int-}
```
public final void setPageCount(int value)
```


저장할 페이지 수를 가져오거나 설정합니다. 기본값은 \{@link int\#Int32Extensions.MaxValue\}이며, 이는 문서의 모든 페이지가 렌더링됨을 의미합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | int |  |

### setPageIndex(int value) {#setPageIndex-int-}
```
public final void setPageIndex(int value)
```


저장할 첫 번째 페이지의 인덱스를 가져오거나 설정합니다. 기본값은 0입니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | int |  |

