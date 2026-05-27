---
title: "Notebook.Save"
second_title: "Aspose.Note for .NET API 参考"
description: "Notebook 方法。将 OneNote 文档保存到文件"
type: docs
weight: 150
url: /zh/net/aspose.note/notebook/save/
---
## Save(string) {#save_3}

将 OneNote 文档保存到文件中。

```csharp
public void Save(string fileName)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fileName | String | 文件的完整名称。如果已存在具有指定完整名称的文件，则会覆盖现有文件。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | 文档结构违反规范。 |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | 不支持请求的保存格式。 |

### 另请参阅

* class [Notebook](../)
* namespace [Aspose.Note](../../notebook/)
* assembly [Aspose.Note](../../../)

---

## Save(Stream) {#save}

将 OneNote 文档保存到流中。

```csharp
public void Save(Stream stream)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | 流 | 流。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | 文档结构违反规范。 |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | 不支持请求的保存格式。 |

### 另请参阅

* class [Notebook](../)
* namespace [Aspose.Note](../../notebook/)
* assembly [Aspose.Note](../../../)

---

## Save(string, SaveFormat) {#save_4}

以指定格式将 OneNote 文档保存到文件中。

```csharp
public void Save(string fileName, SaveFormat format)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fileName | String | 文件的完整名称。如果已存在具有指定完整名称的文件，则会覆盖现有文件。 |
| 格式 | SaveFormat | 用于保存文档的格式。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | 文档结构违反规范。 |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | 不支持请求的保存格式。 |

### 另请参阅

* enum [SaveFormat](../../saveformat/)
* class [Notebook](../)
* namespace [Aspose.Note](../../notebook/)
* assembly [Aspose.Note](../../../)

---

## Save(Stream, SaveFormat) {#save_1}

以指定格式将 OneNote 文档保存到流中。

```csharp
public void Save(Stream stream, SaveFormat format)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | 流 | 流。 |
| 格式 | SaveFormat | 用于保存文档的格式。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | 文档结构违反规范。 |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | 不支持请求的保存格式。 |

### 另请参阅

* enum [SaveFormat](../../saveformat/)
* class [Notebook](../)
* namespace [Aspose.Note](../../notebook/)
* assembly [Aspose.Note](../../../)

---

## Save(string, NotebookSaveOptions) {#save_5}

使用指定的保存选项将 OneNote 文档保存到文件中。

```csharp
public void Save(string fileName, NotebookSaveOptions options)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fileName | String | 文件的完整名称。如果已存在具有指定完整名称的文件，则会覆盖现有文件。 |
| 选项 | NotebookSaveOptions | 指定文档在文件中保存的选项。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | 文档结构违反规范。 |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | 不支持请求的保存格式。 |

### 另请参阅

* class [NotebookSaveOptions](../../../aspose.note.saving/notebooksaveoptions/)
* class [Notebook](../)
* namespace [Aspose.Note](../../notebook/)
* assembly [Aspose.Note](../../../)

---

## Save(Stream, NotebookSaveOptions) {#save_2}

使用指定的保存选项将 OneNote 文档保存到流中。

```csharp
public void Save(Stream stream, NotebookSaveOptions options)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | 流 | 流。 |
| 选项 | NotebookSaveOptions | 指定文档保存的选项。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | 文档结构违反规范。 |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | 不支持请求的保存格式。 |

### 另请参阅

* class [NotebookSaveOptions](../../../aspose.note.saving/notebooksaveoptions/)
* class [Notebook](../)
* namespace [Aspose.Note](../../notebook/)
* assembly [Aspose.Note](../../../)


