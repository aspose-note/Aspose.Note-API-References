---
title: Notebook.Save
second_title: Aspose.Note for .NET API Reference
description: Notebook method. Saves the OneNote document to a file
type: docs
weight: 150
url: /net/aspose.note/notebook/save/
---
## Save(string) {#save_3}

Saves the OneNote document to a file.

```csharp
public void Save(string fileName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String | The full name for the file. If a file with the specified full name already exists, the existing file is overwritten. |

### Exceptions

| exception | condition |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | The document structure violates specification. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | Requested save format is not supported. |

### See Also

* class [Notebook](../)
* namespace [Aspose.Note](../../notebook/)
* assembly [Aspose.Note](../../../)

---

## Save(Stream) {#save}

Saves the OneNote document to a stream.

```csharp
public void Save(Stream stream)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | The stream. |

### Exceptions

| exception | condition |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | The document structure violates specification. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | Requested save format is not supported. |

### See Also

* class [Notebook](../)
* namespace [Aspose.Note](../../notebook/)
* assembly [Aspose.Note](../../../)

---

## Save(string, SaveFormat) {#save_4}

Saves the OneNote document to a file in the specified format.

```csharp
public void Save(string fileName, SaveFormat format)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String | The full name for the file. If a file with the specified full name already exists, the existing file is overwritten. |
| format | SaveFormat | The format in which to save the document. |

### Exceptions

| exception | condition |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | The document structure violates specification. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | Requested save format is not supported. |

### See Also

* enum [SaveFormat](../../saveformat/)
* class [Notebook](../)
* namespace [Aspose.Note](../../notebook/)
* assembly [Aspose.Note](../../../)

---

## Save(Stream, SaveFormat) {#save_1}

Saves the OneNote document to a stream in the specified format.

```csharp
public void Save(Stream stream, SaveFormat format)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | The stream. |
| format | SaveFormat | The format in which to save the document. |

### Exceptions

| exception | condition |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | The document structure violates specification. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | Requested save format is not supported. |

### See Also

* enum [SaveFormat](../../saveformat/)
* class [Notebook](../)
* namespace [Aspose.Note](../../notebook/)
* assembly [Aspose.Note](../../../)

---

## Save(string, NotebookSaveOptions) {#save_5}

Saves the OneNote document to a file using the specified save options.

```csharp
public void Save(string fileName, NotebookSaveOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fileName | String | The full name for the file. If a file with the specified full name already exists, the existing file is overwritten. |
| options | NotebookSaveOptions | Specifies the options how the document is saved in file. |

### Exceptions

| exception | condition |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | The document structure violates specification. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | Requested save format is not supported. |

### See Also

* class [NotebookSaveOptions](../../../aspose.note.saving/notebooksaveoptions/)
* class [Notebook](../)
* namespace [Aspose.Note](../../notebook/)
* assembly [Aspose.Note](../../../)

---

## Save(Stream, NotebookSaveOptions) {#save_2}

Saves the OneNote document to a stream using the specified save options.

```csharp
public void Save(Stream stream, NotebookSaveOptions options)
```

| Parameter | Type | Description |
| --- | --- | --- |
| stream | Stream | The stream. |
| options | NotebookSaveOptions | Specifies the options how the document is saved. |

### Exceptions

| exception | condition |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | The document structure violates specification. |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | Requested save format is not supported. |

### See Also

* class [NotebookSaveOptions](../../../aspose.note.saving/notebooksaveoptions/)
* class [Notebook](../)
* namespace [Aspose.Note](../../notebook/)
* assembly [Aspose.Note](../../../)


