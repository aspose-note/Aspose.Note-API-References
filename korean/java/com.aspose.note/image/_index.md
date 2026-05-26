---
title: "이미지"
second_title: "Java용 Aspose.Note API 레퍼런스"
description: "이미지를 나타냅니다."
type: docs
weight: 33
url: /ko/java/com.aspose.note/image/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode

**All Implemented Interfaces:**
[com.aspose.note.IPageChildNode](../../com.aspose.note/ipagechildnode), [com.aspose.note.IOutlineElementChildNode](../../com.aspose.note/ioutlineelementchildnode), [com.aspose.note.ITaggable](../../com.aspose.note/itaggable)
```
public final class Image extends CompositeNode<Loop> implements IPageChildNode, IOutlineElementChildNode, ITaggable
```

이미지를 나타냅니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [Image(String path)](#Image-java.lang.String-) | `Image` 클래스의 새 인스턴스를 초기화합니다. |
| [Image(String fileName, InputStream imageStream)](#Image-java.lang.String-java.io.InputStream-) | `Image` 클래스의 새 인스턴스를 초기화합니다. |
| [Image()](#Image--) | `Image` 클래스의 새 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | 노드의 방문자를 수락합니다. |
| [getAlignment()](#getAlignment--) | 정렬을 가져옵니다. |
| [getAlternativeTextDescription()](#getAlternativeTextDescription--) | 이미지에 대한 본문 대체 텍스트를 가져옵니다. |
| [getAlternativeTextTitle()](#getAlternativeTextTitle--) | 이미지에 대한 대체 텍스트의 제목을 가져옵니다. |
| [getBytes()](#getBytes--) | 이미지 데이터 저장소를 가져옵니다. |
| [getFileName()](#getFileName--) | 파일 이름을 가져옵니다. |
| [getFilePath()](#getFilePath--) | 이미지 파일 경로를 가져옵니다. |
| [getFormat()](#getFormat--) | 이미지 형식을 가져옵니다. |
| [getHeight()](#getHeight--) | 높이를 가져옵니다. |
| [getHorizontalOffset()](#getHorizontalOffset--) | 수평 오프셋을 가져옵니다. |
| [getHyperlinkUrl()](#getHyperlinkUrl--) | 이미지와 연결된 하이퍼링크를 가져옵니다. |
| [getLastModifiedTime()](#getLastModifiedTime--) | 마지막 수정 시간을 가져옵니다. |
| [getOriginalHeight()](#getOriginalHeight--) | 원본 높이를 가져옵니다. |
| [getOriginalWidth()](#getOriginalWidth--) | 원본 너비를 가져옵니다. |
| [getTags()](#getTags--) | 이미지의 모든 태그 목록을 가져옵니다. |
| [getVerticalOffset()](#getVerticalOffset--) | 수직 오프셋을 가져옵니다. |
| [getWidth()](#getWidth--) | 너비를 가져옵니다. |
| [isBackground()](#isBackground--) | 이미지가 배경 이미지인지 여부를 가져옵니다. |
| [replace(Image newImage)](#replace-com.aspose.note.Image-) | 제공된 Image 객체의 데이터로 현재 이미지 데이터를 교체합니다. |
| [setAlignment(int value)](#setAlignment-int-) | 정렬을 설정합니다. |
| [setAlternativeTextDescription(String value)](#setAlternativeTextDescription-java.lang.String-) | 이미지에 대한 본문 대체 텍스트를 설정합니다. |
| [setAlternativeTextTitle(String value)](#setAlternativeTextTitle-java.lang.String-) | 이미지에 대한 대체 텍스트의 제목을 설정합니다. |
| [setBackground(boolean value)](#setBackground-boolean-) | 이미지가 배경 이미지인지 여부를 가져옵니다. |
| [setHeight(float value)](#setHeight-float-) | 높이를 설정합니다. |
| [setHorizontalOffset(float value)](#setHorizontalOffset-float-) | 수평 오프셋을 설정합니다. |
| [setHyperlinkUrl(String value)](#setHyperlinkUrl-java.lang.String-) | 이미지와 연결된 하이퍼링크를 설정합니다. |
| [setLastModifiedTime(Date value)](#setLastModifiedTime-java.util.Date-) | 마지막 수정 시간을 설정합니다. |
| [setVerticalOffset(float value)](#setVerticalOffset-float-) | 수직 오프셋을 설정합니다. |
| [setWidth(float value)](#setWidth-float-) | 너비를 설정합니다. |
### Image(String path) {#Image-java.lang.String-}
```
public Image(String path)
```


`Image` 클래스의 새 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 경로 | java.lang.String | `Image`를 생성할 파일의 경로를 포함하는 문자열입니다. |

### Image(String fileName, InputStream imageStream) {#Image-java.lang.String-java.io.InputStream-}
```
public Image(String fileName, InputStream imageStream)
```


`Image` 클래스의 새 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 파일이름 | java.lang.String | 이미지의 이름입니다. |
| imageStream | java.io.InputStream | 이미지를 포함하는 스트림입니다. |

### Image() {#Image--}
```
public Image()
```


`Image` 클래스의 새 인스턴스를 초기화합니다.

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


이미지에 대한 본문 대체 텍스트를 가져옵니다.

**Returns:**
java.lang.String
### getAlternativeTextTitle() {#getAlternativeTextTitle--}
```
public final String getAlternativeTextTitle()
```


이미지에 대한 대체 텍스트의 제목을 가져옵니다.

**Returns:**
java.lang.String
### getBytes() {#getBytes--}
```
public byte[] getBytes()
```


이미지 데이터 저장소를 가져옵니다.

**Returns:**
byte[]
### getFileName() {#getFileName--}
```
public String getFileName()
```


파일 이름을 가져옵니다.

**Returns:**
java.lang.String
### getFilePath() {#getFilePath--}
```
public String getFilePath()
```


이미지 파일 경로를 가져옵니다.

**Returns:**
java.lang.String
### getFormat() {#getFormat--}
```
public final System.Drawing.Imaging.ImageFormat getFormat()
```


이미지 형식을 가져옵니다.

**Returns:**
com.aspose.ms.System.Drawing.Imaging.ImageFormat
### getHeight() {#getHeight--}
```
public final float getHeight()
```


높이를 가져옵니다. 이는 MS OneNote 문서에서 이미지의 실제 높이입니다.

**Returns:**
float
### getHorizontalOffset() {#getHorizontalOffset--}
```
public float getHorizontalOffset()
```


수평 오프셋을 가져옵니다.

**Returns:**
float
### getHyperlinkUrl() {#getHyperlinkUrl--}
```
public String getHyperlinkUrl()
```


이미지와 연결된 하이퍼링크를 가져옵니다.

**Returns:**
java.lang.String
### getLastModifiedTime() {#getLastModifiedTime--}
```
public Date getLastModifiedTime()
```


마지막 수정 시간을 가져옵니다.

**Returns:**
java.util.Date
### getOriginalHeight() {#getOriginalHeight--}
```
public float getOriginalHeight()
```


원본 높이를 가져옵니다. 이는 크기 조정 전 이미지의 원본 너비입니다.

**Returns:**
float
### getOriginalWidth() {#getOriginalWidth--}
```
public float getOriginalWidth()
```


원본 너비를 가져옵니다. 이는 크기 조정 전 이미지의 원본 너비입니다.

**Returns:**
float
### getTags() {#getTags--}
```
public final System.Collections.Generic.List<ITag> getTags()
```


이미지의 모든 태그 목록을 가져옵니다.

**Returns:**
com.aspose.ms.System.Collections.Generic.List&lt;com.aspose.note.ITag&gt;
### getVerticalOffset() {#getVerticalOffset--}
```
public float getVerticalOffset()
```


수직 오프셋을 가져옵니다.

**Returns:**
float
### getWidth() {#getWidth--}
```
public final float getWidth()
```


너비를 가져옵니다. 이는 MS OneNote 문서에서 이미지의 실제 너비입니다.

**Returns:**
float
### isBackground() {#isBackground--}
```
public final boolean isBackground()
```


이미지가 배경 이미지인지 여부를 가져옵니다.

**Returns:**
boolean
### replace(Image newImage) {#replace-com.aspose.note.Image-}
```
public void replace(Image newImage)
```


제공된 Image 객체의 데이터로 현재 이미지 데이터를 교체합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| newImage | [Image](../../com.aspose.note/image) |  |

### setAlignment(int value) {#setAlignment-int-}
```
public void setAlignment(int value)
```


정렬을 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | int |  |

### setAlternativeTextDescription(String value) {#setAlternativeTextDescription-java.lang.String-}
```
public final void setAlternativeTextDescription(String value)
```


이미지에 대한 본문 대체 텍스트를 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String |  |

### setAlternativeTextTitle(String value) {#setAlternativeTextTitle-java.lang.String-}
```
public final void setAlternativeTextTitle(String value)
```


이미지에 대한 대체 텍스트의 제목을 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String |  |

### setBackground(boolean value) {#setBackground-boolean-}
```
public final void setBackground(boolean value)
```


이미지가 배경 이미지인지 여부를 가져옵니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | boolean |  |

### setHeight(float value) {#setHeight-float-}
```
public final void setHeight(float value)
```


높이를 설정합니다. 이는 MS OneNote 문서에서 이미지의 실제 높이입니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | float |  |

### setHorizontalOffset(float value) {#setHorizontalOffset-float-}
```
public void setHorizontalOffset(float value)
```


수평 오프셋을 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | float |  |

### setHyperlinkUrl(String value) {#setHyperlinkUrl-java.lang.String-}
```
public void setHyperlinkUrl(String value)
```


이미지와 연결된 하이퍼링크를 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String |  |

### setLastModifiedTime(Date value) {#setLastModifiedTime-java.util.Date-}
```
public void setLastModifiedTime(Date value)
```


마지막 수정 시간을 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.util.Date |  |

### setVerticalOffset(float value) {#setVerticalOffset-float-}
```
public void setVerticalOffset(float value)
```


수직 오프셋을 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | float |  |

### setWidth(float value) {#setWidth-float-}
```
public final void setWidth(float value)
```


너비를 설정합니다. 이는 MS OneNote 문서에서 이미지의 실제 너비입니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | float |  |

