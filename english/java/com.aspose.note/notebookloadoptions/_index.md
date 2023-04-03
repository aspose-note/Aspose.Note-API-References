---
title: NotebookLoadOptions
second_title: Aspose.Note for Java API Reference
description: Options used to load a notebook.
type: docs
weight: 48
url: /java/com.aspose.note/notebookloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class NotebookLoadOptions
```

Options used to load a notebook.
## Constructors

| Constructor | Description |
| --- | --- |
| [NotebookLoadOptions()](#NotebookLoadOptions--) | Initializes a new instance of the  NotebookLoadOptions  class. |
## Methods

| Method | Description |
| --- | --- |
| [getInstantLoading()](#getInstantLoading--) | Gets or sets a value indicating whether children documents should be loaded while the parent document is loading. |
| [setInstantLoading(boolean value)](#setInstantLoading-boolean-) | Gets or sets a value indicating whether children documents should be loaded while the parent document is loading. |
| [getDeferredLoading()](#getDeferredLoading--) | Gets or sets a value indicating whether children documents should be loaded explicitly later. |
| [setDeferredLoading(boolean value)](#setDeferredLoading-boolean-) | Gets or sets a value indicating whether children documents should be loaded explicitly later. |
### NotebookLoadOptions() {#NotebookLoadOptions--}
```
public NotebookLoadOptions()
```


Initializes a new instance of the  NotebookLoadOptions  class.

### getInstantLoading() {#getInstantLoading--}
```
public boolean getInstantLoading()
```


Gets or sets a value indicating whether children documents should be loaded while the parent document is loading.

--------------------

Default value is  false , so child documents will be loaded "lazily", i.e. their loading should be postponed until a direct access to specific child. Value  true  is indicating that their loading should be done immediately.

**Returns:**
boolean
### setInstantLoading(boolean value) {#setInstantLoading-boolean-}
```
public void setInstantLoading(boolean value)
```


Gets or sets a value indicating whether children documents should be loaded while the parent document is loading.

--------------------

Default value is  false , so child documents will be loaded "lazily", i.e. their loading should be postponed until a direct access to specific child. Value  true  is indicating that their loading should be done immediately.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### getDeferredLoading() {#getDeferredLoading--}
```
public final boolean getDeferredLoading()
```


Gets or sets a value indicating whether children documents should be loaded explicitly later.

--------------------

Default value is  false , so child documents will be loaded implicitly. Value  true  is indicating that user should call  Notebook.loadChildDocument  or for each notebook's child node after notebook itself is loaded. If value is  true ,  NotebookLoadOptions.instantLoading  option will be ignored. If notebook is loading from stream, the value is always  true  despite was explicitly set by user to  false .

**Returns:**
boolean
### setDeferredLoading(boolean value) {#setDeferredLoading-boolean-}
```
public final void setDeferredLoading(boolean value)
```


Gets or sets a value indicating whether children documents should be loaded explicitly later.

--------------------

Default value is  false , so child documents will be loaded implicitly. Value  true  is indicating that user should call  Notebook.loadChildDocument  or for each notebook's child node after notebook itself is loaded. If value is  true ,  NotebookLoadOptions.instantLoading  option will be ignored. If notebook is loading from stream, the value is always  true  despite was explicitly set by user to  false .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

