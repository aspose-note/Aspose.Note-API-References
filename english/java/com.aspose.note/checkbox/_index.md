---
title: CheckBox
second_title: Aspose.Note for Java API Reference
description: The base class for tags that can toggle their state between complete and incomplete.
type: docs
weight: 13
url: /java/com.aspose.note/checkbox/
---

**Inheritance:**
java.lang.Object, com.aspose.note.TagExtended
```
public abstract class CheckBox extends TagExtended
```

The base class for tags that can toggle their state between complete and incomplete.
## Methods

| Method | Description |
| --- | --- |
| [getCreationTime()](#getCreationTime--) | Gets or sets the creation time. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Gets or sets the creation time. |
| [getCompletedTime()](#getCompletedTime--) | Gets or sets the completed time. |
| [getStatus()](#getStatus--) | Gets or sets the status. |
| [getIcon()](#getIcon--) | Gets or sets the icon. |
| [getChecked()](#getChecked--) | Gets a value indicating whether the CheckBox is in the checked state. |
| [setCompleted(Date completedTime)](#setCompleted-java.util.Date-) | Sets the tag to completed state. |
| [setCompleted()](#setCompleted--) | Sets the tag to completed state using current time as completed time. |
| [setOpen()](#setOpen--) | Sets the tag to open state. |
### getCreationTime() {#getCreationTime--}
```
public final Date getCreationTime()
```


Gets or sets the creation time.

Value: The java.util.Date.

**Returns:**
java.util.Date
### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public final void setCreationTime(Date value)
```


Gets or sets the creation time.

Value: The java.util.Date.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date |  |

### getCompletedTime() {#getCompletedTime--}
```
public final Date getCompletedTime()
```


Gets or sets the completed time.

Value: The  Nullable\{DateTime\} .

**Returns:**
java.util.Date
### getStatus() {#getStatus--}
```
public final int getStatus()
```


Gets or sets the status.

Value: The [TagStatus](../../com.aspose.note/tagstatus).

**Returns:**
int
### getIcon() {#getIcon--}
```
public abstract int getIcon()
```


Gets or sets the icon.

Value: The [TagIcon](../../com.aspose.note.infrastructure/tagicon).

**Returns:**
int
### getChecked() {#getChecked--}
```
public final boolean getChecked()
```


Gets a value indicating whether the CheckBox is in the checked state.

**Returns:**
boolean
### setCompleted(Date completedTime) {#setCompleted-java.util.Date-}
```
public final void setCompleted(Date completedTime)
```


Sets the tag to completed state.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| completedTime | java.util.Date | The completed time. |

### setCompleted() {#setCompleted--}
```
public final void setCompleted()
```


Sets the tag to completed state using current time as completed time.

### setOpen() {#setOpen--}
```
public void setOpen()
```


Sets the tag to open state.

