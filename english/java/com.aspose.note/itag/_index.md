---
title: ITag
second_title: Aspose.Note for Java API Reference
description: The interface for tags of all kinds.
type: docs
weight: 109
url: /java/com.aspose.note/itag/
---
```
public interface ITag
```

The interface for tags of all kinds.
## Methods

| Method | Description |
| --- | --- |
| [getCompletedTime()](#getCompletedTime--) | Gets the completed time. |
| [getCreationTime()](#getCreationTime--) | Gets the creation time. |
| [getIcon()](#getIcon--) | Gets the icon. |
| [getLabel()](#getLabel--) | Gets the label text. |
| [getStatus()](#getStatus--) | Gets the status. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Sets the creation time. |
### getCompletedTime() {#getCompletedTime--}
```
public abstract Date getCompletedTime()
```


Gets the completed time.

Value: The `Nullable\{DateTime\}`.

**Returns:**
java.util.Date
### getCreationTime() {#getCreationTime--}
```
public abstract Date getCreationTime()
```


Gets the creation time.

Value: The java.util.Date.

**Returns:**
java.util.Date
### getIcon() {#getIcon--}
```
public abstract int getIcon()
```


Gets the icon.

Value: The [TagIcon](../../com.aspose.note.infrastructure/tagicon).

**Returns:**
int
### getLabel() {#getLabel--}
```
public abstract String getLabel()
```


Gets the label text.

**Returns:**
java.lang.String
### getStatus() {#getStatus--}
```
public abstract int getStatus()
```


Gets the status.

Value: The [TagStatus](../../com.aspose.note/tagstatus).

**Returns:**
int
### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public abstract void setCreationTime(Date value)
```


Sets the creation time.

Value: The java.util.Date.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date |  |

