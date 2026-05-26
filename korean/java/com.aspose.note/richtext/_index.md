---
title: "RichText"
second_title: "Java용 Aspose.Note API 레퍼런스"
description: "리치 텍스트를 나타냅니다."
type: docs
weight: 82
url: /ko/java/com.aspose.note/richtext/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node)

**All Implemented Interfaces:**
[com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode), [com.aspose.note.ITaggable](../../com.aspose.note/itaggable), com.aspose.ms.System.Collections.Generic.IGenericEnumerable
```
public class RichText extends Node implements IOutlineElementChildNode, ITaggable, System.Collections.Generic.IGenericEnumerable<Character>
```

리치 텍스트를 나타냅니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [RichText()](#RichText--) | 새 [RichText](../../com.aspose.note/richtext) 클래스 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | 노드의 방문자를 수락합니다. |
| [append(String value)](#append-java.lang.String-) | 마지막 텍스트 범위에 문자열을 추가합니다. |
| [append(String value, TextStyle style)](#append-java.lang.String-com.aspose.note.TextStyle-) | 문자열을 끝에 추가합니다. |
| [appendFront(String value)](#appendFront-java.lang.String-) | 첫 번째 텍스트 범위의 앞에 문자열을 추가합니다. |
| [appendFront(String value, TextStyle style)](#appendFront-java.lang.String-com.aspose.note.TextStyle-) | 문자열을 앞에 추가합니다. |
| [clear()](#clear--) | 이 인스턴스의 내용을 지웁니다. |
| [getAlignment()](#getAlignment--) | 정렬을 가져옵니다. |
| [getLastModifiedTime()](#getLastModifiedTime--) | 마지막 수정 시간을 가져옵니다. |
| [getLength()](#getLength--) |  |
| [getLineSpacing()](#getLineSpacing--) | 줄 간격을 가져옵니다. |
| [getParagraphStyle()](#getParagraphStyle--) | 단락 스타일을 가져옵니다. |
| [getSpaceAfter()](#getSpaceAfter--) | 뒤쪽 최소 간격을 가져옵니다. |
| [getSpaceBefore()](#getSpaceBefore--) | 앞쪽 최소 간격을 가져옵니다. |
| [getStyles()](#getStyles--) | 스타일을 가져옵니다. |
| [getTags()](#getTags--) | 단락의 모든 태그 목록을 가져옵니다. |
| [getText()](#getText--) | 텍스트를 가져옵니다. |
| [getTextRuns()](#getTextRuns--) |  |
| [indexOf(char value)](#indexOf-char-) | 이 문자열에서 지정된 유니코드 문자의 첫 번째 발생 위치의 0부터 시작하는 인덱스를 반환합니다. |
| [indexOf(char value, int startIndex)](#indexOf-char-int-) | 이 문자열에서 지정된 유니코드 문자의 첫 번째 발생 위치의 0부터 시작하는 인덱스를 반환합니다. |
| [indexOf(char value, int startIndex, int count)](#indexOf-char-int-int-) | 이 인스턴스에서 지정된 문자의 첫 번째 발생 위치의 0부터 시작하는 인덱스를 반환합니다. |
| [indexOf(String value)](#indexOf-java.lang.String-) | 이 인스턴스에서 지정된 문자열의 첫 번째 발생 위치의 0부터 시작하는 인덱스를 반환합니다. |
| [indexOf(String value, int startIndex)](#indexOf-java.lang.String-int-) | 이 인스턴스에서 지정된 문자열의 첫 번째 발생 위치의 0부터 시작하는 인덱스를 반환합니다. |
| [indexOf(String value, int startIndex, int count)](#indexOf-java.lang.String-int-int-) | 이 인스턴스에서 지정된 문자열의 첫 번째 발생 위치의 0부터 시작하는 인덱스를 반환합니다. |
| [indexOf(String value, int startIndex, int count, short comparisonType)](#indexOf-java.lang.String-int-int-short-) | 현재 인스턴스에서 지정된 문자열의 첫 번째 발생 위치의 0부터 시작하는 인덱스를 반환합니다. |
| [indexOf(String value, short comparisonType)](#indexOf-java.lang.String-short-) | 현재 인스턴스에서 지정된 문자열의 첫 번째 발생 위치의 0부터 시작하는 인덱스를 반환합니다. |
| [indexOf_Rename_Namesake(String value, int startIndex, short comparisonType)](#indexOf-Rename-Namesake-java.lang.String-int-short-) | 현재 인스턴스에서 지정된 문자열의 첫 번째 발생 위치의 0부터 시작하는 인덱스를 반환합니다. |
| [insert(int startIndex, String value)](#insert-int-java.lang.String-) | 이 인스턴스의 지정된 인덱스 위치에 지정된 문자열을 삽입합니다. |
| [insert(int startIndex, String value, TextStyle style)](#insert-int-java.lang.String-com.aspose.note.TextStyle-) | 이 인스턴스의 지정된 인덱스 위치에 지정된 스타일을 가진 문자열을 삽입합니다. |
| [iterator()](#iterator--) |  |
| [remove(int startIndex)](#remove-int-) | 현재 인스턴스에서 지정된 위치부터 마지막 위치까지 모든 문자를 제거합니다. |
| [remove(int startIndex, int count)](#remove-int-int-) | 현재 인스턴스에서 지정된 위치부터 지정된 수만큼의 문자를 제거합니다. |
| [replace(char oldChar, char newChar)](#replace-char-char-) | 이 인스턴스에서 지정된 유니코드 문자의 모든 발생을 다른 지정된 유니코드 문자로 교체합니다. |
| [replace(String oldValue, String newValue)](#replace-java.lang.String-java.lang.String-) | 현재 인스턴스에서 지정된 문자열의 모든 발생을 다른 지정된 문자열로 교체합니다. |
| [replace(String oldValue, String newValue, TextStyle style)](#replace-java.lang.String-java.lang.String-com.aspose.note.TextStyle-) | 현재 인스턴스에서 지정된 문자열의 모든 발생을 지정된 스타일의 다른 지정된 문자열로 교체합니다. |
| [setAlignment(int value)](#setAlignment-int-) | 정렬을 설정합니다. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | 마지막 수정 시간을 설정합니다. |
| [setLineSpacing(float value)](#setLineSpacing-float-) |  |
| [setLineSpacing(Float value)](#setLineSpacing-java.lang.Float-) | 줄 간격을 설정합니다. |
| [setParagraphStyle(ParagraphStyle value)](#setParagraphStyle-com.aspose.note.ParagraphStyle-) | 단락 스타일을 설정합니다. |
| [setSpaceAfter(float value)](#setSpaceAfter-float-) |  |
| [setSpaceAfter(Float value)](#setSpaceAfter-java.lang.Float-) | 뒤쪽 최소 간격을 설정합니다. |
| [setSpaceBefore(float value)](#setSpaceBefore-float-) |  |
| [setSpaceBefore(Float value)](#setSpaceBefore-java.lang.Float-) | 앞에 최소 공간 양을 설정합니다. |
| [setText(String value)](#setText-java.lang.String-) | 텍스트를 설정합니다. |
| [trim()](#trim--) | 앞뒤의 모든 공백 문자를 제거합니다. |
| [trim(char trimChar)](#trim-char-) | 문자의 앞뒤 모든 인스턴스를 제거합니다. |
| [trim(char[] trimChars)](#trim-char...-) | 배열에 지정된 문자 집합의 앞뒤 모든 발생을 제거합니다. |
| [trimEnd()](#trimEnd--) | 뒤쪽의 모든 공백 문자를 제거합니다. |
| [trimEnd(char trimChar)](#trimEnd-char-) | 문자의 뒤쪽 모든 발생을 제거합니다. |
| [trimEnd(char[] trimChars)](#trimEnd-char...-) | 배열에 지정된 문자 집합의 뒤쪽 모든 발생을 제거합니다. |
| [trimStart()](#trimStart--) | 앞쪽의 모든 공백 문자를 제거합니다. |
| [trimStart(char trimChar)](#trimStart-char-) | 지정된 문자의 앞쪽 모든 발생을 제거합니다. |
| [trimStart(char[] trimChars)](#trimStart-char...-) | 배열에 지정된 문자 집합의 앞쪽 모든 발생을 제거합니다. |
### RichText() {#RichText--}
```
public RichText()
```


새 [RichText](../../com.aspose.note/richtext) 클래스 인스턴스를 초기화합니다.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


노드의 방문자를 수락합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | 다음으로부터 파생된 클래스인 [DocumentVisitor](../../com.aspose.note/documentvisitor)의 객체. |

### append(String value) {#append-java.lang.String-}
```
public RichText append(String value)
```


마지막 텍스트 범위에 문자열을 추가합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | 추가된 값입니다. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### append(String value, TextStyle style) {#append-java.lang.String-com.aspose.note.TextStyle-}
```
public final RichText append(String value, TextStyle style)
```


문자열을 끝에 추가합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | 추가된 값입니다. |
| style | [TextStyle](../../com.aspose.note/textstyle) | 추가된 문자열의 스타일입니다. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### appendFront(String value) {#appendFront-java.lang.String-}
```
public RichText appendFront(String value)
```


첫 번째 텍스트 범위의 앞에 문자열을 추가합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | 추가된 값입니다. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### appendFront(String value, TextStyle style) {#appendFront-java.lang.String-com.aspose.note.TextStyle-}
```
public RichText appendFront(String value, TextStyle style)
```


문자열을 앞에 추가합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | 추가된 값입니다. |
| style | [TextStyle](../../com.aspose.note/textstyle) | 추가된 문자열의 스타일입니다. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### clear() {#clear--}
```
public final RichText clear()
```


이 인스턴스의 내용을 지웁니다.

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### getAlignment() {#getAlignment--}
```
public int getAlignment()
```


정렬을 가져옵니다.

**Returns:**
int
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


마지막 수정 시간을 가져옵니다.

**Returns:**
java.util.Date
### getLength() {#getLength--}
```
public final int getLength()
```




**Returns:**
int
### getLineSpacing() {#getLineSpacing--}
```
public Float getLineSpacing()
```


줄 간격을 가져옵니다.

**Returns:**
java.lang.Float
### getParagraphStyle() {#getParagraphStyle--}
```
public final ParagraphStyle getParagraphStyle()
```


단락 스타일을 가져옵니다. 이 설정은 [getStyles](../../com.aspose.note/richtext\#getStyles) 컬렉션에 일치하는 TextStyle 객체가 없거나 이 객체가 필요한 설정을 지정하지 않은 경우에 사용됩니다.

**Returns:**
[ParagraphStyle](../../com.aspose.note/paragraphstyle)
### getSpaceAfter() {#getSpaceAfter--}
```
public Float getSpaceAfter()
```


뒤쪽 최소 간격을 가져옵니다.

**Returns:**
java.lang.Float
### getSpaceBefore() {#getSpaceBefore--}
```
public Float getSpaceBefore()
```


앞쪽 최소 간격을 가져옵니다.

**Returns:**
java.lang.Float
### getStyles() {#getStyles--}
```
public System.Collections.Generic.IGenericEnumerable<TextStyle> getStyles()
```


스타일을 가져옵니다.

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerable&lt;com.aspose.note.TextStyle&gt;
### getTags() {#getTags--}
```
public final System.Collections.Generic.List<ITag> getTags()
```


단락의 모든 태그 목록을 가져옵니다.

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.note.ITag&gt;
### getText() {#getText--}
```
public final String getText()
```


텍스트를 가져옵니다. 문자열에는 값 10(줄 바꿈) 문자가 포함되어서는 안 됩니다.

**Returns:**
java.lang.String
### getTextRuns() {#getTextRuns--}
```
public final System.Collections.Generic.IGenericEnumerable<TextRun> getTextRuns()
```




**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerable&lt;com.aspose.note.TextRun&gt;
### indexOf(char value) {#indexOf-char-}
```
public final int indexOf(char value)
```


이 문자열에서 지정된 유니코드 문자의 첫 번째 발생 위치의 0부터 시작하는 인덱스를 반환합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | char | 값입니다. |

**Returns:**
int - `int`입니다.
### indexOf(char value, int startIndex) {#indexOf-char-int-}
```
public final int indexOf(char value, int startIndex)
```


이 문자열에서 지정된 유니코드 문자의 첫 번째 발생 위치를 0부터 시작하는 인덱스로 반환합니다. 검색은 지정된 문자 위치에서 시작합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | char | 값입니다. |
| startIndex | int | 시작 검색 위치 |

**Returns:**
int - `int`입니다.
### indexOf(char value, int startIndex, int count) {#indexOf-char-int-int-}
```
public final int indexOf(char value, int startIndex, int count)
```


이 인스턴스에서 지정된 문자의 첫 번째 발생 위치를 0부터 시작하는 인덱스로 반환합니다. 검색은 지정된 문자 위치에서 시작하며 지정된 문자 수만큼 검사합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | char | 값입니다. |
| startIndex | int | 시작 검색 위치 |
| count | int | 카운트입니다. |

**Returns:**
int - `int`입니다.
### indexOf(String value) {#indexOf-java.lang.String-}
```
public final int indexOf(String value)
```


이 인스턴스에서 지정된 문자열의 첫 번째 발생 위치의 0부터 시작하는 인덱스를 반환합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | 값입니다. |

**Returns:**
int - `int`입니다.
### indexOf(String value, int startIndex) {#indexOf-java.lang.String-int-}
```
public final int indexOf(String value, int startIndex)
```


이 인스턴스에서 지정된 문자열이 처음 나타나는 위치의 0부터 시작하는 인덱스를 반환합니다. 검색은 지정된 문자 위치에서 시작합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | 값입니다. |
| startIndex | int | 시작 검색 위치 |

**Returns:**
int - `int`입니다.
### indexOf(String value, int startIndex, int count) {#indexOf-java.lang.String-int-int-}
```
public final int indexOf(String value, int startIndex, int count)
```


이 인스턴스에서 지정된 문자열이 처음 나타나는 위치의 0부터 시작하는 인덱스를 반환합니다. 검색은 지정된 문자 위치에서 시작하고 지정된 문자 수만큼 검사합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | 값입니다. |
| startIndex | int | 시작 검색 위치 |
| count | int | 카운트입니다. |

**Returns:**
int - `int`입니다.
### indexOf(String value, int startIndex, int count, short comparisonType) {#indexOf-java.lang.String-int-int-short-}
```
public final int indexOf(String value, int startIndex, int count, short comparisonType)
```


현재 인스턴스에서 지정된 문자열의 첫 번째 발생 위치의 0부터 시작하는 인덱스를 반환합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | 값입니다. |
| startIndex | int | 시작 검색 위치 |
| count | int | 카운트입니다. |
| comparisonType | short | 지정된 문자열에 사용할 검색 유형 |

**Returns:**
int - `int`입니다.
### indexOf(String value, short comparisonType) {#indexOf-java.lang.String-short-}
```
public final int indexOf(String value, short comparisonType)
```


현재 인스턴스에서 지정된 문자열이 처음 나타나는 위치의 0부터 시작하는 인덱스를 반환합니다. 매개변수는 지정된 문자열에 사용할 검색 유형을 지정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | 값입니다. |
| comparisonType | short | 지정된 문자열에 사용할 검색 유형 |

**Returns:**
int - `int`입니다.
### indexOf_Rename_Namesake(String value, int startIndex, short comparisonType) {#indexOf-Rename-Namesake-java.lang.String-int-short-}
```
public final int indexOf_Rename_Namesake(String value, int startIndex, short comparisonType)
```


현재 인스턴스에서 지정된 문자열이 처음 나타나는 위치의 0부터 시작하는 인덱스를 반환합니다. 매개변수는 현재 문자열에서 검색 시작 위치와 지정된 문자열에 사용할 검색 유형을 지정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | 값입니다. |
| startIndex | int | 시작 검색 위치 |
| comparisonType | short | 지정된 문자열에 사용할 검색 유형 |

**Returns:**
int - `int`입니다.
### insert(int startIndex, String value) {#insert-int-java.lang.String-}
```
public final RichText insert(int startIndex, String value)
```


이 인스턴스의 지정된 인덱스 위치에 지정된 문자열을 삽입합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| startIndex | int | 시작 인덱스. |
| 값 | java.lang.String | 값입니다. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### insert(int startIndex, String value, TextStyle style) {#insert-int-java.lang.String-com.aspose.note.TextStyle-}
```
public final RichText insert(int startIndex, String value, TextStyle style)
```


이 인스턴스의 지정된 인덱스 위치에 지정된 스타일을 가진 문자열을 삽입합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| startIndex | int | 시작 인덱스. |
| 값 | java.lang.String | 값입니다. |
| style | [TextStyle](../../com.aspose.note/textstyle) | 스타일. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<Character> iterator()
```




**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator&lt;java.lang.Character&gt;
### remove(int startIndex) {#remove-int-}
```
public final RichText remove(int startIndex)
```


현재 인스턴스에서 지정된 위치부터 마지막 위치까지 모든 문자를 제거합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| startIndex | int | 시작 인덱스. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### remove(int startIndex, int count) {#remove-int-int-}
```
public final RichText remove(int startIndex, int count)
```


현재 인스턴스에서 지정된 위치부터 지정된 수만큼의 문자를 제거합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| startIndex | int | 시작 인덱스. |
| count | int | 카운트입니다. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### replace(char oldChar, char newChar) {#replace-char-char-}
```
public final RichText replace(char oldChar, char newChar)
```


이 인스턴스에서 지정된 유니코드 문자의 모든 발생을 다른 지정된 유니코드 문자로 교체합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| oldChar | char | 이전 문자. |
| newChar | char | 새 문자. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### replace(String oldValue, String newValue) {#replace-java.lang.String-java.lang.String-}
```
public final RichText replace(String oldValue, String newValue)
```


현재 인스턴스에서 지정된 문자열의 모든 발생을 다른 지정된 문자열로 교체합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| oldValue | java.lang.String | 이전 값. |
| newValue | java.lang.String | 새 값. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### replace(String oldValue, String newValue, TextStyle style) {#replace-java.lang.String-java.lang.String-com.aspose.note.TextStyle-}
```
public final RichText replace(String oldValue, String newValue, TextStyle style)
```


현재 인스턴스에서 지정된 문자열의 모든 발생을 지정된 스타일의 다른 지정된 문자열로 교체합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| oldValue | java.lang.String | 이전 값. |
| newValue | java.lang.String | 새 값. |
| style | [TextStyle](../../com.aspose.note/textstyle) | 새 값의 스타일. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### setAlignment(int value) {#setAlignment-int-}
```
public void setAlignment(int value)
```


정렬을 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | int |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


마지막 수정 시간을 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.util.Date |  |

### setLineSpacing(float value) {#setLineSpacing-float-}
```
public void setLineSpacing(float value)
```




**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | float |  |

### setLineSpacing(Float value) {#setLineSpacing-java.lang.Float-}
```
public void setLineSpacing(Float value)
```


줄 간격을 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.lang.Float |  |

### setParagraphStyle(ParagraphStyle value) {#setParagraphStyle-com.aspose.note.ParagraphStyle-}
```
public final void setParagraphStyle(ParagraphStyle value)
```


단락 스타일을 설정합니다. 이 설정은 [getStyles](../../com.aspose.note/richtext\#getStyles) 컬렉션에 일치하는 TextStyle 객체가 없거나, 해당 객체가 필요한 설정을 지정하지 않은 경우에 사용됩니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| value | [ParagraphStyle](../../com.aspose.note/paragraphstyle) |  |

### setSpaceAfter(float value) {#setSpaceAfter-float-}
```
public void setSpaceAfter(float value)
```




**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | float |  |

### setSpaceAfter(Float value) {#setSpaceAfter-java.lang.Float-}
```
public void setSpaceAfter(Float value)
```


뒤쪽 최소 간격을 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.lang.Float |  |

### setSpaceBefore(float value) {#setSpaceBefore-float-}
```
public void setSpaceBefore(float value)
```




**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | float |  |

### setSpaceBefore(Float value) {#setSpaceBefore-java.lang.Float-}
```
public void setSpaceBefore(Float value)
```


앞에 최소 공간 양을 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.lang.Float |  |

### setText(String value) {#setText-java.lang.String-}
```
public final void setText(String value)
```


텍스트를 설정합니다. 문자열에는 값 10(줄 바꿈) 문자가 포함되어서는 안 됩니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String |  |

### trim() {#trim--}
```
public final RichText trim()
```


앞뒤의 모든 공백 문자를 제거합니다.

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trim(char trimChar) {#trim-char-}
```
public final RichText trim(char trimChar)
```


문자의 앞뒤 모든 인스턴스를 제거합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| trimChar | char | 잘라낼 문자. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trim(char[] trimChars) {#trim-char...-}
```
public final RichText trim(char[] trimChars)
```


배열에 지정된 문자 집합의 앞뒤 모든 발생을 제거합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| trimChars | char[] | 잘라내기 문자. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimEnd() {#trimEnd--}
```
public final RichText trimEnd()
```


뒤쪽의 모든 공백 문자를 제거합니다.

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimEnd(char trimChar) {#trimEnd-char-}
```
public final RichText trimEnd(char trimChar)
```


문자의 뒤쪽 모든 발생을 제거합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| trimChar | char | 잘라낼 문자. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimEnd(char[] trimChars) {#trimEnd-char...-}
```
public final RichText trimEnd(char[] trimChars)
```


배열에 지정된 문자 집합의 뒤쪽 모든 발생을 제거합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| trimChars | char[] | 잘라내기 문자. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimStart() {#trimStart--}
```
public final RichText trimStart()
```


앞쪽의 모든 공백 문자를 제거합니다.

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimStart(char trimChar) {#trimStart-char-}
```
public final RichText trimStart(char trimChar)
```


지정된 문자의 앞쪽 모든 발생을 제거합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| trimChar | char | 잘라낼 문자. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
### trimStart(char[] trimChars) {#trimStart-char...-}
```
public final RichText trimStart(char[] trimChars)
```


배열에 지정된 문자 집합의 앞쪽 모든 발생을 제거합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| trimChars | char[] | 잘라내기 문자. |

**Returns:**
[RichText](../../com.aspose.note/richtext) - The [RichText](../../com.aspose.note/richtext).
