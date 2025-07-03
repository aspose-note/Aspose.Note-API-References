---
title: LoadOptions
second_title: Aspose.Note for Java API Reference
description: Options used to load a document.
type: docs
weight: 46
url: /java/com.aspose.note/loadoptions/
---

**Inheritance:**
java.lang.Object
```
public class LoadOptions
```

Options used to load a document.
## Constructors

| Constructor | Description |
| --- | --- |
| [LoadOptions()](#LoadOptions--) | Initializes a new instance of the `LoadOptions` class. |
## Methods

| Method | Description |
| --- | --- |
| [getDocumentPassword()](#getDocumentPassword--) | Gets or sets a password for the encrypted document content. |
| [getLoadHistory()](#getLoadHistory--) | Gets or sets a value indicating whether a document loader should ignore the history. |
| [setDocumentPassword(String value)](#setDocumentPassword-java.lang.String-) | Gets or sets a password for the encrypted document content. |
| [setLoadHistory(boolean value)](#setLoadHistory-boolean-) | Gets or sets a value indicating whether a document loader should ignore the history. |
### LoadOptions() {#LoadOptions--}
```
public LoadOptions()
```


Initializes a new instance of the `LoadOptions` class.

### getDocumentPassword() {#getDocumentPassword--}
```
public String getDocumentPassword()
```


Gets or sets a password for the encrypted document content. Value is ignored in case the document is not password protected.

**Returns:**
java.lang.String
### getLoadHistory() {#getLoadHistory--}
```
public boolean getLoadHistory()
```


Gets or sets a value indicating whether a document loader should ignore the history. Use this option to decrease memory and CPU usage. Default value is `true`.

**Returns:**
boolean
### setDocumentPassword(String value) {#setDocumentPassword-java.lang.String-}
```
public void setDocumentPassword(String value)
```


Gets or sets a password for the encrypted document content. Value is ignored in case the document is not password protected.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setLoadHistory(boolean value) {#setLoadHistory-boolean-}
```
public void setLoadHistory(boolean value)
```


Gets or sets a value indicating whether a document loader should ignore the history. Use this option to decrease memory and CPU usage. Default value is `true`.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

