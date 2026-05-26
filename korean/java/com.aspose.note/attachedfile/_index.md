---
title: "AttachedFile"
second_title: "Java용 Aspose.Note API 레퍼런스"
description: "첨부 파일을 나타냅니다."
type: docs
weight: 11
url: /ko/java/com.aspose.note/attachedfile/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node)

**All Implemented Interfaces:**
[com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode), [com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode), [com.aspose.note.ITaggable](../../com.aspose.note/itaggable)
```
public class AttachedFile extends Node implements IPageChildNode, IOutlineElementChildNode, ITaggable
```

첨부 파일을 나타냅니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [AttachedFile(String path)](#AttachedFile-java.lang.String-) | 새 `AttachedFile` 클래스 인스턴스를 초기화합니다. |
| [AttachedFile(String path, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)](#AttachedFile-java.lang.String-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-) | 새 `AttachedFile` 클래스 인스턴스를 초기화합니다. |
| [AttachedFile(String fileName, InputStream attachedFileStream)](#AttachedFile-java.lang.String-java.io.InputStream-) | 새 `AttachedFile` 클래스 인스턴스를 초기화합니다. |
| [AttachedFile(String fileName, InputStream attachedFileStream, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)](#AttachedFile-java.lang.String-java.io.InputStream-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-) | 새 `AttachedFile` 클래스 인스턴스를 초기화합니다. |
| [AttachedFile()](#AttachedFile--) | 새 `AttachedFile` 클래스 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | 노드의 방문자를 수락합니다. |
| [getAlignment()](#getAlignment--) | 정렬을 가져옵니다. |
| [getAlternativeTextDescription()](#getAlternativeTextDescription--) | 첨부 파일 아이콘에 대한 본문 대체 텍스트를 가져오거나 설정합니다. |
| [getAlternativeTextTitle()](#getAlternativeTextTitle--) | 첨부 파일 아이콘에 대한 대체 텍스트의 제목을 가져오거나 설정합니다. |
| [getBytes()](#getBytes--) | 임베드된 파일의 바이너리 데이터를 가져옵니다. |
| [getExtension()](#getExtension--) | 임베드된 파일의 확장자를 가져옵니다. |
| [getFileName()](#getFileName--) | 임베드된 파일의 이름을 가져옵니다. |
| [getFilePath()](#getFilePath--) | 원본 파일의 경로를 가져옵니다. |
| [getHeight()](#getHeight--) | 임베드된 파일 아이콘의 원본 높이를 가져옵니다. |
| [getHorizontalOffset()](#getHorizontalOffset--) | 수평 오프셋을 가져옵니다. |
| [getIcon()](#getIcon--) | 임베드된 파일과 연결된 아이콘의 바이너리 데이터를 가져옵니다. |
| [getIconExtension()](#getIconExtension--) | 아이콘의 확장자를 가져옵니다. |
| [getLastModifiedTime()](#getLastModifiedTime--) | 마지막 수정 시간을 가져옵니다. |
| [getMaxHeight()](#getMaxHeight--) | 삽입된 파일 아이콘을 표시하기 위한 최대 높이를 가져옵니다. |
| [getMaxWidth()](#getMaxWidth--) | 삽입된 파일 아이콘을 표시하기 위한 최대 너비를 가져옵니다. |
| [getParsingErrorInfo()](#getParsingErrorInfo--) | 파일에 접근하는 동안 발생한 오류에 대한 데이터를 가져옵니다. |
| [getTags()](#getTags--) | 첨부된 파일의 태그 목록을 가져옵니다. |
| [getText()](#getText--) | 삽입된 파일의 텍스트 표현을 가져옵니다. |
| [getVerticalOffset()](#getVerticalOffset--) | 수직 오프셋을 가져옵니다. |
| [getWidth()](#getWidth--) | 삽입된 파일 아이콘의 원래 너비를 가져옵니다. |
| [isPrintout()](#isPrintout--) | 파일 보기 방식이 인쇄물인지 여부를 나타내는 값을 가져옵니다. |
| [isSizeSetByUser()](#isSizeSetByUser--) | 아이콘 크기 값이 사용자가 명시적으로 업데이트했는지 여부를 나타내는 값을 가져옵니다. |
| [setAlignment(int value)](#setAlignment-int-) | 정렬을 설정합니다. |
| [setAlternativeTextDescription(String value)](#setAlternativeTextDescription-java.lang.String-) | 첨부 파일 아이콘에 대한 본문 대체 텍스트를 가져오거나 설정합니다. |
| [setAlternativeTextTitle(String value)](#setAlternativeTextTitle-java.lang.String-) | 첨부 파일 아이콘에 대한 대체 텍스트의 제목을 가져오거나 설정합니다. |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | 수평 오프셋을 설정합니다. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | 마지막 수정 시간을 설정합니다. |
| [setMaxHeight(float value)](#setMaxHeight-float-) | 삽입된 파일 아이콘을 표시하기 위한 최대 높이를 설정합니다. |
| [setMaxWidth(float value)](#setMaxWidth-float-) | 삽입된 파일 아이콘을 표시하기 위한 최대 너비를 설정합니다. |
| [setPrintout(boolean value)](#setPrintout-boolean-) | 파일 보기 방식이 인쇄물인지 여부를 나타내는 값을 설정합니다. |
| [setSizeSetByUser(boolean value)](#setSizeSetByUser-boolean-) | 아이콘 크기 값이 사용자가 명시적으로 업데이트했는지 여부를 나타내는 값을 설정합니다. |
| [setText(String value)](#setText-java.lang.String-) | 삽입된 파일의 텍스트 표현을 설정합니다. |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | 수직 오프셋을 설정합니다. |
### AttachedFile(String path) {#AttachedFile-java.lang.String-}
```
public AttachedFile(String path)
```


새 `AttachedFile` 클래스 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 경로 | java.lang.String | `AttachedFile`을 생성할 파일의 경로를 포함하는 문자열입니다. |

### AttachedFile(String path, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat) {#AttachedFile-java.lang.String-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-}
```
public AttachedFile(String path, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)
```


새 `AttachedFile` 클래스 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 경로 | java.lang.String | `AttachedFile`을 생성할 파일의 경로를 포함하는 문자열입니다. |
| 아이콘 | java.io.InputStream | 첨부된 파일에 대한 아이콘입니다. |
| 아이콘형식 | com.aspose.ms.System.Drawing.Imaging.ImageFormat |  |

### AttachedFile(String fileName, InputStream attachedFileStream) {#AttachedFile-java.lang.String-java.io.InputStream-}
```
public AttachedFile(String fileName, InputStream attachedFileStream)
```


새 `AttachedFile` 클래스 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 파일이름 | java.lang.String | 첨부된 파일의 이름. |
| attachedFileStream | java.io.InputStream | 첨부된 파일 바이트를 포함하는 스트림. |

### AttachedFile(String fileName, InputStream attachedFileStream, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat) {#AttachedFile-java.lang.String-java.io.InputStream-java.io.InputStream-com.aspose.ms.System.Drawing.Imaging.ImageFormat-}
```
public AttachedFile(String fileName, InputStream attachedFileStream, InputStream icon, System.Drawing.Imaging.ImageFormat iconFormat)
```


새 `AttachedFile` 클래스 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 파일이름 | java.lang.String | 첨부된 파일의 이름. |
| attachedFileStream | java.io.InputStream | 첨부된 파일 바이트를 포함하는 스트림. |
| 아이콘 | java.io.InputStream | 첨부된 파일에 대한 아이콘입니다. |
| 아이콘형식 | com.aspose.ms.System.Drawing.Imaging.ImageFormat | 첨부된 파일 아이콘의 형식. |

### AttachedFile() {#AttachedFile--}
```
public AttachedFile()
```


새 `AttachedFile` 클래스 인스턴스를 초기화합니다.

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


노드의 방문자를 수락합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | `DocumentVisitor`에서 파생된 클래스의 객체. |

### getAlignment() {#getAlignment--}
```
public int getAlignment()
```


정렬을 가져옵니다.

**Returns:**
int
### getAlternativeTextDescription() {#getAlternativeTextDescription--}
```
public final String getAlternativeTextDescription()
```


첨부 파일 아이콘에 대한 본문 대체 텍스트를 가져오거나 설정합니다.

**Returns:**
java.lang.String
### getAlternativeTextTitle() {#getAlternativeTextTitle--}
```
public final String getAlternativeTextTitle()
```


첨부 파일 아이콘에 대한 대체 텍스트의 제목을 가져오거나 설정합니다.

**Returns:**
java.lang.String
### getBytes() {#getBytes--}
```
public byte[] getBytes()
```


임베드된 파일의 바이너리 데이터를 가져옵니다.

**Returns:**
byte[]
### getExtension() {#getExtension--}
```
public String getExtension()
```


임베드된 파일의 확장자를 가져옵니다.

**Returns:**
java.lang.String
### getFileName() {#getFileName--}
```
public String getFileName()
```


임베드된 파일의 이름을 가져옵니다.

**Returns:**
java.lang.String
### getFilePath() {#getFilePath--}
```
public String getFilePath()
```


원본 파일의 경로를 가져옵니다.

**Returns:**
java.lang.String
### getHeight() {#getHeight--}
```
public float getHeight()
```


임베드된 파일 아이콘의 원본 높이를 가져옵니다.

**Returns:**
float
### getHorizontalOffset() {#getHorizontalOffset--}
```
public float getHorizontalOffset()
```


수평 오프셋을 가져옵니다.

**Returns:**
float
### getIcon() {#getIcon--}
```
public byte[] getIcon()
```


임베드된 파일과 연결된 아이콘의 바이너리 데이터를 가져옵니다.

**Returns:**
byte[]
### getIconExtension() {#getIconExtension--}
```
public String getIconExtension()
```


아이콘의 확장자를 가져옵니다.

**Returns:**
java.lang.String
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


마지막 수정 시간을 가져옵니다.

**Returns:**
java.util.Date
### getMaxHeight() {#getMaxHeight--}
```
public float getMaxHeight()
```


삽입된 파일 아이콘을 표시하기 위한 최대 높이를 가져옵니다.

**Returns:**
float
### getMaxWidth() {#getMaxWidth--}
```
public float getMaxWidth()
```


삽입된 파일 아이콘을 표시하기 위한 최대 너비를 가져옵니다.

**Returns:**
float
### getParsingErrorInfo() {#getParsingErrorInfo--}
```
public final ParsingErrorInfo getParsingErrorInfo()
```


파일에 접근하는 동안 발생한 오류에 대한 데이터를 가져옵니다.

**Returns:**
[ParsingErrorInfo](../../com.aspose.note.infrastructure/parsingerrorinfo)
### getTags() {#getTags--}
```
public final System.Collections.Generic.List<ITag> getTags()
```


첨부된 파일의 태그 목록을 가져옵니다.

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.note.ITag&gt;
### getText() {#getText--}
```
public String getText()
```


임베드된 파일의 텍스트 표현을 가져옵니다. 문자열은 값 10(줄 바꿈) 또는 13(캐리지 리턴)의 문자를 절대 포함해서는 안 됩니다.

**Returns:**
java.lang.String
### getVerticalOffset() {#getVerticalOffset--}
```
public float getVerticalOffset()
```


수직 오프셋을 가져옵니다.

**Returns:**
float
### getWidth() {#getWidth--}
```
public float getWidth()
```


삽입된 파일 아이콘의 원래 너비를 가져옵니다.

**Returns:**
float
### isPrintout() {#isPrintout--}
```
public boolean isPrintout()
```


파일 보기 방식이 인쇄물인지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean
### isSizeSetByUser() {#isSizeSetByUser--}
```
public boolean isSizeSetByUser()
```


아이콘 크기 값이 사용자가 명시적으로 업데이트했는지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean
### setAlignment(int value) {#setAlignment-int-}
```
public void setAlignment(int value)
```


정렬을 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | int | Alignment의 값. |

### setAlternativeTextDescription(String value) {#setAlternativeTextDescription-java.lang.String-}
```
public final void setAlternativeTextDescription(String value)
```


첨부 파일 아이콘에 대한 본문 대체 텍스트를 가져오거나 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String |  |

### setAlternativeTextTitle(String value) {#setAlternativeTextTitle-java.lang.String-}
```
public final void setAlternativeTextTitle(String value)
```


첨부 파일 아이콘에 대한 대체 텍스트의 제목을 가져오거나 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String |  |

### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public void setHorizontalOffset(float value)
```


수평 오프셋을 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | float | Offsets의 값. |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


마지막 수정 시간을 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.util.Date | Date의 값. |

### setMaxHeight(float value) {#setMaxHeight-float-}
```
public void setMaxHeight(float value)
```


삽입된 파일 아이콘을 표시하기 위한 최대 높이를 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | float | Maximum height의 값. |

### setMaxWidth(float value) {#setMaxWidth-float-}
```
public void setMaxWidth(float value)
```


삽입된 파일 아이콘을 표시하기 위한 최대 너비를 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | float | Maximum width의 값. |

### setPrintout(boolean value) {#setPrintout-boolean-}
```
public void setPrintout(boolean value)
```


파일 보기 방식이 인쇄물인지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | boolean | 새 값. |

### setSizeSetByUser(boolean value) {#setSizeSetByUser-boolean-}
```
public void setSizeSetByUser(boolean value)
```


아이콘 크기 값이 사용자가 명시적으로 업데이트했는지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | boolean | 새 값. |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


임베드된 파일의 텍스트 표현을 설정합니다. 문자열은 값 10(줄 바꿈) 또는 13(캐리지 리턴)의 문자를 절대 포함해서는 안 됩니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | Text의 값. |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public void setVerticalOffset(float value)
```


수직 오프셋을 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | float | Offset의 값. |

