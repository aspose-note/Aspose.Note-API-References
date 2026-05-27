---
title: "DocumentFontsSubsystem.UsingDefaultFontFromFile"
second_title: "Aspose.Note for .NET API 参考"
description: "DocumentFontsSubsystem 方法。创建新的 DocumentFontsSubsystem 实例，使用指定文件中的字体作为默认"
type: docs
weight: 40
url: /zh/net/aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromfile/
---
## DocumentFontsSubsystem.UsingDefaultFontFromFile method

使用指定文件中的字体作为默认值创建新的 DocumentFontsSubsystem 实例。

```csharp
public static DocumentFontsSubsystem UsingDefaultFontFromFile(string filePath, 
    Dictionary<string, string> fontsSubstitutions = null)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| filePath | String | 包含默认字体名称的文件。 |
| fontsSubstitutions | Dictionary`2 | 字体替换。 |

### 返回值

该 [`DocumentFontsSubsystem`](../)。

## 示例

展示如何使用来自文件的默认字体将文档保存为 PDF 格式。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// 将文档加载到 Aspose.Note 中。
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// 将文档保存为 PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromFile_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions()
                          {
                              FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromFile(fontFile)
                          });
```

### 另请参阅

* class [DocumentFontsSubsystem](../)
* namespace [Aspose.Note.Fonts](../../documentfontssubsystem/)
* assembly [Aspose.Note](../../../)


