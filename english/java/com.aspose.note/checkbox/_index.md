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
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getChecked()](#getChecked--) | Gets a value indicating whether the CheckBox is in the checked state. |
| [getClass()](#getClass--) |  |
| [getCompletedTime()](#getCompletedTime--) | Gets or sets the completed time. |
| [getCreationTime()](#getCreationTime--) | Gets or sets the creation time. |
| [getIcon()](#getIcon--) | Gets or sets the icon. |
| [getStatus()](#getStatus--) | Gets or sets the status. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCompleted()](#setCompleted--) | Sets the tag to completed state using current time as completed time. |
| [setCompleted(Date completedTime)](#setCompleted-java.util.Date-) | Sets the tag to completed state. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Gets or sets the creation time. |
| [setOpen()](#setOpen--) | Sets the tag to open state. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getChecked() {#getChecked--}
```
public final boolean getChecked()
```


Gets a value indicating whether the CheckBox is in the checked state.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCompletedTime() {#getCompletedTime--}
```
public final Date getCompletedTime()
```


Gets or sets the completed time.

Value: The  Nullable\{DateTime\} .

**Returns:**
java.util.Date
### getCreationTime() {#getCreationTime--}
```
public final Date getCreationTime()
```


Gets or sets the creation time.

Value: The java.util.Date.

**Returns:**
java.util.Date
### getIcon() {#getIcon--}
```
public abstract int getIcon()
```


Gets or sets the icon.

Value: The [TagIcon](../../com.aspose.note.infrastructure/tagicon).

**Returns:**
int
### getStatus() {#getStatus--}
```
public final int getStatus()
```


Gets or sets the status.

Value: The [TagStatus](../../com.aspose.note/tagstatus).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setCompleted() {#setCompleted--}
```
public final void setCompleted()
```


Sets the tag to completed state using current time as completed time.

### setCompleted(Date completedTime) {#setCompleted-java.util.Date-}
```
public final void setCompleted(Date completedTime)
```


Sets the tag to completed state.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| completedTime | java.util.Date | The completed time. |

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

### setOpen() {#setOpen--}
```
public void setOpen()
```


Sets the tag to open state.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final void wait(long arg0)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

