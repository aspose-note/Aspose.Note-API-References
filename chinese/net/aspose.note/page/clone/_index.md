---
title: "Page.Clone"
second_title: "Aspose.Note for .NET API 参考"
description: "Page 方法。克隆页面"
type: docs
weight: 140
url: /zh/net/aspose.note/page/clone/
---
## Page.Clone method

克隆页面。

```csharp
public Page Clone(bool cloneHistory = false)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| cloneHistory | Boolean | 指定是否应克隆页面的历史记录。 |

### 返回值

页面的克隆。

## 示例

展示如何将页面的当前版本推送到历史记录。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Pages();

// 加载 OneNote 文档并获取第一个子项
Document document = new Document(dataDir + "Aspose.one");
Page page = document.FirstChild;

var pageHistory = document.GetPageHistory(page);

pageHistory.Add(page.Clone());

document.Save(dataDir + "PushCurrentPageVersion_out.one");
```

展示如何克隆页面。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Pages();

// 加载 OneNote 文档
Document document = new Document(dataDir + "Aspose.one", new LoadOptions { LoadHistory = true });

// 克隆到新文档（不含历史）
var cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone());

// 克隆到新文档（含历史）
cloned = new Document();
cloned.AppendChildLast(document.FirstChild.Clone(true));
```

### 另请参阅

* class [Page](../)
* namespace [Aspose.Note](../../page/)
* assembly [Aspose.Note](../../../)


