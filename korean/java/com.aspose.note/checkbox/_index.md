---
title: "CheckBox"
second_title: "Java용 Aspose.Note API 레퍼런스"
description: "완료와 미완료 상태를 전환할 수 있는 태그의 기본 클래스입니다."
type: docs
weight: 13
url: /ko/java/com.aspose.note/checkbox/
---

**Inheritance:**
java.lang.Object, com.aspose.note.TagExtended
```
public abstract class CheckBox extends TagExtended
```

완료와 미완료 상태를 전환할 수 있는 태그의 기본 클래스입니다.
## 메서드

| 메서드 | 설명 |
| --- | --- |
| [getChecked()](#getChecked--) | CheckBox가 선택된 상태인지 여부를 나타내는 값을 가져옵니다. |
| [getCompletedTime()](#getCompletedTime--) | 완료 시간을 가져오거나 설정합니다. |
| [getCreationTime()](#getCreationTime--) | 생성 시간을 가져오거나 설정합니다. |
| [getIcon()](#getIcon--) | 아이콘을 가져오거나 설정합니다. |
| [getStatus()](#getStatus--) | 상태를 가져오거나 설정합니다. |
| [setCompleted()](#setCompleted--) | 현재 시간을 완료 시간으로 사용하여 태그를 완료 상태로 설정합니다. |
| [setCompleted(Date completedTime)](#setCompleted-java.util.Date-) | 태그를 완료 상태로 설정합니다. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | 생성 시간을 가져오거나 설정합니다. |
| [setOpen()](#setOpen--) | 태그를 열림 상태로 설정합니다. |
### getChecked() {#getChecked--}
```
public final boolean getChecked()
```


CheckBox가 선택된 상태인지 여부를 나타내는 값을 가져옵니다.

**Returns:**
boolean
### getCompletedTime() {#getCompletedTime--}
```
public final Date getCompletedTime()
```


완료 시간을 가져오거나 설정합니다.

값: `Nullable{DateTime}`.

**Returns:**
java.util.Date
### getCreationTime() {#getCreationTime--}
```
public final Date getCreationTime()
```


생성 시간을 가져오거나 설정합니다.

값: java.util.Date입니다.

**Returns:**
java.util.Date
### getIcon() {#getIcon--}
```
public abstract int getIcon()
```


아이콘을 가져오거나 설정합니다.

값: [TagIcon](../../com.aspose.note.infrastructure/tagicon)입니다.

**Returns:**
int
### getStatus() {#getStatus--}
```
public final int getStatus()
```


상태를 가져오거나 설정합니다.

값: [TagStatus](../../com.aspose.note/tagstatus)입니다.

**Returns:**
int
### setCompleted() {#setCompleted--}
```
public final void setCompleted()
```


현재 시간을 완료 시간으로 사용하여 태그를 완료 상태로 설정합니다.

### setCompleted(Date completedTime) {#setCompleted-java.util.Date-}
```
public final void setCompleted(Date completedTime)
```


태그를 완료 상태로 설정합니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| completedTime | java.util.Date | 완료 시간입니다. |

### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public final void setCreationTime(Date value)
```


생성 시간을 가져오거나 설정합니다.

값: java.util.Date입니다.

**Parameters:**
| 매개변수 | 유형 | 설명 |
| --- | --- | --- |
| 값 | java.util.Date |  |

### setOpen() {#setOpen--}
```
public void setOpen()
```


태그를 열림 상태로 설정합니다.

