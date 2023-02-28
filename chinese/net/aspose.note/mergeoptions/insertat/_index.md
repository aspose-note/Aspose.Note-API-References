---
title: MergeOptions.InsertAt
second_title: Aspose.Note for .NET API 参考
description: MergeOptions 财产. 获取或设置将插入导入页面的位置
type: docs
weight: 40
url: /zh/net/aspose.note/mergeoptions/insertat/
---
## MergeOptions.InsertAt property

获取或设置将插入导入页面的位置。

```csharp
public int InsertAt { get; set; }
```

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| ArgumentOutOfRangeException |  |

### 评论

如果值大于目标文档中的页数，则将导入的页面添加到文档末尾。

### 例子

显示如何从一组 PDF 文档导入所有页面，同时从每个 PDF 文档插入页面作为顶级 OneNote 页面的子页面。

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

### 也可以看看

* class [MergeOptions](../)
* 命名空间 [Aspose.Note](../../mergeoptions/)
* 部件 [Aspose.Note](../../../)


