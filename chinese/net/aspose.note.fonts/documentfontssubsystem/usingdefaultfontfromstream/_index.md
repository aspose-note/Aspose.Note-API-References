---
title: DocumentFontsSubsystem.UsingDefaultFontFromStream
second_title: Aspose.Note for .NET API 参考
description: DocumentFontsSubsystem 方法. 使用来自指定流的字体作为默认值创建新的 DocumentFontsSubsystem 实例
type: docs
weight: 50
url: /zh/net/aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromstream/
---
## DocumentFontsSubsystem.UsingDefaultFontFromStream method

使用来自指定流的字体作为默认值创建新的 DocumentFontsSubsystem 实例。

```csharp
public static DocumentFontsSubsystem UsingDefaultFontFromStream(Stream defaultFontStream, 
    Dictionary<string, string> fontsSubstitutions = null)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| defaultFontStream | Stream | 包含默认字体名称的流。 |
| fontsSubstitutions | Dictionary`2 | 字体替换。 |

### 返回值

的[`DocumentFontsSubsystem`](../).

### 例子

显示如何使用流中的默认字体以 pdf 格式保存文档。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// 将文档加载到 Aspose.Note 中。
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// 将文档保存为 PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromStream_out.pdf";

using (var stream = File.Open(fontFile, FileMode.Open, FileAccess.Read, FileShare.Read))
{
    oneFile.Save(dataDir, new PdfSaveOptions()
                              {
                                  FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromStream(stream)
                              });
}
```

### 也可以看看

* class [DocumentFontsSubsystem](../)
* 命名空间 [Aspose.Note.Fonts](../../documentfontssubsystem/)
* 部件 [Aspose.Note](../../../)


