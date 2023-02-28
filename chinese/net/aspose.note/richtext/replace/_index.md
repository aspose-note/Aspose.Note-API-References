---
title: RichText.Replace
second_title: Aspose.Note for .NET API 参考
description: RichText 方法. 将此实例中所有出现的指定 Unicode 字符替换为另一个指定的 Unicode 字符
type: docs
weight: 200
url: /zh/net/aspose.note/richtext/replace/
---
## Replace(char, char) {#replace}

将此实例中所有出现的指定 Unicode 字符替换为另一个指定的 Unicode 字符。

```csharp
public RichText Replace(char oldChar, char newChar)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| oldChar | Char | 旧字符. |
| newChar | Char | 新字符。 |

### 返回值

的[`RichText`](../).

### 也可以看看

* class [RichText](../)
* 命名空间 [Aspose.Note](../../richtext/)
* 部件 [Aspose.Note](../../../)

---

## Replace(string, string) {#replace_1}

用另一个指定的字符串替换当前实例中所有出现的指定字符串。

```csharp
public RichText Replace(string oldValue, string newValue)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| oldValue | String | 旧值。 |
| newValue | String | 新值。 |

### 返回值

的[`RichText`](../).

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| ArgumentNullException |  |
| ArgumentException |  |

### 例子

显示如何传递页面文本并进行替换。

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

// 保存为任何支持的文件格式
dataDir = dataDir + "ReplaceTextOnParticularPage_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

展示如何通过替换模板中的特殊文本片段来生成新文档。

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

// 让我们替换所有模板词
foreach (var e in d.GetChildNodes<RichText>())
{
    foreach (var replace in D)
    {
        e.Replace($"${{{replace.Key}}}", replace.Value);
    }
}

d.Save(Path.Combine(dataDir, "JobOffer_out.one"));
```

### 也可以看看

* class [RichText](../)
* 命名空间 [Aspose.Note](../../richtext/)
* 部件 [Aspose.Note](../../../)

---

## Replace(string, string, TextStyle) {#replace_2}

用指定样式的另一个指定字符串替换当前实例中所有出现的指定字符串。

```csharp
public RichText Replace(string oldValue, string newValue, TextStyle style)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| oldValue | String | 旧值。 |
| newValue | String | 新值。 |
| style | TextStyle | 新值的样式。 |

### 返回值

的[`RichText`](../).

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| ArgumentNullException |  |
| ArgumentException |  |

### 也可以看看

* class [TextStyle](../../textstyle/)
* class [RichText](../)
* 命名空间 [Aspose.Note](../../richtext/)
* 部件 [Aspose.Note](../../../)


