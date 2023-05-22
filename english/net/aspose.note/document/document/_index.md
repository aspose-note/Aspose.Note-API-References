---
title: Document.Document
second_title: Aspose.Note for .NET API Reference
description: Document constructor. Initializes a new instance of the Document class. Creates a blank OneNote document
type: docs
weight: 10
url: /net/aspose.note/document/document/
---
## Document() {#constructor}

Initializes a new instance of the [`Document`](../) class. Creates a blank OneNote document.

```csharp
public Document()
```

### See Also

* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)

---

## Document(string) {#constructor_3}

Initializes a new instance of the [`Document`](../) class. Opens an existing OneNote document from a file.

```csharp
public Document(string filePath)
```

| Parameter | Type | Description |
| --- | --- | --- |
| filePath | String | The file path. |

### Exceptions

| exception | condition |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception/) | The document format is not recognized or not supported. |
| [FileCorruptedException](../../filecorruptedexception/) | The document appears to be corrupted and cannot be loaded. |
| [IncorrectPasswordException](../../incorrectpasswordexception/) | The document is encrypted and requires a password to open, but you supplied an incorrect password. |
| InvalidOperationException | There is a problem with the document and it should be reported to Aspose.Note developers. |
| IOException | There is an input/output exception. |

### See Also

* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)

---

## Document(string, LoadOptions) {#constructor_4}

Initializes a new instance of the [`Document`](../) class. Opens an existing OneNote document from a file. Allows to specify additional options such as an encryption password.

```csharp
public Document(string filePath, LoadOptions loadOptions)
```

| Parameter | Type | Description |
| --- | --- | --- |
| filePath | String | The file path. |
| loadOptions | LoadOptions | Options used to load a document. Can be null. |

### Exceptions

| exception | condition |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception/) | The document format is not recognized or not supported. |
| [FileCorruptedException](../../filecorruptedexception/) | The document appears to be corrupted and cannot be loaded. |
| [IncorrectPasswordException](../../incorrectpasswordexception/) | The document is encrypted and requires a password to open, but you supplied an incorrect password. |
| InvalidOperationException | There is a problem with the document and it should be reported to Aspose.Note developers. |
| IOException | There is an input/output exception. |

### See Also

* class [LoadOptions](../../loadoptions/)
* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)

---

## Document(Stream) {#constructor_1}

Initializes a new instance of the [`Document`](../) class. Opens an existing OneNote document from a stream.

```csharp
public Document(Stream inStream)
```

| Parameter | Type | Description |
| --- | --- | --- |
| inStream | Stream | The stream. |

### Exceptions

| exception | condition |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception/) | The document format is not recognized or not supported. |
| [FileCorruptedException](../../filecorruptedexception/) | The document appears to be corrupted and cannot be loaded. |
| [IncorrectPasswordException](../../incorrectpasswordexception/) | The document is encrypted and requires a password to open, but you supplied an incorrect password. |
| InvalidOperationException | There is a problem with the document and it should be reported to Aspose.Note developers. |
| IOException | There is an input/output exception. |
| ArgumentException | The stream does not support reading, is null, or is already closed. |

### See Also

* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)

---

## Document(Stream, LoadOptions) {#constructor_2}

Initializes a new instance of the [`Document`](../) class. Opens an existing OneNote document from a stream. Allows to specify additional options such as an encryption password.

```csharp
public Document(Stream inStream, LoadOptions loadOptions)
```

| Parameter | Type | Description |
| --- | --- | --- |
| inStream | Stream | The stream. |
| loadOptions | LoadOptions | Options used to load a document. Can be null. |

### Exceptions

| exception | condition |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception/) | The document format is not recognized or not supported. |
| [FileCorruptedException](../../filecorruptedexception/) | The document appears to be corrupted and cannot be loaded. |
| [IncorrectPasswordException](../../incorrectpasswordexception/) | The document is encrypted and requires a password to open, but you supplied an incorrect password. |
| InvalidOperationException | There is a problem with the document and it should be reported to Aspose.Note developers. |
| IOException | There is an input/output exception. |
| ArgumentException | The stream does not support reading, is null, or is already closed. |

### See Also

* class [LoadOptions](../../loadoptions/)
* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)


