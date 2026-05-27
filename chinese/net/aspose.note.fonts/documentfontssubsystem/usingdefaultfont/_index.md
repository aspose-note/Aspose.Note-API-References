---
title: "DocumentFontsSubsystem.UsingDefaultFont"
second_title: "Aspose.Note for .NET API 参考"
description: "DocumentFontsSubsystem 方法。创建新的 DocumentFontsSubsystem 实例，使用指定的默认字体名称"
type: docs
weight: 30
url: /zh/net/aspose.note.fonts/documentfontssubsystem/usingdefaultfont/
---
## DocumentFontsSubsystem.UsingDefaultFont method

使用指定的默认字体名称创建新的 DocumentFontsSubsystem 实例。

```csharp
public static DocumentFontsSubsystem UsingDefaultFont(string defaultFontName, 
    Dictionary<string, string> fontsSubstitutions = null)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| defaultFontName | String | 默认字体名称。 |
| fontsSubstitutions | Dictionary`2 | 字体替换。 |

### 返回值

该 [`DocumentFontsSubsystem`](../)。

## 示例

展示如何使用指定的默认字体将文档保存为 PDF 格式。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note 中。
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// 将文档保存为 PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontName_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions() 
                      {
                          FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFont("Times New Roman")
                      });
```

### 另请参阅

* class [DocumentFontsSubsystem](../)
* namespace [Aspose.Note.Fonts](../../documentfontssubsystem/)
* assembly [Aspose.Note](../../../)


