---
title: "FontsSubsystem"
second_title: "Java용 Aspose.Note API 레퍼런스"
description: "com.aspose.note.IFontsSubsystem 인터페이스를 구현하는 기본 클래스."
type: docs
weight: 11
url: /ko/java/com.aspose.note.fonts/fontssubsystem/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.note.fonts.IFontsSubsystem](../../com.aspose.note.fonts/ifontssubsystem)
```
public abstract class FontsSubsystem implements IFontsSubsystem
```

com.aspose.note.IFontsSubsystem 인터페이스를 구현하는 기본 클래스입니다. 기본 글꼴 및 글꼴 대체 기능을 제공합니다. 파생 클래스에서 com.aspose.note.FontsSubsystem.fetchFontFamily 보호된 멤버 함수를 재정의하여 Font 객체를 검색하는 로직을 구현합니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [addFont(InputStream stream)](#addFont-java.io.InputStream-) | 글꼴을 추가합니다. |
| [addFont(String file)](#addFont-java.lang.String-) | 글꼴을 추가합니다. |
| [addFontSubstitution(String substituted, String substitution)](#addFontSubstitution-java.lang.String-java.lang.String-) | 글꼴 대체를 추가합니다. |
| [getDefaultFont()](#getDefaultFont--) | 기본 글꼴을 가져옵니다. |
| [getFontFamily(String fontName)](#getFontFamily-java.lang.String-) | 글꼴을 가져옵니다. |
| [loadFontsFromFolder(String folder)](#loadFontsFromFolder-java.lang.String-) | 지정된 폴더에서 모든 TrueType 글꼴을 내부 컬렉션으로 로드합니다. |
### addFont(InputStream stream) {#addFont-java.io.InputStream-}
```
public final void addFont(InputStream stream)
```


글꼴을 추가합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 스트림 | java.io.InputStream | 글꼴을 포함하는 스트림입니다. |

### addFont(String file) {#addFont-java.lang.String-}
```
public final void addFont(String file)
```


글꼴을 추가합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 파일 | java.lang.String | 글꼴을 포함하는 파일의 경로입니다. |

### addFontSubstitution(String substituted, String substitution) {#addFontSubstitution-java.lang.String-java.lang.String-}
```
public final void addFontSubstitution(String substituted, String substitution)
```


글꼴 대체를 추가합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 대체된 | java.lang.String | 대체된 글꼴 이름입니다. |
| 대체 | java.lang.String | 대체 글꼴 이름입니다. |

### getDefaultFont() {#getDefaultFont--}
```
public Font getDefaultFont()
```


기본 글꼴을 가져옵니다.

**Returns:**
java.awt.Font
### getFontFamily(String fontName) {#getFontFamily-java.lang.String-}
```
public Font getFontFamily(String fontName)
```


글꼴을 가져옵니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| fontName | java.lang.String | 글꼴 이름입니다. |

**Returns:**
java.awt.Font - Font입니다.
### loadFontsFromFolder(String folder) {#loadFontsFromFolder-java.lang.String-}
```
public final void loadFontsFromFolder(String folder)
```


지정된 폴더에서 모든 TrueType 글꼴을 내부 컬렉션으로 로드합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 폴더 | java.lang.String | 글꼴을 포함하는 폴더입니다. |

