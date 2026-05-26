---
title: "TextStyle"
second_title: "Java용 Aspose.Note API 레퍼런스"
description: "텍스트 스타일을 지정합니다."
type: docs
weight: 93
url: /ko/java/com.aspose.note/textstyle/
---

**Inheritance:**
java.lang.Object, com.aspose.note.Style
```
public final class TextStyle extends Style<TextStyle>
```

텍스트 스타일을 지정합니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [TextStyle()](#TextStyle--) | 새 인스턴스를 초기화합니다 `TextStyle` 클래스. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [equals(TextStyle other)](#equals-com.aspose.note.TextStyle-) | 지정된 객체가 현재 객체와 같은지 여부를 결정합니다. |
| [equals(Object obj)](#equals-java.lang.Object-) | 지정된 객체가 현재 객체와 같은지 여부를 결정합니다. |
| [getDefault()](#getDefault--) | "en-US" 문화권의 스타일을 가져옵니다. |
| [getDefaultMsOneNoteTitleDateStyle()](#getDefaultMsOneNoteTitleDateStyle--) | MS OneNote에서 제목 날짜에 대한 기본 스타일을 가져옵니다. |
| [getDefaultMsOneNoteTitleTextStyle()](#getDefaultMsOneNoteTitleTextStyle--) | MS OneNote에서 제목 텍스트에 대한 기본 스타일을 가져옵니다. |
| [getDefaultMsOneNoteTitleTimeStyle()](#getDefaultMsOneNoteTitleTimeStyle--) | MS OneNote에서 제목 시간에 대한 기본 스타일을 가져옵니다. |
| [getHyperlinkAddress()](#getHyperlinkAddress--) | 하이퍼링크 주소를 가져옵니다. |
| [getLanguage()](#getLanguage--) | 텍스트의 언어를 가져옵니다. |
| [hashCode()](#hashCode--) | 해당 유형에 대한 해시 함수로 사용됩니다. |
| [isHidden()](#isHidden--) | 텍스트 스타일이 숨겨져 있는지 여부를 나타내는 값을 가져옵니다. |
| [isHyperlink()](#isHyperlink--) | 텍스트 스타일이 하이퍼링크인지 여부를 나타내는 값을 가져옵니다. |
| [isMathFormatting()](#isMathFormatting--) | 텍스트 스타일이 수학 형식인지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [setHidden(boolean value)](#setHidden-boolean-) | 텍스트 스타일이 숨겨져 있는지 여부를 나타내는 값을 설정합니다. |
| [setHyperlink(boolean value)](#setHyperlink-boolean-) | 텍스트 스타일이 하이퍼링크인지 여부를 나타내는 값을 설정합니다. |
| [setHyperlinkAddress(String value)](#setHyperlinkAddress-java.lang.String-) | 하이퍼링크 주소를 설정합니다. |
| [setLanguage(Locale value)](#setLanguage-java.util.Locale-) | 텍스트의 언어를 설정합니다. |
| [setMathFormatting(boolean value)](#setMathFormatting-boolean-) | 텍스트 스타일이 수학 형식인지 여부를 나타내는 값을 설정합니다. |
### TextStyle() {#TextStyle--}
```
public TextStyle()
```


새 인스턴스를 초기화합니다 `TextStyle` 클래스.

### equals(TextStyle other) {#equals-com.aspose.note.TextStyle-}
```
public boolean equals(TextStyle other)
```


지정된 객체가 현재 객체와 같은지 여부를 결정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| other | [TextStyle](../../com.aspose.note/textstyle) | 객체입니다. |

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
### getDefault() {#getDefault--}
```
public static TextStyle getDefault()
```


"en-US" 문화권의 스타일을 가져옵니다.

**Returns:**
[TextStyle](../../com.aspose.note/textstyle)
### getDefaultMsOneNoteTitleDateStyle() {#getDefaultMsOneNoteTitleDateStyle--}
```
public static TextStyle getDefaultMsOneNoteTitleDateStyle()
```


MS OneNote에서 제목 날짜에 대한 기본 스타일을 가져옵니다.

**Returns:**
[TextStyle](../../com.aspose.note/textstyle)
### getDefaultMsOneNoteTitleTextStyle() {#getDefaultMsOneNoteTitleTextStyle--}
```
public static TextStyle getDefaultMsOneNoteTitleTextStyle()
```


MS OneNote에서 제목 텍스트에 대한 기본 스타일을 가져옵니다.

**Returns:**
[TextStyle](../../com.aspose.note/textstyle)
### getDefaultMsOneNoteTitleTimeStyle() {#getDefaultMsOneNoteTitleTimeStyle--}
```
public static TextStyle getDefaultMsOneNoteTitleTimeStyle()
```


MS OneNote에서 제목 시간에 대한 기본 스타일을 가져옵니다.

**Returns:**
[TextStyle](../../com.aspose.note/textstyle)
### getHyperlinkAddress() {#getHyperlinkAddress--}
```
public String getHyperlinkAddress()
```


하이퍼링크 주소를 가져옵니다. [isHyperlink](../../com.aspose.note/textstyle\#isHyperlink--) 속성의 값이 true인 경우 설정해야 합니다.

**Returns:**
java.lang.String
### getLanguage() {#getLanguage--}
```
public Locale getLanguage()
```


텍스트의 언어를 가져옵니다.

**Returns:**
java.util.Locale
### hashCode() {#hashCode--}
```
public int hashCode()
```


해당 유형에 대한 해시 함수로 사용됩니다.

**Returns:**
int - `int`입니다.
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


텍스트 스타일이 숨겨져 있는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean
### isHyperlink() {#isHyperlink--}
```
public boolean isHyperlink()
```


텍스트 스타일이 하이퍼링크인지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean
### isMathFormatting() {#isMathFormatting--}
```
public boolean isMathFormatting()
```


텍스트 스타일이 수학 형식인지 여부를 나타내는 값을 가져오거나 설정합니다.

**Returns:**
boolean
### setHidden(boolean value) {#setHidden-boolean-}
```
public TextStyle setHidden(boolean value)
```


텍스트 스타일이 숨겨져 있는지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | boolean |  |

**Returns:**
[TextStyle](../../com.aspose.note/textstyle)
### setHyperlink(boolean value) {#setHyperlink-boolean-}
```
public TextStyle setHyperlink(boolean value)
```


텍스트 스타일이 하이퍼링크인지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | boolean |  |

**Returns:**
[TextStyle](../../com.aspose.note/textstyle)
### setHyperlinkAddress(String value) {#setHyperlinkAddress-java.lang.String-}
```
public TextStyle setHyperlinkAddress(String value)
```


하이퍼링크 주소를 설정합니다. [isHyperlink](../../com.aspose.note/textstyle\#isHyperlink--) 속성의 값이 true인 경우 설정해야 합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String |  |

**Returns:**
[TextStyle](../../com.aspose.note/textstyle)
### setLanguage(Locale value) {#setLanguage-java.util.Locale-}
```
public TextStyle setLanguage(Locale value)
```


텍스트의 언어를 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.util.Locale |  |

**Returns:**
[TextStyle](../../com.aspose.note/textstyle)
### setMathFormatting(boolean value) {#setMathFormatting-boolean-}
```
public TextStyle setMathFormatting(boolean value)
```


텍스트 스타일이 수학 형식인지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | boolean |  |

**Returns:**
[TextStyle](../../com.aspose.note/textstyle)
