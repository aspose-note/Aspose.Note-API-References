---
title: Document
second_title: Aspose.Note for Java API Reference
description: Represents an Aspose.Note document.
type: docs
weight: 19
url: /java/com.aspose.note/document/
---

**Inheritance:**
java.lang.Object, [com.aspose.note.Node](../../com.aspose.note/node), [com.aspose.note.CompositeNodeBase](../../com.aspose.note/compositenodebase), com.aspose.note.CompositeNode

**All Implemented Interfaces:**
[com.aspose.note.INotebookChildNode](../../com.aspose.note/inotebookchildnode)
```
public class Document extends CompositeNode<Page> implements INotebookChildNode
```

Represents an Aspose.Note document.
## Constructors

| Constructor | Description |
| --- | --- |
| [Document()](#Document--) | Initializes a new instance of the  Document  class. |
| [Document(String filePath)](#Document-java.lang.String-) | Initializes a new instance of the  Document  class. |
| [Document(String filePath, LoadOptions loadOptions)](#Document-java.lang.String-com.aspose.note.LoadOptions-) | Initializes a new instance of the  Document  class. |
| [Document(InputStream inStream)](#Document-java.io.InputStream-) | Initializes a new instance of the  Document  class. |
| [Document(InputStream inStream, LoadOptions loadOptions)](#Document-java.io.InputStream-com.aspose.note.LoadOptions-) | Initializes a new instance of the  Document  class. |
## Methods

| Method | Description |
| --- | --- |
| [isEncrypted(InputStream stream, LoadOptions options, Document[] document)](#isEncrypted-java.io.InputStream-com.aspose.note.LoadOptions-com.aspose.note.Document---) | Checks whether a document from a stream is encrypted. |
| [isEncrypted(InputStream stream, String password, Document[] document)](#isEncrypted-java.io.InputStream-java.lang.String-com.aspose.note.Document---) | Checks whether a document from a stream is encrypted. |
| [isEncrypted(InputStream stream, Document[] document)](#isEncrypted-java.io.InputStream-com.aspose.note.Document---) | Checks whether a document from a stream is encrypted. |
| [isEncrypted(String filePath, LoadOptions options, Document[] document)](#isEncrypted-java.lang.String-com.aspose.note.LoadOptions-com.aspose.note.Document---) | Checks whether a document from a file is encrypted. |
| [isEncrypted(String filePath, Document[] document)](#isEncrypted-java.lang.String-com.aspose.note.Document---) | Checks whether a document from a file is encrypted. |
| [isEncrypted(String filePath, String password, Document[] document)](#isEncrypted-java.lang.String-java.lang.String-com.aspose.note.Document---) | Checks whether a document from a file is encrypted. |
| [getAutomaticLayoutChangesDetectionEnabled()](#getAutomaticLayoutChangesDetectionEnabled--) | Gets a value indicating whether Aspose.Note performs detection of layout changes automatically. |
| [setAutomaticLayoutChangesDetectionEnabled(boolean value)](#setAutomaticLayoutChangesDetectionEnabled-boolean-) | Sets a value indicating whether Aspose.Note performs detection of layout changes automatically. |
| [getCreationTime()](#getCreationTime--) | Gets the creation time. |
| [setCreationTime(Date value)](#setCreationTime-java.util.Date-) | Sets the creation time. |
| [getColor()](#getColor--) | Gets the color. |
| [setColor(Color value)](#setColor-java.awt.Color-) | Sets the color. |
| [getDisplayName()](#getDisplayName--) | Gets the display name. |
| [setDisplayName(String value)](#setDisplayName-java.lang.String-) | Sets the display name. |
| [getGuid()](#getGuid--) | Gets the object's globally unique id. |
| [getGuidInternal()](#getGuidInternal--) |  |
| [getFileFormat()](#getFileFormat--) | Gets file format (OneNote 2010, OneNote Online). |
| [accept(DocumentVisitor visitor)](#accept-com.aspose.note.DocumentVisitor-) | Accepts the visitor of the node. |
| [getPageHistory(Page page)](#getPageHistory-com.aspose.note.Page-) | Gets the  PageHistory  which contains full history for each page presented in a document (the earliest at index 0). |
| [save(String fileName)](#save-java.lang.String-) | Saves the OneNote document to a file. |
| [save(OutputStream stream)](#save-java.io.OutputStream-) | Saves the OneNote document to a stream. |
| [save(String fileName, int format)](#save-java.lang.String-int-) | Saves the OneNote document to a file in the specified format. |
| [save(OutputStream stream, int format)](#save-java.io.OutputStream-int-) | Saves the OneNote document to a stream in the specified format. |
| [save(String fileName, SaveOptions options)](#save-java.lang.String-com.aspose.note.SaveOptions-) | Saves the OneNote document to a file using the specified save options. |
| [save(OutputStream stream, SaveOptions options)](#save-java.io.OutputStream-com.aspose.note.SaveOptions-) | Saves the OneNote document to a stream using the specified save options. |
| [print()](#print--) | Prints the document using the default printer. |
| [print(String printerName)](#print-java.lang.String-) | Prints the document using the default printer. |
| [print(AttributeSet printSettings)](#print-javax.print.attribute.AttributeSet-) | Prints the document using the default printer. |
| [print(PrintOptions options)](#print-com.aspose.note.PrintOptions-) | Prints the document using the default printer. |
| [detectLayoutChanges()](#detectLayoutChanges--) | Detects all changes made to the document layout since the previous  DetectLayoutChanges  call. |
### Document() {#Document--}
```
public Document()
```


Initializes a new instance of the  Document  class. Creates a blank OneNote document.

### Document(String filePath) {#Document-java.lang.String-}
```
public Document(String filePath)
```


Initializes a new instance of the  Document  class. Opens an existing OneNote document from a file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | The file path. |

### Document(String filePath, LoadOptions loadOptions) {#Document-java.lang.String-com.aspose.note.LoadOptions-}
```
public Document(String filePath, LoadOptions loadOptions)
```


Initializes a new instance of the  Document  class. Opens an existing OneNote document from a file. Allows to specify additional options such as an encryption password.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | The file path. |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | Options used to load a document. Can be null. |

### Document(InputStream inStream) {#Document-java.io.InputStream-}
```
public Document(InputStream inStream)
```


Initializes a new instance of the  Document  class. Opens an existing OneNote document from a stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| inStream | java.io.InputStream | The stream. |

### Document(InputStream inStream, LoadOptions loadOptions) {#Document-java.io.InputStream-com.aspose.note.LoadOptions-}
```
public Document(InputStream inStream, LoadOptions loadOptions)
```


Initializes a new instance of the  Document  class. Opens an existing OneNote document from a stream. Allows to specify additional options such as an encryption password.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| inStream | java.io.InputStream | The stream. |
| loadOptions | [LoadOptions](../../com.aspose.note/loadoptions) | Options used to load a document. Can be null. |

### isEncrypted(InputStream stream, LoadOptions options, Document[] document) {#isEncrypted-java.io.InputStream-com.aspose.note.LoadOptions-com.aspose.note.Document---}
```
public static boolean isEncrypted(InputStream stream, LoadOptions options, Document[] document)
```


Checks whether a document from a stream is encrypted. To check it we need to completely load this document. So this method can lead to performance penalty.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | The stream. |
| options | [LoadOptions](../../com.aspose.note/loadoptions) | The load options. |
| document | [Document\[\]](../../com.aspose.note/document) | The loaded document. |

**Returns:**
boolean - Returns true if the document is encrypted otherwise false.
### isEncrypted(InputStream stream, String password, Document[] document) {#isEncrypted-java.io.InputStream-java.lang.String-com.aspose.note.Document---}
```
public static boolean isEncrypted(InputStream stream, String password, Document[] document)
```


Checks whether a document from a stream is encrypted. To check it we need to completely load this document. So this method can lead to performance penalty.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | The stream. |
| password | java.lang.String | The password to decrypt a document. |
| document | [Document\[\]](../../com.aspose.note/document) | The loaded document. |

**Returns:**
boolean - Returns true if the document is encrypted otherwise false.
### isEncrypted(InputStream stream, Document[] document) {#isEncrypted-java.io.InputStream-com.aspose.note.Document---}
```
public static boolean isEncrypted(InputStream stream, Document[] document)
```


Checks whether a document from a stream is encrypted. To check it we need to completely load this document. So this method can lead to performance penalty.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | The stream. |
| document | [Document\[\]](../../com.aspose.note/document) | The loaded document. |

**Returns:**
boolean - Returns true if the document is encrypted otherwise false.
### isEncrypted(String filePath, LoadOptions options, Document[] document) {#isEncrypted-java.lang.String-com.aspose.note.LoadOptions-com.aspose.note.Document---}
```
public static boolean isEncrypted(String filePath, LoadOptions options, Document[] document)
```


Checks whether a document from a file is encrypted. To check it we need to completely load this document. So this method can lead to performance penalty.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | The file path. |
| options | [LoadOptions](../../com.aspose.note/loadoptions) | The load options. |
| document | [Document\[\]](../../com.aspose.note/document) | The loaded document. |

**Returns:**
boolean - Returns true if the document is encrypted otherwise false.
### isEncrypted(String filePath, Document[] document) {#isEncrypted-java.lang.String-com.aspose.note.Document---}
```
public static boolean isEncrypted(String filePath, Document[] document)
```


Checks whether a document from a file is encrypted. To check it we need to completely load this document. So this method can lead to performance penalty.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | The file path. |
| document | [Document\[\]](../../com.aspose.note/document) | The loaded document. |

**Returns:**
boolean - Returns true if the document is encrypted otherwise false.
### isEncrypted(String filePath, String password, Document[] document) {#isEncrypted-java.lang.String-java.lang.String-com.aspose.note.Document---}
```
public static boolean isEncrypted(String filePath, String password, Document[] document)
```


Checks whether a document from a file is encrypted. To check it we need to completely load this document. So this method can lead to performance penalty.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filePath | java.lang.String | The file path. |
| password | java.lang.String | The password to decrypt a document. |
| document | [Document\[\]](../../com.aspose.note/document) | The loaded document. |

**Returns:**
boolean - Returns true if the document is encrypted otherwise false.
### getAutomaticLayoutChangesDetectionEnabled() {#getAutomaticLayoutChangesDetectionEnabled--}
```
public boolean getAutomaticLayoutChangesDetectionEnabled()
```


Gets a value indicating whether Aspose.Note performs detection of layout changes automatically. Default value is  true .

**Returns:**
boolean
### setAutomaticLayoutChangesDetectionEnabled(boolean value) {#setAutomaticLayoutChangesDetectionEnabled-boolean-}
```
public void setAutomaticLayoutChangesDetectionEnabled(boolean value)
```


Sets a value indicating whether Aspose.Note performs detection of layout changes automatically.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | New value. Can be null. |

### getCreationTime() {#getCreationTime--}
```
public Date getCreationTime()
```


Gets the creation time.

**Returns:**
java.util.Date
### setCreationTime(Date value) {#setCreationTime-java.util.Date-}
```
public void setCreationTime(Date value)
```


Sets the creation time.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | DateTime's value. |

### getColor() {#getColor--}
```
public Color getColor()
```


Gets the color.

**Returns:**
java.awt.Color
### setColor(Color value) {#setColor-java.awt.Color-}
```
public void setColor(Color value)
```


Sets the color.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.awt.Color | Color's value. |

### getDisplayName() {#getDisplayName--}
```
public String getDisplayName()
```


Gets the display name.

**Returns:**
java.lang.String
### setDisplayName(String value) {#setDisplayName-java.lang.String-}
```
public void setDisplayName(String value)
```


Sets the display name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | DateTime's value. |

### getGuid() {#getGuid--}
```
public UUID getGuid()
```


Gets the object's globally unique id.

**Returns:**
java.util.UUID
### getGuidInternal() {#getGuidInternal--}
```
public System.Guid getGuidInternal()
```




**Returns:**
com.aspose.ms.System.Guid
### getFileFormat() {#getFileFormat--}
```
public int getFileFormat()
```


Gets file format (OneNote 2010, OneNote Online).

**Returns:**
int
### accept(DocumentVisitor visitor) {#accept-com.aspose.note.DocumentVisitor-}
```
public void accept(DocumentVisitor visitor)
```


Accepts the visitor of the node.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| visitor | [DocumentVisitor](../../com.aspose.note/documentvisitor) | The object of a class derived from the  DocumentVisitor . |

### getPageHistory(Page page) {#getPageHistory-com.aspose.note.Page-}
```
public PageHistory getPageHistory(Page page)
```


Gets the  PageHistory  which contains full history for each page presented in a document (the earliest at index 0). The current page revision can be accessed as  PageHistory.current  and contained separately from collection of historical versions.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| page | [Page](../../com.aspose.note/page) | The current revision of a page. |

**Returns:**
[PageHistory](../../com.aspose.note/pagehistory) - The  PageHistory .
### save(String fileName) {#save-java.lang.String-}
```
public void save(String fileName)
```


Saves the OneNote document to a file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | The full name for the file. If a file with the specified full name already exists, the existing file is overwritten. |

### save(OutputStream stream) {#save-java.io.OutputStream-}
```
public void save(OutputStream stream)
```


Saves the OneNote document to a stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | The System.iO.stream where the document will be saved. |

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

### save(OutputStream stream, int format) {#save-java.io.OutputStream-int-}
```
public void save(OutputStream stream, int format)
```


Saves the OneNote document to a stream in the specified format.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | The System.iO.stream where the document will be saved. |
| format | int | The format in which to save the document. |

### save(String fileName, SaveOptions options) {#save-java.lang.String-com.aspose.note.SaveOptions-}
```
public void save(String fileName, SaveOptions options)
```


Saves the OneNote document to a file using the specified save options.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | The full name for the file. If a file with the specified full name already exists, the existing file is overwritten. |
| options | [SaveOptions](../../com.aspose.note/saveoptions) | Specifies the options how the document is saved in file. |

### save(OutputStream stream, SaveOptions options) {#save-java.io.OutputStream-com.aspose.note.SaveOptions-}
```
public void save(OutputStream stream, SaveOptions options)
```


Saves the OneNote document to a stream using the specified save options.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | The System.iO.stream where the document will be saved. |
| options | [SaveOptions](../../com.aspose.note/saveoptions) | Specifies the options how the document is saved in stream. |

### print() {#print--}
```
public void print()
```


Prints the document using the default printer.

### print(String printerName) {#print-java.lang.String-}
```
public void print(String printerName)
```


Prints the document using the default printer.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| printerName | java.lang.String |  |

### print(AttributeSet printSettings) {#print-javax.print.attribute.AttributeSet-}
```
public void print(AttributeSet printSettings)
```


Prints the document using the default printer.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| printSettings | javax.print.attribute.AttributeSet |  |

### print(PrintOptions options) {#print-com.aspose.note.PrintOptions-}
```
public void print(PrintOptions options)
```


Prints the document using the default printer.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [PrintOptions](../../com.aspose.note/printoptions) | Options used to print a document. Can be null. |

### detectLayoutChanges() {#detectLayoutChanges--}
```
public void detectLayoutChanges()
```


Detects all changes made to the document layout since the previous  DetectLayoutChanges  call. In case  AutomaticLayoutChangesDetectionEnabled  set to true, used automatically in the beginning of document export.

