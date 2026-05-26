---
title: "IFontsSubsystem"
second_title: "Java용 Aspose.Note API 레퍼런스"
description: "문서를 저장할 때 Aspose.Note가 글꼴을 검색하는 방식을 제어하려면 이 인터페이스를 구현하십시오."
type: docs
weight: 12
url: /ko/java/com.aspose.note.fonts/ifontssubsystem/
---
```
public interface IFontsSubsystem
```

문서를 저장할 때 Aspose.Note가 글꼴을 검색하는 방식을 제어하려면 이 인터페이스를 구현하십시오.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getFontFamily(String fontName)](#getFontFamily-java.lang.String-) | 글꼴을 가져옵니다. |
### getFontFamily(String fontName) {#getFontFamily-java.lang.String-}
```
public abstract Font getFontFamily(String fontName)
```


글꼴을 가져옵니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| fontName | java.lang.String | 글꼴 이름입니다. |

**Returns:**
java.awt.Font - Font입니다.
