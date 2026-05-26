---
title: "LoadOptions"
second_title: "Java용 Aspose.Note API 레퍼런스"
description: "문서를 로드하는 데 사용되는 옵션입니다."
type: docs
weight: 46
url: /ko/java/com.aspose.note/loadoptions/
---

**Inheritance:**
java.lang.Object
```
public class LoadOptions
```

문서를 로드하는 데 사용되는 옵션입니다.
## 생성자

| 생성자 | 설명 |
| --- | --- |
| [LoadOptions()](#LoadOptions--) | `LoadOptions` 클래스의 새 인스턴스를 초기화합니다. |
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getDocumentPassword()](#getDocumentPassword--) | 암호화된 문서 내용에 대한 비밀번호를 가져오거나 설정합니다. |
| [getLoadHistory()](#getLoadHistory--) | 문서 로더가 기록을 무시해야 하는지를 나타내는 값을 가져오거나 설정합니다. |
| [setDocumentPassword(String value)](#setDocumentPassword-java.lang.String-) | 암호화된 문서 내용에 대한 비밀번호를 가져오거나 설정합니다. |
| [setLoadHistory(boolean value)](#setLoadHistory-boolean-) | 문서 로더가 기록을 무시해야 하는지를 나타내는 값을 가져오거나 설정합니다. |
### LoadOptions() {#LoadOptions--}
```
public LoadOptions()
```


`LoadOptions` 클래스의 새 인스턴스를 초기화합니다.

### getDocumentPassword() {#getDocumentPassword--}
```
public String getDocumentPassword()
```


암호화된 문서 내용에 대한 비밀번호를 가져오거나 설정합니다. 문서가 비밀번호로 보호되지 않은 경우 이 값은 무시됩니다.

**Returns:**
java.lang.String
### getLoadHistory() {#getLoadHistory--}
```
public boolean getLoadHistory()
```


문서 로더가 기록을 무시해야 하는지를 나타내는 값을 가져오거나 설정합니다. 이 옵션을 사용하면 메모리와 CPU 사용량을 줄일 수 있습니다. 기본값은 `true`입니다.

**Returns:**
boolean
### setDocumentPassword(String value) {#setDocumentPassword-java.lang.String-}
```
public void setDocumentPassword(String value)
```


암호화된 문서 내용에 대한 비밀번호를 가져오거나 설정합니다. 문서가 비밀번호로 보호되지 않은 경우 이 값은 무시됩니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.lang.String |  |

### setLoadHistory(boolean value) {#setLoadHistory-boolean-}
```
public void setLoadHistory(boolean value)
```


문서 로더가 기록을 무시해야 하는지를 나타내는 값을 가져오거나 설정합니다. 이 옵션을 사용하면 메모리와 CPU 사용량을 줄일 수 있습니다. 기본값은 `true`입니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | boolean |  |

