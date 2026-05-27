---
title: "RichText.Replace"
second_title: "Aspose.Note for .NET API 参考"
description: "RichText 方法。将此实例中指定的 Unicode 字符的所有出现替换为另一个指定的 Unicode 字符"
type: docs
weight: 230
url: /zh/net/aspose.note/richtext/replace/
---
## Replace(char, char) {#replace}

将此实例中所有指定的 Unicode 字符替换为另一个指定的 Unicode 字符。

```csharp
public RichText Replace(char oldChar, char newChar)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 旧字符 | Char | 旧字符。 |
| 新字符 | Char | 新字符。 |

### 返回值

该 [`RichText`](../)。

### 另请参阅

* class [RichText](../)
* namespace [Aspose.Note](../../richtext/)
* assembly [Aspose.Note](../../../)

---

## Replace(string, string) {#replace_1}

将当前实例中所有指定的字符串替换为另一个指定的字符串。

```csharp
public RichText Replace(string oldValue, string newValue)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| oldValue | String | 旧值。 |
| newValue | String | 新值。 |

### 返回值

该 [`RichText`](../)。

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentNullException |  |
| ArgumentException |  |

## 示例

展示如何遍历页面的文本并进行替换。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Text();

Dictionary<string, string> replacements = new Dictionary<string, string>();
replacements.Add("voice over", "voice over new text");

// 将文档加载到 Aspose.Note 中。
Document oneFile = new Document(dataDir + "Aspose.one");

IList<Page> pageNodes = oneFile.GetChildNodes<Page>();

// 获取所有 RichText 节点
IList<RichText> textNodes = pageNodes[0].GetChildNodes<RichText>();

foreach (RichText richText in textNodes)
{
    foreach (KeyValuePair<string, string> kvp in replacements)
    {
        // 替换形状的文本
        richText.Replace(kvp.Key, kvp.Value);
    }
}

// 保存为任何受支持的文件格式
dataDir = dataDir + "ReplaceTextOnParticularPage_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

展示如何通过在模板中替换特殊文本片段来生成新文档。

```csharp
string dataDir = RunExamples.GetDataDir_Text();

var D = new Dictionary<string, string>
            {
                { "Company", "Atlas Shrugged Ltd" },
                { "CandidateName", "John Galt" },
                { "JobTitle", "Chief Entrepreneur Officer" },
                { "Department", "Sales" },
                { "Salary", "123456 USD" },
                { "Vacation", "30" },
                { "StartDate", "29 Feb 2024" },
                { "YourName", "Ayn Rand" }
            };

// 将模板文档加载到 Aspose.Note 中。
var d = new Document(Path.Combine(dataDir, "JobOffer.one"));

// 让我们替换所有模板词汇
foreach (var e in d.GetChildNodes<RichText>())
{
    foreach (var replace in D)
    {
        e.Replace($"${{{replace.Key}}}", replace.Value);
    }
}

d.Save(Path.Combine(dataDir, "JobOffer_out.one"));
```

### 另请参阅

* class [RichText](../)
* namespace [Aspose.Note](../../richtext/)
* assembly [Aspose.Note](../../../)

---

## Replace(string, string, TextStyle) {#replace_2}

将当前实例中所有指定的字符串替换为具有指定样式的另一个指定字符串。

```csharp
public RichText Replace(string oldValue, string newValue, TextStyle style)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| oldValue | String | 旧值。 |
| newValue | String | 新值。 |
| style | TextStyle | 新值的样式。 |

### 返回值

该 [`RichText`](../)。

### 异常

| 异常 | 条件 |
| --- | --- |
| ArgumentNullException |  |
| ArgumentException |  |

### 另请参阅

* class [TextStyle](../../textstyle/)
* class [RichText](../)
* namespace [Aspose.Note](../../richtext/)
* assembly [Aspose.Note](../../../)


