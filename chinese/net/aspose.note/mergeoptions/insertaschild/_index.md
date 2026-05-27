---
title: "MergeOptions.InsertAsChild"
second_title: "Aspose.Note for .NET API 参考"
description: "MergeOptions 属性。获取或设置一个值，指示插入的页面是否应作为前一页面的子项添加"
type: docs
weight: 30
url: /zh/net/aspose.note/mergeoptions/insertaschild/
---
## MergeOptions.InsertAsChild property

获取或设置一个值，指示插入的页面是否应作为前一页面的子页面添加。

```csharp
public bool InsertAsChild { get; set; }
```

## 示例

展示如何从一组 PDF 文档导入所有页面，同时将每个 PDF 文档的页面插入为顶层 OneNote 页面下的子页面。

```csharp
string dataDir = RunExamples.GetDataDir_Import();

var d = new Document();

foreach (var file in new[] { "sampleText.pdf", "sampleImage.pdf", "sampleTable.pdf" })
{
    d.AppendChildLast(new Page()).Title = new Title() { TitleText = new RichText() { ParagraphStyle = ParagraphStyle.Default }.Append(file) };
    d.Import(Path.Combine(dataDir, file), new PdfImportOptions(), new MergeOptions() { InsertAt = int.MaxValue, InsertAsChild = true });
}

d.Save(Path.Combine(dataDir, "sample_StructuredMerge.one"));
```

### 另请参阅

* class [MergeOptions](../)
* namespace [Aspose.Note](../../mergeoptions/)
* assembly [Aspose.Note](../../../)


