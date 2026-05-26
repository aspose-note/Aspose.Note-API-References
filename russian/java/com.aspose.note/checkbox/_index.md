---
title: "CheckBox"
second_title: "Справочник API Aspose.Note for Java"
description: "Базовый класс для тегов, которые могут переключать своё состояние между завершённым и незавершённым."
type: docs
weight: 13
url: /ru/java/com.aspose.note/checkbox/
---

**Inheritance:**
java.lang.Object, com.aspose.note.TagExtended
```
public abstract class CheckBox extends TagExtended
```

Базовый класс для тегов, которые могут переключать своё состояние между завершённым и незавершённым.
## Методы

| Метод | Описание |
| --- | --- |
| [getChecked()](#getChecked--) | Возвращает значение, указывающее, находится ли CheckBox в отмеченном состоянии. |
| [getCompletedTime()](#getCompletedTime--) | Получает или задает время завершения. |
| [getCreationTime()](#getCreationTime--) | Получает или задает время создания. |
| [getIcon()](#getIcon--) | Получает или задает значок. |
| [getStatus()](#getStatus--) | Получает или задает статус. |
| [setCompleted()](#setCompleted--) | Устанавливает тег в состояние завершено, используя текущее время в качестве времени завершения. |
| [setCompleted(Date completedTime)](#setCompleted-java.util.Date-) | Устанавливает тег в состояние завершено. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Получает или задает время создания. |
| [setOpen()](#setOpen--) | Устанавливает тег в открытое состояние. |
### getChecked() {#getChecked--}
```
public final boolean getChecked()
```


Возвращает значение, указывающее, находится ли CheckBox в отмеченном состоянии.

**Returns:**
boolean
### getCompletedTime() {#getCompletedTime--}
```
public final Date getCompletedTime()
```


Получает или задает время завершения.

Значение: `Nullable\{DateTime\}`.

**Returns:**
java.util.Date
### getCreationTime() {#getCreationTime--}
```
public final Date getCreationTime()
```


Получает или задает время создания.

Значение: java.util.Date.

**Returns:**
java.util.Date
### getIcon() {#getIcon--}
```
public abstract int getIcon()
```


Получает или задает значок.

Значение: [TagIcon](../../com.aspose.note.infrastructure/tagicon).

**Returns:**
int
### getStatus() {#getStatus--}
```
public final int getStatus()
```


Получает или задает статус.

Значение: [TagStatus](../../com.aspose.note/tagstatus).

**Returns:**
int
### setCompleted() {#setCompleted--}
```
public final void setCompleted()
```


Устанавливает тег в состояние завершено, используя текущее время в качестве времени завершения.

### setCompleted(Date completedTime) {#setCompleted-java.util.Date-}
```
public final void setCompleted(Date completedTime)
```


Устанавливает тег в состояние завершено.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| completedTime | java.util.Date | Время завершения. |

### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public final void setCreationTime(Date value)
```


Получает или задает время создания.

Значение: java.util.Date.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | java.util.Date |  |

### setOpen() {#setOpen--}
```
public void setOpen()
```


Устанавливает тег в открытое состояние.

