---
title: "ITag"
second_title: "Java용 Aspose.Note API 레퍼런스"
description: "모든 종류의 태그에 대한 인터페이스입니다."
type: docs
weight: 109
url: /ko/java/com.aspose.note/itag/
---
```
public interface ITag
```

모든 종류의 태그에 대한 인터페이스입니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getCompletedTime()](#getCompletedTime--) | 완료 시간을 가져옵니다. |
| [getCreationTime()](#getCreationTime--) | 생성 시간을 가져옵니다. |
| [getIcon()](#getIcon--) | 아이콘을 가져옵니다. |
| [getLabel()](#getLabel--) | 레이블 텍스트를 가져옵니다. |
| [getStatus()](#getStatus--) | 상태를 가져옵니다. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | 생성 시간을 설정합니다. |
### getCompletedTime() {#getCompletedTime--}
```
public abstract Date getCompletedTime()
```


완료 시간을 가져옵니다.

값: `Nullable{DateTime}`.

**Returns:**
java.util.Date
### getCreationTime() {#getCreationTime--}
```
public abstract Date getCreationTime()
```


생성 시간을 가져옵니다.

값: java.util.Date입니다.

**Returns:**
java.util.Date
### getIcon() {#getIcon--}
```
public abstract int getIcon()
```


아이콘을 가져옵니다.

값: [TagIcon](../../com.aspose.note.infrastructure/tagicon)입니다.

**Returns:**
int
### getLabel() {#getLabel--}
```
public abstract String getLabel()
```


레이블 텍스트를 가져옵니다.

**Returns:**
java.lang.String
### getStatus() {#getStatus--}
```
public abstract int getStatus()
```


상태를 가져옵니다.

값: [TagStatus](../../com.aspose.note/tagstatus)입니다.

**Returns:**
int
### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public abstract void setCreationTime(Date value)
```


생성 시간을 설정합니다.

값: java.util.Date입니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.util.Date |  |

