---
title: DocumentFontsSubsystem.UsingDefaultFontFromFile
second_title: Aspose.Note for .NET API 参考
description: DocumentFontsSubsystem 方法. 使用指定文件中的字体作为默认字体创建新的 DocumentFontsSubsystem 实例
type: docs
weight: 40
url: /zh/net/aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromfile/
---
## DocumentFontsSubsystem.UsingDefaultFontFromFile method

使用指定文件中的字体作为默认字体创建新的 DocumentFontsSubsystem 实例。

```csharp
public static DocumentFontsSubsystem UsingDefaultFontFromFile(string filePath, 
    Dictionary<string, string> fontsSubstitutions = null)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| filePath | String | 包含默认字体名称的文件。 |
| fontsSubstitutions | Dictionary`2 | 字体替换。 |

### 返回值

的[`DocumentFontsSubsystem`](../).

### 例子

显示如何使用文件中的默认字体将文档保存为 pdf 格式。

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

### 也可以看看

* class [DocumentFontsSubsystem](../)
* 命名空间 [Aspose.Note.Fonts](../../documentfontssubsystem/)
* 部件 [Aspose.Note](../../../)


