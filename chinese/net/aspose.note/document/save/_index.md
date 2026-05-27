---
title: "Document.Save"
second_title: "Aspose.Note for .NET API 参考"
description: "Document 方法。将 OneNote 文档保存到文件。"
type: docs
weight: 140
url: /zh/net/aspose.note/document/save/
---
## Save(string) {#save_3}

将 OneNote 文档保存到文件中。

```csharp
public void Save(string fileName)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fileName | String | 文件的完整名称。如果已存在具有指定完整名称的文件，则会覆盖现有文件。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | 文档结构违反规范。 |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | 不支持请求的保存格式。 |

## 示例

展示如何保存文档。

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormat_out.one";

Document doc = new Document(dataDir + inputFile);
doc.Save(dataDir + outputFile);
```

### 另请参阅

* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)

---

## Save(Stream) {#save}

将 OneNote 文档保存到流中。

```csharp
public void Save(Stream stream)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | 流 | 用于保存文档的 System.IO.Stream。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | 文档结构违反规范。 |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | 不支持请求的保存格式。 |

### 另请参阅

* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)

---

## Save(string, SaveFormat) {#save_4}

以指定格式将 OneNote 文档保存到文件中。

```csharp
public void Save(string fileName, SaveFormat format)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fileName | String | 文件的完整名称。如果已存在具有指定完整名称的文件，则会覆盖现有文件。 |
| 格式 | SaveFormat | 用于保存文档的格式。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | 文档结构违反规范。 |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | 不支持请求的保存格式。 |

## 示例

展示如何使用 SaveFormat 枚举保存文档。

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingSaveFormat_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, SaveFormat.One);
```

展示如何将文档保存为 gif 格式。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note 中。
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToImageDefaultOptions_out.gif";

// 将文档保存为 gif。
oneFile.Save(dataDir, SaveFormat.Gif);
```

### 另请参阅

* enum [SaveFormat](../../saveformat/)
* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)

---

## Save(Stream, SaveFormat) {#save_1}

以指定格式将 OneNote 文档保存到流中。

```csharp
public void Save(Stream stream, SaveFormat format)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | 流 | 用于保存文档的 System.IO.Stream。 |
| 格式 | SaveFormat | 用于保存文档的格式。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | 文档结构违反规范。 |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | 不支持请求的保存格式。 |

## 示例

展示如何将 OneNote 文档转换为 HTML 格式。

```csharp
var dataDir = RunExamples.GetDataDir_Conversion_Html();

var oneFilePath = Path.Combine(dataDir, "sample.one");
var htmlFilePath = Path.Combine(dataDir, "output.html");

// 将 OneNote 转换为 HTML
var doc = new Document(oneFilePath);
doc.Save(htmlFilePath, SaveFormat.Html);
```

展示如何使用默认设置将文档保存为 pdf 格式。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note 中。
Document oneFile = new Document(dataDir + "Aspose.one");

// 将文档保存为 PDF
dataDir = dataDir + "SaveWithDefaultSettings_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

展示如何将文档保存到流中。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note 中。
Document doc = new Document(dataDir + "Aspose.one");

MemoryStream dstStream = new MemoryStream();
doc.Save(dstStream, SaveFormat.Pdf);

// 将流位置倒回到零，以便下一个读取器使用。
dstStream.Seek(0, SeekOrigin.Begin);
```

展示如何将 OneNote 文档转换为 Markdown 格式。

```csharp
var dataDir = RunExamples.GetDataDir_Conversion_Markdown();

var oneFilePath = Path.Combine(dataDir, "sample.one");
var mdFilePath = Path.Combine(dataDir, "output.md");
var htmlFilePath = Path.Combine(dataDir, "temp.html");

// 将 OneNote 转换为 HTML
var document = new Document(oneFilePath);
document.Save(htmlFilePath, SaveFormat.Html);

// 将 HTML 转换为 Markdown
Converter.ConvertHTML(htmlFilePath, new MarkdownSaveOptions(), mdFilePath);

Console.WriteLine("\nOneNote document converted to Markdown successfully.");
```

展示如何对文档应用暗色主题样式。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_Text();

// 将文档加载到 Aspose.Note 中。
Document doc = new Document(Path.Combine(dataDir, "Aspose.one"));

foreach (var page in doc)
{
    page.BackgroundColor = Color.Black;
}

foreach (var node in doc.GetChildNodes<RichText>())
{
    var c = node.ParagraphStyle.FontColor;
    if (c.IsEmpty || Math.Abs(c.R - Color.Black.R) + Math.Abs(c.G - Color.Black.G) + Math.Abs(c.B - Color.Black.B) <= 30)
    {
        node.ParagraphStyle.FontColor = Color.White;
    }
}

doc.Save(Path.Combine(dataDir, "AsposeDarkTheme.pdf"));
```

### 另请参阅

* enum [SaveFormat](../../saveformat/)
* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)

---

## Save(string, SaveOptions) {#save_5}

使用指定的保存选项将 OneNote 文档保存到文件中。

```csharp
public void Save(string fileName, SaveOptions options)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fileName | String | 文件的完整名称。如果已存在具有指定完整名称的文件，则会覆盖现有文件。 |
| 选项 | SaveOptions | 指定文档在文件中保存的选项。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | 文档结构违反规范。 |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | 不支持请求的保存格式。 |

## 示例

展示如何使用 OneSaveOptions 保存文档。

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingOneSaveOptions_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, new OneSaveOptions());
```

展示如何使用 SaveFormat 将文档保存为 JPEG 格式的图像。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note 中。
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToJpegImageUsingSaveFormat_out.jpg";

// 保存文档。
oneFile.Save(dataDir, SaveFormat.Jpeg);
```

展示如何使用 ImageSaveOptions 将文档保存为 BMP 格式的图像。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note 中。
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBmpImageUsingImageSaveOptions_out.bmp";

// 保存文档。
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Bmp));
```

展示如何将文档保存为 Pdf 格式并使用 Letter 页面布局。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note 中。
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingLetterPageSettings.pdf");

// 保存文档。
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.Letter });
```

展示如何将文档保存为 Pdf 格式并使用 A4 页面布局且不限制高度。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note 中。
Document oneFile = new Document(dataDir + "OneNote.one");

var dst = Path.Combine(dataDir, "SaveToPdfUsingA4PageSettingsWithoutHeightLimit.pdf");

// 保存文档。
oneFile.Save(dst, new PdfSaveOptions() { PageSettings = PageSettings.A4NoHeightLimit });
```

展示如何将文档保存为灰度图像。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note 中。
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveAsGrayscaleImage_out.png";

// 将文档保存为 gif。
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                          {
                              ColorMode = ColorMode.GrayScale
                          });
```

展示如何使用 PackBits 压缩将文档保存为 TIFF 格式的图像。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note 中。
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingPackBitsCompression.tiff");

// 保存文档。
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          TiffCompression = TiffCompression.PackBits
                      });
```

展示如何使用 JPEG 压缩将文档保存为 TIFF 格式的图像。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note 中。
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingJpegCompression.tiff");

// 保存文档。
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          TiffCompression = TiffCompression.Jpeg,
                          Quality = 93
                      });
```

展示如何使用 CCITT Group 3 传真压缩将文档保存为 TIFF 格式的图像。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note 中。
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingCcitt3Compression.tiff");

// 保存文档。
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          ColorMode = ColorMode.BlackAndWhite,
                          TiffCompression = TiffCompression.Ccitt3
                      });
```

展示如何以 PDF 格式保存文档。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note 中。
Document oneFile = new Document(dataDir + "Aspose.one");

// 初始化 PdfSaveOptions 对象
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // 设置要保存的第一页的页面索引
                              PageIndex = 0,

                              // 设置页面数量
                              PageCount = 1,
                          };

// 将文档保存为 PDF
dataDir = dataDir + "SaveRangeOfPagesAsPDF_out.pdf";
oneFile.Save(dataDir, opts);
```

展示如何使用特定设置以 PDF 格式保存文档。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note 中。
Document doc = new Document(dataDir + "Aspose.one");

// 初始化 PdfSaveOptions 对象
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // 使用 Jpeg 压缩
                              ImageCompression = Saving.Pdf.PdfImageCompression.Jpeg,

                              // JPEG 压缩质量
                              JpegQuality = 90
                          };

dataDir = dataDir + "Document.SaveWithOptions_out.pdf";
doc.Save(dataDir, opts);
```

展示如何使用 Otsu 方法将文档保存为二值图像。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note 中。
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBinaryImageUsingOtsuMethod_out.png";

// 将文档保存为 gif。
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                        {
                            ColorMode = ColorMode.BlackAndWhite,
                            BinarizationOptions = new ImageBinarizationOptions()
                                                  {
                                                      BinarizationMethod = BinarizationMethod.Otsu,
                                                  }
                        });
```

展示如何使用固定阈值将文档保存为二值图像。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note 中。
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBinaryImageUsingFixedThreshold_out.png";

// 将文档保存为 gif。
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                          {
                              ColorMode = ColorMode.BlackAndWhite,
                              BinarizationOptions = new ImageBinarizationOptions()
                                                        {
                                                            BinarizationMethod = BinarizationMethod.FixedThreshold,
                                                            BinarizationThreshold = 123
                                                        }
                          });
```

### 另请参阅

* class [SaveOptions](../../../aspose.note.saving/saveoptions/)
* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)

---

## Save(Stream, SaveOptions) {#save_2}

使用指定的保存选项将 OneNote 文档保存到流中。

```csharp
public void Save(Stream stream, SaveOptions options)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | 流 | 用于保存文档的 System.IO.Stream。 |
| 选项 | SaveOptions | 指定文档在流中保存的选项。 |

### 异常

| 异常 | 条件 |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception/) | 文档结构违反规范。 |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception/) | 不支持请求的保存格式。 |

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

展示如何使用来自流的默认字体将文档保存为 PDF 格式。

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

### 另请参阅

* class [SaveOptions](../../../aspose.note.saving/saveoptions/)
* class [Document](../)
* namespace [Aspose.Note](../../document/)
* assembly [Aspose.Note](../../../)


