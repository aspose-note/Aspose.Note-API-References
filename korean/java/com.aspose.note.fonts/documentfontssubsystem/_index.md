---
title: "DocumentFontsSubsystem"
second_title: "Java용 Aspose.Note API 레퍼런스"
description: "Aspose.Note.Fonts.FontsSubsystem의 간단한 구현."
type: docs
weight: 10
url: /ko/java/com.aspose.note.fonts/documentfontssubsystem/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.fonts.FontsSubsystem](../../com.aspose.note.fonts/fontssubsystem)
```
public class DocumentFontsSubsystem extends FontsSubsystem
```

Aspose.Note.Fonts.FontsSubsystem의 간단한 구현입니다. OS에서 FontFamily 객체를 검색합니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [DocumentFontsSubsystem(InputStream defaultFontStream, Map&lt;String,String&gt; fontsSubstitutions)](#DocumentFontsSubsystem-java.io.InputStream-java.util.Map-java.lang.String-java.lang.String--) | [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) 클래스의 새 인스턴스를 초기화합니다. |
| [DocumentFontsSubsystem(InputStream defaultFontStream)](#DocumentFontsSubsystem-java.io.InputStream-) | [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) 클래스의 새 인스턴스를 초기화합니다. |
| [DocumentFontsSubsystem(String defaultFontFile, Map&lt;String,String&gt; fontsSubstitutions)](#DocumentFontsSubsystem-java.lang.String-java.util.Map-java.lang.String-java.lang.String--) | [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) 클래스의 새 인스턴스를 초기화합니다. |
| [DocumentFontsSubsystem(String defaultFontFile)](#DocumentFontsSubsystem-java.lang.String-) | [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) 클래스의 새 인스턴스를 초기화합니다. |
| [DocumentFontsSubsystem(Map&lt;String,String&gt; fontsSubstitutions)](#DocumentFontsSubsystem-java.util.Map-java.lang.String-java.lang.String--) | [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) 클래스의 새 인스턴스를 초기화합니다. |
| [DocumentFontsSubsystem()](#DocumentFontsSubsystem--) | [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) 클래스의 새 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getDefault()](#getDefault--) | 정적 기본 인스턴스를 가져오거나 설정합니다. |
| [setDefault(DocumentFontsSubsystem value)](#setDefault-com.aspose.note.fonts.DocumentFontsSubsystem-) | 정적 기본 인스턴스를 가져오거나 설정합니다. |
| [usingDefaultFont(String defaultFontName)](#usingDefaultFont-java.lang.String-) | 지정된 기본 글꼴 이름을 사용하여 새 DocumentFontsSubsystem 인스턴스를 생성합니다. |
| [usingDefaultFont(String defaultFontName, Map&lt;String,String&gt; fontsSubstitutions)](#usingDefaultFont-java.lang.String-java.util.Map-java.lang.String-java.lang.String--) | 지정된 기본 글꼴 이름을 사용하여 새 DocumentFontsSubsystem 인스턴스를 생성합니다. |
| [usingDefaultFontFromFile(String filePath)](#usingDefaultFontFromFile-java.lang.String-) | 지정된 기본 글꼴 이름을 사용하여 새 DocumentFontsSubsystem 인스턴스를 생성합니다. |
| [usingDefaultFontFromFile(String filePath, Map&lt;String,String&gt; fontsSubstitutions)](#usingDefaultFontFromFile-java.lang.String-java.util.Map-java.lang.String-java.lang.String--) | 지정된 파일에서 글꼴을 기본값으로 사용하여 새 DocumentFontsSubsystem 인스턴스를 생성합니다. |
| [usingDefaultFontFromStream(InputStream defaultFontStream)](#usingDefaultFontFromStream-java.io.InputStream-) | 지정된 스트림에서 글꼴을 기본값으로 사용하여 새 DocumentFontsSubsystem 인스턴스를 생성합니다. |
| [usingDefaultFontFromStream(InputStream defaultFontStream, Map&lt;String,String&gt; fontsSubstitutions)](#usingDefaultFontFromStream-java.io.InputStream-java.util.Map-java.lang.String-java.lang.String--) | 지정된 스트림에서 글꼴을 기본값으로 사용하여 새 DocumentFontsSubsystem 인스턴스를 생성합니다. |
### DocumentFontsSubsystem(InputStream defaultFontStream, Map&lt;String,String&gt; fontsSubstitutions) {#DocumentFontsSubsystem-java.io.InputStream-java.util.Map-java.lang.String-java.lang.String--}
```
public DocumentFontsSubsystem(InputStream defaultFontStream, Map<String,String> fontsSubstitutions)
```


[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) 클래스의 새 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| defaultFontStream | java.io.InputStream | 기본 Font를 포함하는 스트림입니다. |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | 글꼴 대체입니다. |

### DocumentFontsSubsystem(InputStream defaultFontStream) {#DocumentFontsSubsystem-java.io.InputStream-}
```
public DocumentFontsSubsystem(InputStream defaultFontStream)
```


[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) 클래스의 새 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| defaultFontStream | java.io.InputStream | 기본 Font를 포함하는 스트림입니다. |

### DocumentFontsSubsystem(String defaultFontFile, Map&lt;String,String&gt; fontsSubstitutions) {#DocumentFontsSubsystem-java.lang.String-java.util.Map-java.lang.String-java.lang.String--}
```
public DocumentFontsSubsystem(String defaultFontFile, Map<String,String> fontsSubstitutions)
```


[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) 클래스의 새 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| defaultFontFile | java.lang.String | 기본 Font를 포함하는 파일의 경로입니다. |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | 글꼴 대체입니다. |

### DocumentFontsSubsystem(String defaultFontFile) {#DocumentFontsSubsystem-java.lang.String-}
```
public DocumentFontsSubsystem(String defaultFontFile)
```


[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) 클래스의 새 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| defaultFontFile | java.lang.String | 기본 Font를 포함하는 파일의 경로입니다. |

### DocumentFontsSubsystem(Map&lt;String,String&gt; fontsSubstitutions) {#DocumentFontsSubsystem-java.util.Map-java.lang.String-java.lang.String--}
```
public DocumentFontsSubsystem(Map<String,String> fontsSubstitutions)
```


[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) 클래스의 새 인스턴스를 초기화합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | 글꼴 대체입니다. |

### DocumentFontsSubsystem() {#DocumentFontsSubsystem--}
```
public DocumentFontsSubsystem()
```


[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) 클래스의 새 인스턴스를 초기화합니다.

### getDefault() {#getDefault--}
```
public static DocumentFontsSubsystem getDefault()
```


정적 기본 인스턴스를 가져오거나 설정합니다.

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem)
### setDefault(DocumentFontsSubsystem value) {#setDefault-com.aspose.note.fonts.DocumentFontsSubsystem-}
```
public static void setDefault(DocumentFontsSubsystem value)
```


정적 기본 인스턴스를 가져오거나 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| value | [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) |  |

### usingDefaultFont(String defaultFontName) {#usingDefaultFont-java.lang.String-}
```
public static DocumentFontsSubsystem usingDefaultFont(String defaultFontName)
```


지정된 기본 글꼴 이름을 사용하여 새 DocumentFontsSubsystem 인스턴스를 생성합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| defaultFontName | java.lang.String | 기본 글꼴 이름입니다. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFont(String defaultFontName, Map&lt;String,String&gt; fontsSubstitutions) {#usingDefaultFont-java.lang.String-java.util.Map-java.lang.String-java.lang.String--}
```
public static DocumentFontsSubsystem usingDefaultFont(String defaultFontName, Map<String,String> fontsSubstitutions)
```


지정된 기본 글꼴 이름을 사용하여 새 DocumentFontsSubsystem 인스턴스를 생성합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| defaultFontName | java.lang.String | 기본 글꼴 이름입니다. |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | 글꼴 대체입니다. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFontFromFile(String filePath) {#usingDefaultFontFromFile-java.lang.String-}
```
public static DocumentFontsSubsystem usingDefaultFontFromFile(String filePath)
```


지정된 기본 글꼴 이름을 사용하여 새 DocumentFontsSubsystem 인스턴스를 생성합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| filePath | java.lang.String | 기본 글꼴 이름을 포함하는 파일입니다. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFontFromFile(String filePath, Map&lt;String,String&gt; fontsSubstitutions) {#usingDefaultFontFromFile-java.lang.String-java.util.Map-java.lang.String-java.lang.String--}
```
public static DocumentFontsSubsystem usingDefaultFontFromFile(String filePath, Map<String,String> fontsSubstitutions)
```


지정된 파일에서 글꼴을 기본값으로 사용하여 새 DocumentFontsSubsystem 인스턴스를 생성합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| filePath | java.lang.String | 기본 글꼴 이름을 포함하는 파일입니다. |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | 글꼴 대체입니다. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFontFromStream(InputStream defaultFontStream) {#usingDefaultFontFromStream-java.io.InputStream-}
```
public static DocumentFontsSubsystem usingDefaultFontFromStream(InputStream defaultFontStream)
```


지정된 스트림에서 글꼴을 기본값으로 사용하여 새 DocumentFontsSubsystem 인스턴스를 생성합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| defaultFontStream | java.io.InputStream | 기본 글꼴 이름을 포함하는 스트림입니다. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
### usingDefaultFontFromStream(InputStream defaultFontStream, Map&lt;String,String&gt; fontsSubstitutions) {#usingDefaultFontFromStream-java.io.InputStream-java.util.Map-java.lang.String-java.lang.String--}
```
public static DocumentFontsSubsystem usingDefaultFontFromStream(InputStream defaultFontStream, Map<String,String> fontsSubstitutions)
```


지정된 스트림에서 글꼴을 기본값으로 사용하여 새 DocumentFontsSubsystem 인스턴스를 생성합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| defaultFontStream | java.io.InputStream | 기본 글꼴 이름을 포함하는 스트림입니다. |
| fontsSubstitutions | java.util.Map&lt;java.lang.String,java.lang.String&gt; | 글꼴 대체입니다. |

**Returns:**
[DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem) - [DocumentFontsSubsystem](../../com.aspose.note.fonts/documentfontssubsystem).
