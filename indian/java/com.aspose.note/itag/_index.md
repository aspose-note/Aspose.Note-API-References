---
title: "ITag"
second_title: "Aspose.Note for Java API Reference"
description: "The interface for tags of all kinds."
type: docs
weight: 109
url: /hi/java/com.aspose.note/itag/
---
```
public interface ITag
```

The interface for tags of all kinds.
## Methods

| Method | Description |
| --- | --- |
| [getCompletedTime()](#getCompletedTime--) | पूरा होने का समय प्राप्त करता है। |
| [getCreationTime()](#getCreationTime--) | Gets the creation time. |
| [getIcon()](#getIcon--) | आइकन प्राप्त करता है। |
| [getLabel()](#getLabel--) | लेबल टेक्स्ट प्राप्त करता है. |
| [getStatus()](#getStatus--) | स्थिति प्राप्त करता है। |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Sets the creation time. |
### getCompletedTime() {#getCompletedTime--}
```
public abstract Date getCompletedTime()
```


पूरा होने का समय प्राप्त करता है।

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


आइकन प्राप्त करता है।

Value: The [TagIcon](../../com.aspose.note.infrastructure/tagicon).

**Returns:**
int
### getLabel() {#getLabel--}
```
public abstract String getLabel()
```


लेबल टेक्स्ट प्राप्त करता है.

**Returns:**
java.lang.String
### getStatus() {#getStatus--}
```
public abstract int getStatus()
```


स्थिति प्राप्त करता है।

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

