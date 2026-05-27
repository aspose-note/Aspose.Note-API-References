---
title: "类 OneSaveOptions"
second_title: "Aspose.Note for .NET API 参考"
description: "Aspose.Note.Saving.OneSaveOptions 类。允许在将文档保存为 OneNote 格式时指定其他选项"
type: docs
weight: 890
url: /zh/net/aspose.note.saving/onesaveoptions/
---
## OneSaveOptions class

允许在将文档保存为 OneNote 格式时指定其他选项。

```csharp
public sealed class OneSaveOptions : SaveOptions
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [OneSaveOptions](onesaveoptions/)() | 默认构造函数。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [DocumentPassword](../../aspose.note.saving/onesaveoptions/documentpassword/) { get; set; } | 获取或设置用于加密文档内容的密码。 |
| [FontsSubsystem](../../aspose.note.saving/saveoptions/fontssubsystem/) { get; set; } | 获取或设置在保存时使用的字体设置 |
| [PageCount](../../aspose.note.saving/saveoptions/pagecount/) { get; set; } | 获取或设置要保存的页数。默认值为 MaxValue，表示将渲染文档的所有页面。 |
| [PageIndex](../../aspose.note.saving/saveoptions/pageindex/) { get; set; } | 获取或设置要保存的第一页的索引。默认值为 0。 |
| [SaveFormat](../../aspose.note.saving/saveoptions/saveformat/) { get; } | 获取文档保存的格式。 |

## 示例

展示如何使用加密保存文档。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_NoteBook();

Document document = new Document();
document.Save(dataDir + "CreatingPasswordProtectedDoc_out.one", new OneSaveOptions() { DocumentPassword = "pass" });
```

展示如何使用 OneSaveOptions 保存文档。

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingOneSaveOptions_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, new OneSaveOptions());
```

### 另请参阅

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Note.Saving](../../aspose.note.saving/)
* assembly [Aspose.Note](../../)


