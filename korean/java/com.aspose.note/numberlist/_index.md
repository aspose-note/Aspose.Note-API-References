---
title: "NumberList"
second_title: "Java용 Aspose.Note API 레퍼런스"
description: "번호 매기기 또는 글머리표 목록을 나타냅니다."
type: docs
weight: 64
url: /ko/java/com.aspose.note/numberlist/
---

**Inheritance:**
java.lang.Object
```
public class NumberList
```

번호 매기기 또는 글머리표 목록을 나타냅니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [NumberList(String bulletedSymbol, String font, int fontSize)](#NumberList-java.lang.String-java.lang.String-int-) | `NumberList` 클래스의 새 인스턴스를 초기화합니다. |
| [NumberList(String format, byte numberFormat, String font, int fontSize)](#NumberList-java.lang.String-byte-java.lang.String-int-) | `NumberList` 클래스의 새 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [equals(NumberList other)](#equals-com.aspose.note.NumberList-) | 지정된 객체가 현재 객체와 같은지 여부를 결정합니다. |
| [equals(Object obj)](#equals-java.lang.Object-) | 지정된 객체가 현재 객체와 같은지 여부를 결정합니다. |
| [getFont()](#getFont--) | 글꼴 이름을 가져오거나 설정합니다. |
| [getFontColor()](#getFontColor--) | 글꼴 색상을 가져오거나 설정합니다. |
| [getFontSize()](#getFontSize--) | 글꼴 크기를 가져오거나 설정합니다. |
| [getFormat()](#getFormat--) | 줄 머리글의 형식을 가져오거나 설정합니다. |
| [getLastModifiedTime()](#getLastModifiedTime--) | 마지막 수정 시간을 가져오거나 설정합니다. |
| [getNumberFormat()](#getNumberFormat--) | 자동 번호가 매겨진 객체 그룹에 사용되는 번호 형식을 가져오거나 설정합니다. |
| [getNumberedListHeader(int sequenceNumber)](#getNumberedListHeader-int-) | 번호 매겨진 목록 머리글을 가져옵니다. |
| [getRestart()](#getRestart--) | 목록 항목의 자동 번호 값을 재정의하는 숫자 값을 가져오거나 설정합니다. |
| [hashCode()](#hashCode--) | 해당 유형에 대한 해시 함수로 사용됩니다. |
| [isBold()](#isBold--) | 텍스트 스타일이 굵게인지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [isItalic()](#isItalic--) | 텍스트 스타일이 이탤릭인지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [setBold(boolean value)](#setBold-boolean-) | 텍스트 스타일이 굵게인지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [setFont(String value)](#setFont-java.lang.String-) | 글꼴 이름을 가져오거나 설정합니다. |
| [setFontColor(Color value)](#setFontColor-java.awt.Color-) | 글꼴 색상을 가져오거나 설정합니다. |
| [setFontSize(int value)](#setFontSize-int-) | 글꼴 크기를 가져오거나 설정합니다. |
| [setFormat(String value)](#setFormat-java.lang.String-) | 줄 머리글의 형식을 가져오거나 설정합니다. |
| [setItalic(boolean value)](#setItalic-boolean-) | 텍스트 스타일이 이탤릭인지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | 마지막 수정 시간을 가져오거나 설정합니다. |
| [setNumberFormat(Byte value)](#setNumberFormat-java.lang.Byte-) | 자동 번호가 매겨진 객체 그룹에 사용되는 번호 형식을 가져오거나 설정합니다. |
| [setRestart(int value)](#setRestart-int-) | 목록 항목의 자동 번호 값을 재정의하는 숫자 값을 가져오거나 설정합니다. |
### NumberList(String bulletedSymbol, String font, int fontSize) {#NumberList-java.lang.String-java.lang.String-int-}
```
public NumberList(String bulletedSymbol, String font, int fontSize)
```


`NumberList` 클래스의 새 인스턴스를 초기화합니다. 이 인스턴스는 글머리표 목록을 나타냅니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| bulletedSymbol | java.lang.String | 글머리표를 나타내는 기호. |
| font | java.lang.String | 글머리표용 글꼴. |
| fontSize | int | 글머리표용 글꼴 크기. |

### NumberList(String format, byte numberFormat, String font, int fontSize) {#NumberList-java.lang.String-byte-java.lang.String-int-}
```
public NumberList(String format, byte numberFormat, String font, int fontSize)
```


`NumberList` 클래스의 새 인스턴스를 초기화합니다. 이 인스턴스는 번호 매겨진 목록을 나타냅니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| format | java.lang.String | 번호 매겨진 머리글의 형식. |
| numberFormat | byte | 헤더에 있는 번호의 형식입니다. |
| font | java.lang.String | 번호가 매겨진 헤더에 대한 글꼴입니다. |
| fontSize | int | 번호가 매겨진 헤더에 대한 글꼴 크기입니다. |

### equals(NumberList other) {#equals-com.aspose.note.NumberList-}
```
public boolean equals(NumberList other)
```


지정된 객체가 현재 객체와 같은지 여부를 결정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| other | [NumberList](../../com.aspose.note/numberlist) | 객체입니다. |

**Returns:**
boolean - `bool`입니다.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


지정된 객체가 현재 객체와 같은지 여부를 결정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| obj | java.lang.Object | 객체입니다. |

**Returns:**
boolean - `bool`입니다.
### getFont() {#getFont--}
```
public String getFont()
```


글꼴 이름을 가져오거나 설정합니다.

**Returns:**
java.lang.String
### getFontColor() {#getFontColor--}
```
public Color getFontColor()
```


글꼴 색상을 가져오거나 설정합니다.

**Returns:**
java.awt.Color
### getFontSize() {#getFontSize--}
```
public int getFontSize()
```


글꼴 크기를 가져오거나 설정합니다.

**Returns:**
int
### getFormat() {#getFormat--}
```
public String getFormat()
```


줄 헤더의 형식을 가져오거나 설정합니다. 글머리표 목록의 경우 글머리 기호를 나타냅니다.

**Returns:**
java.lang.String
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


마지막 수정 시간을 가져오거나 설정합니다.

**Returns:**
java.util.Date
### getNumberFormat() {#getNumberFormat--}
```
public Byte getNumberFormat()
```


자동 번호가 매겨진 객체 그룹에 사용되는 번호 형식을 가져오거나 설정합니다. 글머리표 목록의 경우 null이어야 합니다.

**Returns:**
java.lang.Byte
### getNumberedListHeader(int sequenceNumber) {#getNumberedListHeader-int-}
```
public String getNumberedListHeader(int sequenceNumber)
```


번호 매겨진 목록 머리글을 가져옵니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| sequenceNumber | int | 번호가 매겨진 목록의 순서 번호입니다. |

**Returns:**
java.lang.String - 지정된 순서 번호의 문자열 표현입니다.
### getRestart() {#getRestart--}
```
public int getRestart()
```


목록 항목의 자동 번호 값을 재정의하는 숫자 값을 가져오거나 설정합니다.

**Returns:**
int
### hashCode() {#hashCode--}
```
public int hashCode()
```


해당 유형에 대한 해시 함수로 사용됩니다.

**Returns:**
int - `int`입니다.
### isBold() {#isBold--}
```
public boolean isBold()
```


텍스트 스타일이 굵게인지 여부를 나타내는 값을 가져오거나 설정합니다.

**Returns:**
boolean
### isItalic() {#isItalic--}
```
public boolean isItalic()
```


텍스트 스타일이 이탤릭인지 여부를 나타내는 값을 가져오거나 설정합니다.

**Returns:**
boolean
### setBold(boolean value) {#setBold-boolean-}
```
public void setBold(boolean value)
```


텍스트 스타일이 굵게인지 여부를 나타내는 값을 가져오거나 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | boolean |  |

### setFont(String value) {#setFont-java.lang.String-}
```
public void setFont(String value)
```


글꼴 이름을 가져오거나 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String |  |

### setFontColor(Color value) {#setFontColor-java.awt.Color-}
```
public void setFontColor(Color value)
```


글꼴 색상을 가져오거나 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.awt.Color |  |

### setFontSize(int value) {#setFontSize-int-}
```
public void setFontSize(int value)
```


글꼴 크기를 가져오거나 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | int |  |

### setFormat(String value) {#setFormat-java.lang.String-}
```
public void setFormat(String value)
```


줄 헤더의 형식을 가져오거나 설정합니다. 글머리표 목록의 경우 글머리 기호를 나타냅니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String |  |

### setItalic(boolean value) {#setItalic-boolean-}
```
public void setItalic(boolean value)
```


텍스트 스타일이 이탤릭인지 여부를 나타내는 값을 가져오거나 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | boolean |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


마지막 수정 시간을 가져오거나 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.util.Date |  |

### setNumberFormat(Byte value) {#setNumberFormat-java.lang.Byte-}
```
public void setNumberFormat(Byte value)
```


자동 번호가 매겨진 객체 그룹에 사용되는 번호 형식을 가져오거나 설정합니다. 글머리표 목록의 경우 null이어야 합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.lang.Byte |  |

### setRestart(int value) {#setRestart-int-}
```
public void setRestart(int value)
```


목록 항목의 자동 번호 값을 재정의하는 숫자 값을 가져오거나 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | int |  |

