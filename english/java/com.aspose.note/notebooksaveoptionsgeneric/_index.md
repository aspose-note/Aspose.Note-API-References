---
title: NotebookSaveOptionsGeneric
second_title: Aspose.Note for Java API Reference
description: An abstract base class which represents notebook saving options for a particular format and provides common saving options for all document child nodes.
type: docs
weight: 62
url: /java/com.aspose.note/notebooksaveoptionsgeneric/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.NotebookSaveOptions](../../com.aspose.note/notebooksaveoptions)
```
public abstract class NotebookSaveOptionsGeneric<TDocumentSaveOptions> extends NotebookSaveOptions
```

An abstract base class which represents notebook saving options for a particular format and provides common saving options for all document child nodes.

 TDocumentSaveOptions : The save options for all notebook's child documents.
## Constructors

| Constructor | Description |
| --- | --- |
| [NotebookSaveOptionsGeneric()](#NotebookSaveOptionsGeneric--) |  |
## Methods

| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDeferredSaving()](#getDeferredSaving--) | Gets or sets a value indicating whether children documents should be saved explicitly. |
| [getDocumentSaveOptions()](#getDocumentSaveOptions--) | Gets or sets the save options for all notebook's child documents. |
| [getDocumentSaveOptionsInternal()](#getDocumentSaveOptionsInternal--) | Gets the save options for all notebook's child documents. |
| [getFlatten()](#getFlatten--) | Gets or sets a value indicating whether the notebook children hierarchy is saved flattened. |
| [getSaveFormat()](#getSaveFormat--) | Gets the format in which the notebook is saved. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setDeferredSaving(boolean value)](#setDeferredSaving-boolean-) | Gets or sets a value indicating whether children documents should be saved explicitly. |
| [setFlatten(boolean value)](#setFlatten-boolean-) | Gets or sets a value indicating whether the notebook children hierarchy is saved flattened. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### NotebookSaveOptionsGeneric() {#NotebookSaveOptionsGeneric--}
```
public NotebookSaveOptionsGeneric()
```


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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDeferredSaving() {#getDeferredSaving--}
```
public boolean getDeferredSaving()
```


Gets or sets a value indicating whether children documents should be saved explicitly.

--------------------

Default value is  false , so child documents will be saved implicitly. Value  true  is indicating that user should save each notebook's child node explicitly. If notebook is saving to stream, the value is always  true  despite was explicitly set by user to  false .

**Returns:**
boolean
### getDocumentSaveOptions() {#getDocumentSaveOptions--}
```
public TDocumentSaveOptions getDocumentSaveOptions()
```


Gets or sets the save options for all notebook's child documents.

**Returns:**
TDocumentSaveOptions
### getDocumentSaveOptionsInternal() {#getDocumentSaveOptionsInternal--}
```
public SaveOptions getDocumentSaveOptionsInternal()
```


Gets the save options for all notebook's child documents.

**Returns:**
[SaveOptions](../../com.aspose.note/saveoptions) - The  SaveOptions .
### getFlatten() {#getFlatten--}
```
public boolean getFlatten()
```


Gets or sets a value indicating whether the notebook children hierarchy is saved flattened.

**Returns:**
boolean
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Gets the format in which the notebook is saved.

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




### setDeferredSaving(boolean value) {#setDeferredSaving-boolean-}
```
public void setDeferredSaving(boolean value)
```


Gets or sets a value indicating whether children documents should be saved explicitly.

--------------------

Default value is  false , so child documents will be saved implicitly. Value  true  is indicating that user should save each notebook's child node explicitly. If notebook is saving to stream, the value is always  true  despite was explicitly set by user to  false .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setFlatten(boolean value) {#setFlatten-boolean-}
```
public void setFlatten(boolean value)
```


Gets or sets a value indicating whether the notebook children hierarchy is saved flattened.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

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

