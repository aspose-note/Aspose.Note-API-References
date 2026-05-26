---
title: "Document"
second_title: "Java용 Aspose.Note API 레퍼런스"
description: "Aspose.Note 문서를 나타냅니다."
type: docs
weight: 20
url: /ko/java/com.aspose.note/document/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode

**All Implemented Interfaces:**
[com.aspose.note.INotebookChildNode](../../com.aspose.note/inotebookchildnode)
```
public class Document extends CompositeNode<Page> implements INotebookChildNode
```

Aspose.Note 문서를 나타냅니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [Document()](#Document--) | 새 인스턴스를 초기화합니다 `Document` 클래스. |
| [Document(String filePath)](#Document-java.lang.String-) | 새 인스턴스를 초기화합니다 `Document` 클래스. |
| [Document(String filePath, LoadOptions loadOptions)](#Document-java.lang.String-com.aspose.note.LoadOptions-) | 새 인스턴스를 초기화합니다 `Document` 클래스. |
| [Document(InputStream inStream)](#Document-java.io.InputStream-) | 새 인스턴스를 초기화합니다 `Document` 클래스. |
| [Document(InputStream inStream, LoadOptions loadOptions)](#Document-java.io.InputStream-com.aspose.note.LoadOptions-) | 새 인스턴스를 초기화합니다 `Document` 클래스. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | 노드의 방문자를 수락합니다. |
| [detectLayoutChanges()](#detectLayoutChanges--) | 이전 `DetectLayoutChanges` 호출 이후 문서 레이아웃에 발생한 모든 변경 사항을 감지합니다. |
| [getAutomaticLayoutChangesDetectionEnabled()](#getAutomaticLayoutChangesDetectionEnabled--) | Aspose.Note가 레이아웃 변경 감지를 자동으로 수행하는지 여부를 나타내는 값을 가져옵니다. |
| [getColor()](#getColor--) | 색상을 가져옵니다. |
| [getCreationTime()](#getCreationTime--) | 생성 시간을 가져옵니다. |
| [getDisplayName()](#getDisplayName--) | 표시 이름을 가져옵니다. |
| [getFileFormat()](#getFileFormat--) | 파일 형식을 가져옵니다 (OneNote 2010, OneNote Online). |
| [getGuid()](#getGuid--) | 객체의 전역 고유 ID를 가져옵니다. |
| [getGuidInternal()](#getGuidInternal--) |  |
| [getPageHistory(Page page)](#getPageHistory-com.aspose.note.Page-) | `PageHistory`를 가져옵니다. 이 객체는 문서에 표시된 각 페이지에 대한 전체 기록을 포함합니다(가장 오래된 것이 인덱스 0에 있습니다). |
| [isEncrypted(InputStream stream, Document[] document)](#isEncrypted-java.io.InputStream-com.aspose.note.Document---) | 스트림에서 가져온 문서가 암호화되었는지 확인합니다. |
| [isEncrypted(InputStream stream, LoadOptions options, Document[] document)](#isEncrypted-java.io.InputStream-com.aspose.note.LoadOptions-com.aspose.note.Document---) | 스트림에서 가져온 문서가 암호화되었는지 확인합니다. |
| [isEncrypted(InputStream stream, String password, Document[] document)](#isEncrypted-java.io.InputStream-java.lang.String-com.aspose.note.Document---) | 스트림에서 가져온 문서가 암호화되었는지 확인합니다. |
| [isEncrypted(String filePath, Document[] document)](#isEncrypted-java.lang.String-com.aspose.note.Document---) | 파일에서 가져온 문서가 암호화되었는지 확인합니다. |
| [isEncrypted(String filePath, LoadOptions options, Document[] document)](#isEncrypted-java.lang.String-com.aspose.note.LoadOptions-com.aspose.note.Document---) | 파일에서 가져온 문서가 암호화되었는지 확인합니다. |
| [isEncrypted(String filePath, String password, Document[] document)](#isEncrypted-java.lang.String-java.lang.String-com.aspose.note.Document---) | 파일에서 가져온 문서가 암호화되었는지 확인합니다. |
| [print()](#print--) | 기본 프린터를 사용하여 문서를 인쇄합니다. |
| [print(PrintOptions options)](#print-com.aspose.note.PrintOptions-) | 기본 프린터를 사용하여 문서를 인쇄합니다. |
| [print(String printerName)](#print-java.lang.String-) | 기본 프린터를 사용하여 문서를 인쇄합니다. |
| [print(AttributeSet printSettings)](#print-javax.print.attribute.AttributeSet-) | 기본 프린터를 사용하여 문서를 인쇄합니다. |
| [save(OutputStream stream)](#save-java.io.OutputStream-) | OneNote 문서를 스트림에 저장합니다. |
| [save(OutputStream stream, SaveOptions options)](#save-java.io.OutputStream-com.aspose.note.SaveOptions-) | 지정된 저장 옵션을 사용하여 OneNote 문서를 스트림에 저장합니다. |
| [save(OutputStream stream, int format)](#save-java.io.OutputStream-int-) | 지정된 형식으로 OneNote 문서를 스트림에 저장합니다. |
| [save(String fileName)](#save-java.lang.String-) | OneNote 문서를 파일에 저장합니다. |
| [save(String fileName, SaveOptions options)](#save-java.lang.String-com.aspose.note.SaveOptions-) | 지정된 저장 옵션을 사용하여 OneNote 문서를 파일에 저장합니다. |
| [save(String fileName, int format)](#save-java.lang.String-int-) | 지정된 형식으로 OneNote 문서를 파일에 저장합니다. |
| [setAutomaticLayoutChangesDetectionEnabled(boolean value)](#setAutomaticLayoutChangesDetectionEnabled-boolean-) | Aspose.Note가 레이아웃 변경을 자동으로 감지할지 여부를 나타내는 값을 설정합니다. |
| [setColor(Color value)](#setColor-java.awt.Color-) | 색상을 설정합니다. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | 생성 시간을 설정합니다. |
| [setDisplayName(String value)](#setDisplayName-java.lang.String-) | 표시 이름을 설정합니다. |
### Document() {#Document--}
```
public Document()
```


`Document` 클래스의 새 인스턴스를 초기화합니다. 빈 OneNote 문서를 생성합니다.

### Document(String filePath) {#Document-java.lang.String-}
```
public Document(String filePath)
```


`Document` 클래스의 새 인스턴스를 초기화합니다. 파일에서 기존 OneNote 문서를 엽니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| filePath | java.lang.String | 파일 경로. |

### Document(String filePath, LoadOptions loadOptions) {#Document-java.lang.String-com.aspose.note.LoadOptions-}
```
public Document(String filePath, LoadOptions loadOptions)
```


`Document` 클래스의 새 인스턴스를 초기화합니다. 파일에서 기존 OneNote 문서를 엽니다. 암호화 비밀번호와 같은 추가 옵션을 지정할 수 있습니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| filePath | java.lang.String | 파일 경로. |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | 문서를 로드하는 데 사용되는 옵션입니다. null일 수 있습니다. |

### Document(InputStream inStream) {#Document-java.io.InputStream-}
```
public Document(InputStream inStream)
```


`Document` 클래스의 새 인스턴스를 초기화합니다. 스트림에서 기존 OneNote 문서를 엽니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| inStream | java.io.InputStream | 스트림입니다. |

### Document(InputStream inStream, LoadOptions loadOptions) {#Document-java.io.InputStream-com.aspose.note.LoadOptions-}
```
public Document(InputStream inStream, LoadOptions loadOptions)
```


`Document` 클래스의 새 인스턴스를 초기화합니다. 스트림에서 기존 OneNote 문서를 엽니다. 암호화 비밀번호와 같은 추가 옵션을 지정할 수 있습니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| inStream | java.io.InputStream | 스트림입니다. |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | 문서를 로드하는 데 사용되는 옵션입니다. null일 수 있습니다. |

### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


노드의 방문자를 수락합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | `DocumentVisitor`에서 파생된 클래스의 객체. |

### detectLayoutChanges() {#detectLayoutChanges--}
```
public void detectLayoutChanges()
```


이전 `DetectLayoutChanges` 호출 이후 문서 레이아웃에 발생한 모든 변경 사항을 감지합니다. `AutomaticLayoutChangesDetectionEnabled`가 true로 설정된 경우, 문서 내보내기 시작 시 자동으로 사용됩니다.

### getAutomaticLayoutChangesDetectionEnabled() {#getAutomaticLayoutChangesDetectionEnabled--}
```
public boolean getAutomaticLayoutChangesDetectionEnabled()
```


Aspose.Note가 레이아웃 변경을 자동으로 감지할지 여부를 나타내는 값을 가져옵니다. 기본값은 `true`입니다.

**Returns:**
boolean
### getColor() {#getColor--}
```
public Color getColor()
```


색상을 가져옵니다.

**Returns:**
java.awt.Color
### getCreationTime() {#getCreationTime--}
```
public Date getCreationTime()
```


생성 시간을 가져옵니다.

**Returns:**
java.util.Date
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


표시 이름을 가져옵니다.

**Returns:**
java.lang.String
### getFileFormat() {#getFileFormat--}
```
public int getFileFormat()
```


파일 형식을 가져옵니다 (OneNote 2010, OneNote Online).

**Returns:**
int
### getGuid() {#getGuid--}
```
public UUID getGuid()
```


객체의 전역 고유 ID를 가져옵니다.

**Returns:**
java.util.UUID
### getGuidInternal() {#getGuidInternal--}
```
public System.Guid getGuidInternal()
```




**Returns:**
com.aspose.ms.System.Guid
### getPageHistory(Page page) {#getPageHistory-com.aspose.note.Page-}
```
public PageHistory getPageHistory(Page page)
```


`PageHistory`를 가져옵니다. 이 객체는 문서에 표시된 각 페이지에 대한 전체 기록을 포함합니다(가장 오래된 것이 인덱스 0에 있습니다). 현재 페이지 리비전은 `PageHistory.current`로 접근할 수 있으며, 과거 버전 컬렉션과 별도로 포함됩니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | 페이지의 현재 리비전입니다. |

**Returns:**
[PageHistory](../../com.aspose.note/pagehistory) - The `PageHistory`.
### isEncrypted(InputStream stream, Document[] document) {#isEncrypted-java.io.InputStream-com.aspose.note.Document---}
```
public static boolean isEncrypted(InputStream stream, Document[] document)
```


스트림에서 가져온 문서가 암호화되었는지 확인합니다. 확인하려면 문서를 완전히 로드해야 합니다. 따라서 이 메서드는 성능 저하를 초래할 수 있습니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 스트림 | java.io.InputStream | 스트림입니다. |
| document | [Document\[\]](../../com.aspose.note/document) | 로드된 문서입니다. |

**Returns:**
boolean - 문서가 암호화된 경우 true를 반환하고, 그렇지 않으면 false를 반환합니다.
### isEncrypted(InputStream stream, LoadOptions options, Document[] document) {#isEncrypted-java.io.InputStream-com.aspose.note.LoadOptions-com.aspose.note.Document---}
```
public static boolean isEncrypted(InputStream stream, LoadOptions options, Document[] document)
```


스트림에서 가져온 문서가 암호화되었는지 확인합니다. 확인하려면 문서를 완전히 로드해야 합니다. 따라서 이 메서드는 성능 저하를 초래할 수 있습니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 스트림 | java.io.InputStream | 스트림입니다. |
| options | [LoadOptions](../../com.aspose.note/loadoptions) | 로드 옵션입니다. |
| document | [Document\[\]](../../com.aspose.note/document) | 로드된 문서입니다. |

**Returns:**
boolean - 문서가 암호화된 경우 true를 반환하고, 그렇지 않으면 false를 반환합니다.
### isEncrypted(InputStream stream, String password, Document[] document) {#isEncrypted-java.io.InputStream-java.lang.String-com.aspose.note.Document---}
```
public static boolean isEncrypted(InputStream stream, String password, Document[] document)
```


스트림에서 가져온 문서가 암호화되었는지 확인합니다. 확인하려면 문서를 완전히 로드해야 합니다. 따라서 이 메서드는 성능 저하를 초래할 수 있습니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 스트림 | java.io.InputStream | 스트림입니다. |
| password | java.lang.String | 문서를 복호화하기 위한 비밀번호입니다. |
| document | [Document\[\]](../../com.aspose.note/document) | 로드된 문서입니다. |

**Returns:**
boolean - 문서가 암호화된 경우 true를 반환하고, 그렇지 않으면 false를 반환합니다.
### isEncrypted(String filePath, Document[] document) {#isEncrypted-java.lang.String-com.aspose.note.Document---}
```
public static boolean isEncrypted(String filePath, Document[] document)
```


파일에서 가져온 문서가 암호화되었는지 확인합니다. 확인하려면 문서를 완전히 로드해야 합니다. 따라서 이 메서드는 성능 저하를 초래할 수 있습니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| filePath | java.lang.String | 파일 경로. |
| document | [Document\[\]](../../com.aspose.note/document) | 로드된 문서입니다. |

**Returns:**
boolean - 문서가 암호화된 경우 true를 반환하고, 그렇지 않으면 false를 반환합니다.
### isEncrypted(String filePath, LoadOptions options, Document[] document) {#isEncrypted-java.lang.String-com.aspose.note.LoadOptions-com.aspose.note.Document---}
```
public static boolean isEncrypted(String filePath, LoadOptions options, Document[] document)
```


파일에서 가져온 문서가 암호화되었는지 확인합니다. 확인하려면 문서를 완전히 로드해야 합니다. 따라서 이 메서드는 성능 저하를 초래할 수 있습니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| filePath | java.lang.String | 파일 경로. |
| options | [LoadOptions](../../com.aspose.note/loadoptions) | 로드 옵션입니다. |
| document | [Document\[\]](../../com.aspose.note/document) | 로드된 문서입니다. |

**Returns:**
boolean - 문서가 암호화된 경우 true를 반환하고, 그렇지 않으면 false를 반환합니다.
### isEncrypted(String filePath, String password, Document[] document) {#isEncrypted-java.lang.String-java.lang.String-com.aspose.note.Document---}
```
public static boolean isEncrypted(String filePath, String password, Document[] document)
```


파일에서 가져온 문서가 암호화되었는지 확인합니다. 확인하려면 문서를 완전히 로드해야 합니다. 따라서 이 메서드는 성능 저하를 초래할 수 있습니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| filePath | java.lang.String | 파일 경로. |
| password | java.lang.String | 문서를 복호화하기 위한 비밀번호입니다. |
| document | [Document\[\]](../../com.aspose.note/document) | 로드된 문서입니다. |

**Returns:**
boolean - 문서가 암호화된 경우 true를 반환하고, 그렇지 않으면 false를 반환합니다.
### print() {#print--}
```
public void print()
```


기본 프린터를 사용하여 문서를 인쇄합니다.

### print(PrintOptions options) {#print-com.aspose.note.PrintOptions-}
```
public void print(PrintOptions options)
```


기본 프린터를 사용하여 문서를 인쇄합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| options | [PrintOptions](../../com.aspose.note/printoptions) | 문서를 인쇄하는 데 사용되는 옵션입니다. null일 수 있습니다. |

### print(String printerName) {#print-java.lang.String-}
```
public void print(String printerName)
```


기본 프린터를 사용하여 문서를 인쇄합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| printerName | java.lang.String |  |

### print(AttributeSet printSettings) {#print-javax.print.attribute.AttributeSet-}
```
public void print(AttributeSet printSettings)
```


기본 프린터를 사용하여 문서를 인쇄합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| printSettings | javax.print.attribute.AttributeSet |  |

### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public void save(OutputStream stream)
```


OneNote 문서를 스트림에 저장합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 스트림 | java.io.OutputStream | 문서가 저장될 System.iO.stream입니다. |

### save(OutputStream stream, SaveOptions options) {#save-java.io.OutputStream-com.aspose.note.SaveOptions-}
```
public void save(OutputStream stream, SaveOptions options)
```


지정된 저장 옵션을 사용하여 OneNote 문서를 스트림에 저장합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 스트림 | java.io.OutputStream | 문서가 저장될 System.iO.stream입니다. |
| options | [SaveOptions](../../com.aspose.note/saveoptions) | 문서가 스트림에 저장되는 방식을 지정하는 옵션입니다. |

### save(OutputStream stream, int format) {#save-java.io.OutputStream-int-}
```
public void save(OutputStream stream, int format)
```


지정된 형식으로 OneNote 문서를 스트림에 저장합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 스트림 | java.io.OutputStream | 문서가 저장될 System.iO.stream입니다. |
| format | int | 문서를 저장할 형식. |

### save(String fileName) {#save-java.lang.String-}
```
public void save(String fileName)
```


OneNote 문서를 파일에 저장합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 파일이름 | java.lang.String | 파일의 전체 이름입니다. 지정된 전체 이름을 가진 파일이 이미 존재하면 기존 파일이 덮어쓰기됩니다. |

### save(String fileName, SaveOptions options) {#save-java.lang.String-com.aspose.note.SaveOptions-}
```
public void save(String fileName, SaveOptions options)
```


지정된 저장 옵션을 사용하여 OneNote 문서를 파일에 저장합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 파일이름 | java.lang.String | 파일의 전체 이름입니다. 지정된 전체 이름을 가진 파일이 이미 존재하면 기존 파일이 덮어쓰기됩니다. |
| options | [SaveOptions](../../com.aspose.note/saveoptions) | 문서가 파일에 저장되는 옵션을 지정합니다. |

### save(String fileName, int format) {#save-java.lang.String-int-}
```
public void save(String fileName, int format)
```


지정된 형식으로 OneNote 문서를 파일에 저장합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 파일이름 | java.lang.String | 파일의 전체 이름입니다. 지정된 전체 이름을 가진 파일이 이미 존재하면 기존 파일이 덮어쓰기됩니다. |
| format | int | 문서를 저장할 형식. |

### setAutomaticLayoutChangesDetectionEnabled(boolean value) {#setAutomaticLayoutChangesDetectionEnabled-boolean-}
```
public void setAutomaticLayoutChangesDetectionEnabled(boolean value)
```


Aspose.Note가 레이아웃 변경을 자동으로 감지할지 여부를 나타내는 값을 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | boolean | 새 값입니다. null일 수 있습니다. |

### setColor(Color value) {#setColor-java.awt.Color-}
```
public void setColor(Color value)
```


색상을 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.awt.Color | Color의 값입니다. |

### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public void setCreationTime(Date value)
```


생성 시간을 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.util.Date | DateTime의 값입니다. |

### setDisplayName(String value) {#setDisplayName-java.lang.String-}
```
public void setDisplayName(String value)
```


표시 이름을 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String | DateTime의 값입니다. |

