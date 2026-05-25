---
title: "CheckBox"
second_title: "Aspose.Note for Java API Reference"
description: "The base class for tags that can toggle their state between complete and incomplete."
type: docs
weight: 13
url: /hi/java/com.aspose.note/checkbox/
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
| [getChecked()](#getChecked--) | CheckBox की जांच स्थिति में है या नहीं, यह दर्शाने वाला मान प्राप्त करता है। |
| [getCompletedTime()](#getCompletedTime--) | पूरा किया गया समय प्राप्त करता है या सेट करता है। |
| [getCreationTime()](#getCreationTime--) | निर्माण समय प्राप्त करता है या सेट करता है। |
| [getIcon()](#getIcon--) | आइकन प्राप्त करता है या सेट करता है. |
| [getStatus()](#getStatus--) | स्थिति प्राप्त करता है या सेट करता है. |
| [setCompleted()](#setCompleted--) | वर्तमान समय को पूर्ण समय के रूप में उपयोग करके टैग को पूर्ण स्थिति में सेट करता है। |
| [setCompleted(Date completedTime)](#setCompleted-java.util.Date-) | टैग को पूर्ण स्थिति में सेट करता है। |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | निर्माण समय प्राप्त करता है या सेट करता है। |
| [setOpen()](#setOpen--) | Sets the tag to open state. |
### getChecked() {#getChecked--}
```
public final boolean getChecked()
```


CheckBox की जांच स्थिति में है या नहीं, यह दर्शाने वाला मान प्राप्त करता है।

**Returns:**
boolean
### getCompletedTime() {#getCompletedTime--}
```
public final Date getCompletedTime()
```


पूरा किया गया समय प्राप्त करता है या सेट करता है।

Value: The `Nullable\{DateTime\}`.

**Returns:**
java.util.Date
### getCreationTime() {#getCreationTime--}
```
public final Date getCreationTime()
```


निर्माण समय प्राप्त करता है या सेट करता है।

Value: The java.util.Date.

**Returns:**
java.util.Date
### getIcon() {#getIcon--}
```
public abstract int getIcon()
```


आइकन प्राप्त करता है या सेट करता है.

Value: The [TagIcon](../../com.aspose.note.infrastructure/tagicon).

**Returns:**
int
### getStatus() {#getStatus--}
```
public final int getStatus()
```


स्थिति प्राप्त करता है या सेट करता है.

Value: The [TagStatus](../../com.aspose.note/tagstatus).

**Returns:**
int
### setCompleted() {#setCompleted--}
```
public final void setCompleted()
```


वर्तमान समय को पूर्ण समय के रूप में उपयोग करके टैग को पूर्ण स्थिति में सेट करता है।

### setCompleted(Date completedTime) {#setCompleted-java.util.Date-}
```
public final void setCompleted(Date completedTime)
```


टैग को पूर्ण स्थिति में सेट करता है।

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| completedTime | java.util.Date | पूरा किया गया समय। |

### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public final void setCreationTime(Date value)
```


निर्माण समय प्राप्त करता है या सेट करता है।

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

