---
title: Class DocumentFontsSubsystem
second_title: Aspose.Note for .NET API 参考
description: Aspose.Note.Fonts.DocumentFontsSubsystem 班级. Aspose.Note.Fonts.FontsSubsystem 的简单实现检索FontFamily来自 OS. 的对象
type: docs
weight: 100
url: /zh/net/aspose.note.fonts/documentfontssubsystem/
---
## DocumentFontsSubsystem class

Aspose.Note.Fonts.FontsSubsystem 的简单实现。检索FontFamily来自 OS. 的对象

```csharp
public class DocumentFontsSubsystem : FontsSubsystem
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [DocumentFontsSubsystem](documentfontssubsystem/#constructor)(Dictionary&lt;string, string&gt;) | 初始化一个新的实例`DocumentFontsSubsystem`类. |
| [DocumentFontsSubsystem](documentfontssubsystem/#constructor_1)(Stream, Dictionary&lt;string, string&gt;) | 初始化一个新的实例`DocumentFontsSubsystem`类. |
| [DocumentFontsSubsystem](documentfontssubsystem/#constructor_2)(string, Dictionary&lt;string, string&gt;) | 初始化一个新的实例`DocumentFontsSubsystem`类. |

## 特性

| 姓名 | 描述 |
| --- | --- |
| static [Default](../../aspose.note.fonts/documentfontssubsystem/default/) { get; set; } | 获取或设置静态默认实例。 |
| [DefaultFont](../../aspose.note.fonts/fontssubsystem/defaultfont/) { get; } | 获取或设置默认字体。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| static [UsingDefaultFont](../../aspose.note.fonts/documentfontssubsystem/usingdefaultfont/)(string, Dictionary&lt;string, string&gt;) | 使用指定的默认字体名称创建新的 DocumentFontsSubsystem 实例。 |
| static [UsingDefaultFontFromFile](../../aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromfile/)(string, Dictionary&lt;string, string&gt;) | 使用指定文件中的字体作为默认字体创建新的 DocumentFontsSubsystem 实例。 |
| static [UsingDefaultFontFromStream](../../aspose.note.fonts/documentfontssubsystem/usingdefaultfontfromstream/)(Stream, Dictionary&lt;string, string&gt;) | 使用来自指定流的字体作为默认值创建新的 DocumentFontsSubsystem 实例。 |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont/)(Stream) | 添加字体。 |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont/)(string) | 添加字体。 |
| [AddFont](../../aspose.note.fonts/fontssubsystem/addfont/)(Stream, string) | 添加字体。 |
| [AddFontSubstitution](../../aspose.note.fonts/fontssubsystem/addfontsubstitution/)(string, string) | 添加字体替换。 |
| virtual [GetFontFamily](../../aspose.note.fonts/fontssubsystem/getfontfamily/)(string) | 获取字体系列。 |
| [LoadFontsFromFolder](../../aspose.note.fonts/fontssubsystem/loadfontsfromfolder/)(string) | 将指定文件夹中的所有 TrueType 字体加载到内部集合。 |

### 例子

显示如何使用指定的默认字体以 pdf 格式保存文档。

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

* class [FontsSubsystem](../fontssubsystem/)
* 命名空间 [Aspose.Note.Fonts](../../aspose.note.fonts/)
* 部件 [Aspose.Note](../../)


