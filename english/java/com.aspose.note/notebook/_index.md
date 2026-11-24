---
title: Notebook
second_title: Aspose.Note for Java API Reference
description: Represents an Aspose.Note notebook.
type: docs
weight: 56
url: /java/com.aspose.note/notebook/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
[com.aspose.note.INotebookChildNode](../../com.aspose.note/inotebookchildnode), com.aspose.ms.System.Collections.Generic.IGenericEnumerable
```
public class Notebook implements INotebookChildNode, System.Collections.Generic.IGenericEnumerable<INotebookChildNode>
```

Represents an Aspose.Note notebook.
## Constructors

| Constructor | Description |
| --- | --- |
| [Notebook()](#Notebook--) | Initializes a new instance of the  Notebook  class. |
| [Notebook(String filePath)](#Notebook-java.lang.String-) | Initializes a new instance of the  Notebook  class. |
| [Notebook(String filePath, NotebookLoadOptions loadOptions)](#Notebook-java.lang.String-com.aspose.note.NotebookLoadOptions-) | Initializes a new instance of the  Notebook  class. |
## Methods

| Method | Description |
| --- | --- |
| [<T1>getChildNodes(Class<T1> typeParameterClass)](#-T1-getChildNodes-java.lang.Class-T1--) | Get all child nodes by the node type. |
| [appendChild(INotebookChildNode newChild)](#appendChild-com.aspose.note.INotebookChildNode-) | Adds the node to the end of the list. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Gets or sets the color. |
| [getCount()](#getCount--) | Gets the number of elements contained in the  Notebook . |
| [getDisplayName()](#getDisplayName--) | Gets or sets the display name. |
| [getFileFormat()](#getFileFormat--) | Gets file format (OneNote 2010, OneNote Online). |
| [getGuid()](#getGuid--) | Gets the object's globally unique id. |
| [getGuidInternal()](#getGuidInternal--) |  |
| [get_Item(int index)](#get-Item-int-) | Gets notebook child node by the given index. |
| [hashCode()](#hashCode--) |  |
| [isHistoryEnabled()](#isHistoryEnabled--) | Gets or sets a value indicating whether the history is enabled. |
| [iterator()](#iterator--) | Returns an enumerator that iterates through child nodes of the  Notebook . |
| [loadChildDocument(InputStream stream)](#loadChildDocument-java.io.InputStream-) | Adds a child document node. |
| [loadChildDocument(InputStream stream, LoadOptions loadOptions)](#loadChildDocument-java.io.InputStream-com.aspose.note.LoadOptions-) | Adds a child document node. |
| [loadChildDocument(String filePath)](#loadChildDocument-java.lang.String-) | Adds a child document node. |
| [loadChildDocument(String filePath, LoadOptions loadOptions)](#loadChildDocument-java.lang.String-com.aspose.note.LoadOptions-) | Adds a child document node. |
| [loadChildNotebook(String filePath)](#loadChildNotebook-java.lang.String-) | Adds a child notebook node. |
| [loadChildNotebook(String filePath, NotebookLoadOptions loadOptions)](#loadChildNotebook-java.lang.String-com.aspose.note.NotebookLoadOptions-) | Adds a child notebook node. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeChild(INotebookChildNode oldChild)](#removeChild-com.aspose.note.INotebookChildNode-) | Removes the child node. |
| [save(OutputStream stream)](#save-java.io.OutputStream-) | Saves the OneNote document to a stream. |
| [save(OutputStream stream, NotebookSaveOptions options)](#save-java.io.OutputStream-com.aspose.note.NotebookSaveOptions-) | Saves the OneNote document to a stream using the specified save options. |
| [save(OutputStream stream, int format)](#save-java.io.OutputStream-int-) | Saves the OneNote document to a stream in the specified format. |
| [save(String fileName)](#save-java.lang.String-) | Saves the OneNote document to a file. |
| [save(String fileName, NotebookSaveOptions options)](#save-java.lang.String-com.aspose.note.NotebookSaveOptions-) | Saves the OneNote document to a file using the specified save options. |
| [save(String fileName, int format)](#save-java.lang.String-int-) | Saves the OneNote document to a file in the specified format. |
| [setColor(Color value)](#setColor-java.awt.Color-) | Gets or sets the color. |
| [setDisplayName(String value)](#setDisplayName-java.lang.String-) | Gets or sets the display name. |
| [setHistoryEnabled(boolean value)](#setHistoryEnabled-boolean-) | Gets or sets a value indicating whether the history is enabled. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Notebook() {#Notebook--}
```
public Notebook()
```


Initializes a new instance of the  Notebook  class.

### Notebook(String filePath) {#Notebook-java.lang.String-}
```
public Notebook(String filePath)
```


Initializes a new instance of the  Notebook  class. Opens an existing OneNote notebook from a file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | The file path. |

### Notebook(String filePath, NotebookLoadOptions loadOptions) {#Notebook-java.lang.String-com.aspose.note.NotebookLoadOptions-}
```
public Notebook(String filePath, NotebookLoadOptions loadOptions)
```


Initializes a new instance of the  Notebook  class. Opens an existing OneNote notebook from a file. Allows to specify additional options such as a children loading strategy ("lazy"/instant).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | The file path. |
| loadOptions | [NotebookLoadOptions](../../com.aspose.note/notebookloadoptions) | The load options. |

### <T1>getChildNodes(Class<T1> typeParameterClass) {#-T1-getChildNodes-java.lang.Class-T1--}
```
public List<T1> <T1>getChildNodes(Class<T1> typeParameterClass)
```


Get all child nodes by the node type.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| typeParameterClass | java.lang.Class<T1> |  |

**Returns:**
java.util.List<T1> - A list of child nodes.

 T1 : The type of elements in the returned list.
### appendChild(INotebookChildNode newChild) {#appendChild-com.aspose.note.INotebookChildNode-}
```
public INotebookChildNode appendChild(INotebookChildNode newChild)
```


Adds the node to the end of the list.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| newChild | [INotebookChildNode](../../com.aspose.note/inotebookchildnode) | The node to add. |

**Returns:**
[INotebookChildNode](../../com.aspose.note/inotebookchildnode) - The added node.
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
### getColor() {#getColor--}
```
public Color getColor()
```


Gets or sets the color.

**Returns:**
java.awt.Color
### getCount() {#getCount--}
```
public int getCount()
```


Gets the number of elements contained in the  Notebook .

**Returns:**
int
### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


Gets or sets the display name.

**Returns:**
java.lang.String
### getFileFormat() {#getFileFormat--}
```
public int getFileFormat()
```


Gets file format (OneNote 2010, OneNote Online).

**Returns:**
int
### getGuid() {#getGuid--}
```
public UUID getGuid()
```


Gets the object's globally unique id.

Value: The GUID.

**Returns:**
java.util.UUID
### getGuidInternal() {#getGuidInternal--}
```
public System.Guid getGuidInternal()
```




**Returns:**
com.aspose.ms.System.Guid
### get_Item(int index) {#get-Item-int-}
```
public INotebookChildNode get_Item(int index)
```


Gets notebook child node by the given index.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | Index to child node. |

**Returns:**
[INotebookChildNode](../../com.aspose.note/inotebookchildnode) - The child node on the  index  position.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isHistoryEnabled() {#isHistoryEnabled--}
```
public boolean isHistoryEnabled()
```


Gets or sets a value indicating whether the history is enabled.

**Returns:**
boolean
### iterator() {#iterator--}
```
public System.Collections.Generic.IGenericEnumerator<INotebookChildNode> iterator()
```


Returns an enumerator that iterates through child nodes of the  Notebook .

**Returns:**
com.aspose.ms.System.Collections.Generic.IGenericEnumerator<com.aspose.note.INotebookChildNode> - A  IEnumerator .
### loadChildDocument(InputStream stream) {#loadChildDocument-java.io.InputStream-}
```
public void loadChildDocument(InputStream stream)
```


Adds a child document node. Opens an existing OneNote document from a stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | The stream. |

### loadChildDocument(InputStream stream, LoadOptions loadOptions) {#loadChildDocument-java.io.InputStream-com.aspose.note.LoadOptions-}
```
public void loadChildDocument(InputStream stream, LoadOptions loadOptions)
```


Adds a child document node. Opens an existing OneNote document from a stream. Allows to specify additional load options.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | The stream. |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | The load options. |

### loadChildDocument(String filePath) {#loadChildDocument-java.lang.String-}
```
public void loadChildDocument(String filePath)
```


Adds a child document node. Opens an existing OneNote document from a file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | The file path. |

### loadChildDocument(String filePath, LoadOptions loadOptions) {#loadChildDocument-java.lang.String-com.aspose.note.LoadOptions-}
```
public void loadChildDocument(String filePath, LoadOptions loadOptions)
```


Adds a child document node. Opens an existing OneNote document from a file. Allows to specify additional load options.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | The file path. |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | The load options. |

### loadChildNotebook(String filePath) {#loadChildNotebook-java.lang.String-}
```
public void loadChildNotebook(String filePath)
```


Adds a child notebook node. Opens an existing OneNote notebook from a file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | The file path. |

### loadChildNotebook(String filePath, NotebookLoadOptions loadOptions) {#loadChildNotebook-java.lang.String-com.aspose.note.NotebookLoadOptions-}
```
public void loadChildNotebook(String filePath, NotebookLoadOptions loadOptions)
```


Adds a child notebook node. Opens an existing OneNote notebook from a file. Allows to specify additional load options.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | The file path. |
| loadOptions | [NotebookLoadOptions](../../com.aspose.note/notebookloadoptions) | The load options. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### removeChild(INotebookChildNode oldChild) {#removeChild-com.aspose.note.INotebookChildNode-}
```
public INotebookChildNode removeChild(INotebookChildNode oldChild)
```


Removes the child node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| oldChild | [INotebookChildNode](../../com.aspose.note/inotebookchildnode) | The node to remove. |

**Returns:**
[INotebookChildNode](../../com.aspose.note/inotebookchildnode) - The removed node.
### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public void save(OutputStream stream)
```


Saves the OneNote document to a stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | The stream. |

### save(OutputStream stream, NotebookSaveOptions options) {#save-java.io.OutputStream-com.aspose.note.NotebookSaveOptions-}
```
public void save(OutputStream stream, NotebookSaveOptions options)
```


Saves the OneNote document to a stream using the specified save options.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | The stream. |
| options | [NotebookSaveOptions](../../com.aspose.note/notebooksaveoptions) | Specifies the options how the document is saved. |

### save(OutputStream stream, int format) {#save-java.io.OutputStream-int-}
```
public void save(OutputStream stream, int format)
```


Saves the OneNote document to a stream in the specified format.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | The stream. |
| format | int | The format in which to save the document. |

### save(String fileName) {#save-java.lang.String-}
```
public void save(String fileName)
```


Saves the OneNote document to a file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | The full name for the file. If a file with the specified full name already exists, the existing file is overwritten. |

### save(String fileName, NotebookSaveOptions options) {#save-java.lang.String-com.aspose.note.NotebookSaveOptions-}
```
public void save(String fileName, NotebookSaveOptions options)
```


Saves the OneNote document to a file using the specified save options.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | The full name for the file. If a file with the specified full name already exists, the existing file is overwritten. |
| options | [NotebookSaveOptions](../../com.aspose.note/notebooksaveoptions) | Specifies the options how the document is saved in file. |

### save(String fileName, int format) {#save-java.lang.String-int-}
```
public void save(String fileName, int format)
```


Saves the OneNote document to a file in the specified format.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | The full name for the file. If a file with the specified full name already exists, the existing file is overwritten. |
| format | int | The format in which to save the document. |

### setColor(Color value) {#setColor-java.awt.Color-}
```
public void setColor(Color value)
```


Gets or sets the color.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.awt.Color |  |

### setDisplayName(String value) {#setDisplayName-java.lang.String-}
```
public void setDisplayName(String value)
```


Gets or sets the display name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setHistoryEnabled(boolean value) {#setHistoryEnabled-boolean-}
```
public void setHistoryEnabled(boolean value)
```


Gets or sets a value indicating whether the history is enabled.

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

