---
title: "Document.Document"
second_title: "Aspose.Note for .NET API 参考"
description: "Document 构造函数。初始化 Document 类的新实例。创建一个空的 OneNote 文档"
type: docs
weight: 10
url: /zh/net/aspose.note/document/document/
---
## Document() {#constructor}

初始化 [`Document`](../) 类的新实例。创建一个空的 OneNote 文档。

```csharp
public Document()
```

### 另请参阅

* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)

---

## Document(string) {#constructor_3}

初始化 [`Document`](../) 类的新实例。打开文件中的现有 OneNote 文档。

```csharp
public Document(string filePath)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| filePath | String | 文件路径。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception/) | 未识别或不支持该文档格式。 |
| [FileCorruptedException](../../filecorruptedexception/) | 文档似乎已损坏，无法加载。 |
| [IncorrectPasswordException](../../incorrectpasswordexception/) | 文档已加密，需要密码才能打开，但您提供的密码不正确。 |
| InvalidOperationException | 文档存在问题，应向 Aspose.Note 开发人员报告。 |
| IOException | 发生输入/输出异常。 |

## 示例

展示如何将 OneNote 文档转换为 Notion 兼容的 HTML。

```csharp
var dataDir = RunExamples.GetDataDir_Import();
var documentPath = Path.Combine(dataDir, "Sample.one");

// 初始化 OneNote 文档
var document = new Document(documentPath);

// Notion 客户端设置
var authToken = "your-notion-auth-token";
var parentPageId = "your-notion-parent-page-id";

var client = NotionClientFactory.Create(new ClientOptions
{
    AuthToken = authToken
});

// 检索 Notion 页面
var page = await client.Pages.RetrieveAsync(parentPageId);

// 遍历 OneNote 页面并将其添加到 Notion
foreach (var oneNotePage in document)
{
    var oneNoteAllRichText = oneNotePage.GetChildNodes<RichText>();

    var pagesCreateParametersBuilder = PagesCreateParametersBuilder
        .Create(new ParentPageInput { PageId = page.Id })
        .AddProperty("title",
        new TitlePropertyValue
        {
            Title = new List<RichTextBase>
            {
            new RichTextTextInput { Text = new Notion.Client.Text { Content = oneNotePage.Title.TitleText.Text } }
            }
        });

    foreach (var richText in oneNoteAllRichText)
    {
        // 跳过标题、日期或时间文本
        if (richText.IsTitleDate || richText.IsTitleText || richText.IsTitleTime)
        {
            continue;
        }

        pagesCreateParametersBuilder.AddPageContent(new ParagraphBlock
        {
            Paragraph = new ParagraphBlock.Info
            {
                RichText = new List<RichTextBase> {
                new RichTextText
                {
                    Text = new Notion.Client.Text { Content = richText.Text }
                }
            }
            }
        });
    }

    // 在 Notion 中创建页面
    var pagesCreateParameters = pagesCreateParametersBuilder.Build();
    await client.Pages.CreateAsync(pagesCreateParameters);
}

Console.WriteLine("\nOneNote document converted to Notion-compatible format successfully.");
```

### 另请参阅

* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)

---

## Document(string, LoadOptions) {#constructor_4}

初始化 [`Document`](../) 类的新实例。打开文件中的现有 OneNote 文档。允许指定额外选项，例如加密密码。

```csharp
public Document(string filePath, LoadOptions loadOptions)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| filePath | String | 文件路径。 |
| loadOptions | LoadOptions | 用于加载文档的选项。可以为 null。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception/) | 未识别或不支持该文档格式。 |
| [FileCorruptedException](../../filecorruptedexception/) | 文档似乎已损坏，无法加载。 |
| [IncorrectPasswordException](../../incorrectpasswordexception/) | 文档已加密，需要密码才能打开，但您提供的密码不正确。 |
| InvalidOperationException | 文档存在问题，应向 Aspose.Note 开发人员报告。 |
| IOException | 发生输入/输出异常。 |

### 另请参阅

* class [LoadOptions](../../loadoptions/)
* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)

---

## Document(Stream) {#constructor_1}

初始化一个新的 [`Document`](../) 类实例。 从流中打开现有的 OneNote 文档。

```csharp
public Document(Stream inStream)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| inStream | 流 | 流。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception/) | 未识别或不支持该文档格式。 |
| [FileCorruptedException](../../filecorruptedexception/) | 文档似乎已损坏，无法加载。 |
| [IncorrectPasswordException](../../incorrectpasswordexception/) | 文档已加密，需要密码才能打开，但您提供的密码不正确。 |
| InvalidOperationException | 文档存在问题，应向 Aspose.Note 开发人员报告。 |
| IOException | 发生输入/输出异常。 |
| ArgumentException | 流不支持读取，或为 null，或已关闭。 |

### 另请参阅

* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)

---

## Document(Stream, LoadOptions) {#constructor_2}

初始化一个新的 [`Document`](../) 类实例。 从流中打开现有的 OneNote 文档。 允许指定额外选项，例如加密密码。

```csharp
public Document(Stream inStream, LoadOptions loadOptions)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| inStream | 流 | 流。 |
| loadOptions | LoadOptions | 用于加载文档的选项。可以为 null。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| [UnsupportedFileFormatException](../../unsupportedfileformatexception/) | 未识别或不支持该文档格式。 |
| [FileCorruptedException](../../filecorruptedexception/) | 文档似乎已损坏，无法加载。 |
| [IncorrectPasswordException](../../incorrectpasswordexception/) | 文档已加密，需要密码才能打开，但您提供的密码不正确。 |
| InvalidOperationException | 文档存在问题，应向 Aspose.Note 开发人员报告。 |
| IOException | 发生输入/输出异常。 |
| ArgumentException | 流不支持读取，或为 null，或已关闭。 |

### 另请参阅

* class [LoadOptions](../../loadoptions/)
* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)


