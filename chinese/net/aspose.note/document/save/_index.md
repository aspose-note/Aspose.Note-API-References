---
title: Save
second_title: Aspose.Note for .NET API 参考
description: 将 OneNote 文档保存到文件中
type: docs
weight: 140
url: /zh/net/aspose.note/document/save/
---
## Save(string) {#save_3}

将 OneNote 文档保存到文件中。

```csharp
public void Save(string fileName)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| fileName | String | 文件的全名。如果指定全名的文件已经存在，则覆盖现有文件。 |

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception) | 文档结构违反规范。 |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception) | 不支持请求的保存格式。 |

### 例子

显示如何保存文档。

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormat_out.one";

Document doc = new Document(dataDir + inputFile);
doc.Save(dataDir + outputFile);
```

### 也可以看看

* class [Document](../../document)
* 命名空间 [Aspose.Note](../../document)
* 部件 [Aspose.Note](../../../)

---

## Save(Stream) {#save}

将 OneNote 文档保存到流中。

```csharp
public void Save(Stream stream)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| stream | Stream | 将保存文档的 System.IO.Stream。 |

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception) | 文档结构违反规范。 |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception) | 不支持请求的保存格式。 |

### 也可以看看

* class [Document](../../document)
* 命名空间 [Aspose.Note](../../document)
* 部件 [Aspose.Note](../../../)

---

## Save(string, SaveFormat) {#save_4}

将 OneNote 文档保存到指定格式的文件中。

```csharp
public void Save(string fileName, SaveFormat format)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| fileName | String | 文件的全名。如果指定全名的文件已经存在，则覆盖现有文件。 |
| format | SaveFormat | 保存文档的格式。 |

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception) | 文档结构违反规范。 |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception) | 不支持请求的保存格式。 |

### 例子

演示如何使用 SaveFormat 枚举保存文档。

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingSaveFormat_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, SaveFormat.One);
```

显示如何以 gif 格式保存文档。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note。
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToImageDefaultOptions_out.gif";

// 将文档保存为 gif。
oneFile.Save(dataDir, SaveFormat.Gif);
```

### 也可以看看

* enum [SaveFormat](../../saveformat)
* class [Document](../../document)
* 命名空间 [Aspose.Note](../../document)
* 部件 [Aspose.Note](../../../)

---

## Save(Stream, SaveFormat) {#save_1}

将 OneNote 文档以指定格式保存到流中。

```csharp
public void Save(Stream stream, SaveFormat format)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| stream | Stream | 将保存文档的 System.IO.Stream。 |
| format | SaveFormat | 保存文档的格式。 |

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception) | 文档结构违反规范。 |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception) | 不支持请求的保存格式。 |

### 例子

显示如何使用默认设置以 pdf 格式保存文档。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note。
Document oneFile = new Document(dataDir + "Aspose.one");

// 将文档保存为 PDF
dataDir = dataDir + "SaveWithDefaultSettings_out.pdf";
oneFile.Save(dataDir, SaveFormat.Pdf);
```

显示如何将文档保存到流中。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note。
Document doc = new Document(dataDir + "Aspose.one");

MemoryStream dstStream = new MemoryStream();
doc.Save(dstStream, SaveFormat.Pdf);

// 将流位置倒回零，以便为下一个阅读器做好准备。
dstStream.Seek(0, SeekOrigin.Begin);
```

### 也可以看看

* enum [SaveFormat](../../saveformat)
* class [Document](../../document)
* 命名空间 [Aspose.Note](../../document)
* 部件 [Aspose.Note](../../../)

---

## Save(string, SaveOptions) {#save_5}

使用指定的保存选项将 OneNote 文档保存到文件中。

```csharp
public void Save(string fileName, SaveOptions options)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| fileName | String | 文件的全名。如果指定全名的文件已经存在，则覆盖现有文件。 |
| options | SaveOptions | 指定文档如何保存在文件中的选项。 |

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception) | 文档结构违反规范。 |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception) | 不支持请求的保存格式。 |

### 例子

演示如何使用 OneSaveOptions 保存文档。

```csharp
string inputFile = "Sample1.one";
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();
string outputFile = "SaveDocToOneNoteFormatUsingOneSaveOptions_out.one";

Document document = new Document(dataDir + inputFile);

document.Save(dataDir + outputFile, new OneSaveOptions());
```

演示如何使用 SaveFormat 将文档保存为 Jpeg 格式的图像。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note。
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToJpegImageUsingSaveFormat_out.jpg";

// 保存文档。
oneFile.Save(dataDir, SaveFormat.Jpeg);
```

演示如何使用 ImageSaveOptions 将文档保存为 Bmp 格式的图像。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note。
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveToBmpImageUsingImageSaveOptions_out.bmp";

// 保存文档。
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Bmp));
```

显示如何将文档另存为灰度图像。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note。
Document oneFile = new Document(dataDir + "Aspose.one");

dataDir = dataDir + "SaveAsGrayscaleImage_out.png";

// 将文档保存为 gif。
oneFile.Save(dataDir, new ImageSaveOptions(SaveFormat.Png)
                          {
                              ColorMode = ColorMode.GrayScale
                          });
```

演示如何使用 PackBits 压缩将文档另存为 Tiff 格式的图像。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note。
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingPackBitsCompression.tiff");

// 保存文档。
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          TiffCompression = TiffCompression.PackBits
                      });
```

演示如何使用 Jpeg 压缩将文档保存为 Tiff 格式的图像。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note。
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingJpegCompression.tiff");

// 保存文档。
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          TiffCompression = TiffCompression.Jpeg,
                          Quality = 93
                      });
```

展示如何使用 CCITT Group 3 传真压缩将文档保存为 Tiff 格式的图像。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note。
Document oneFile = new Document(Path.Combine(dataDir, "Aspose.one"));

var dst = Path.Combine(dataDir, "SaveToTiffUsingCcitt3Compression.tiff");

// 保存文档。
oneFile.Save(dst, new ImageSaveOptions(SaveFormat.Tiff)
                      {
                          ColorMode = ColorMode.BlackAndWhite,
                          TiffCompression = TiffCompression.Ccitt3
                      });
```

显示如何以 pdf 格式保存文档。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note。
Document oneFile = new Document(dataDir + "Aspose.one");

// 初始化 PdfSaveOptions 对象
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // 设置要保存的第一页的页索引
                              PageIndex = 0,

                              // 设置页数
                              PageCount = 1,
                          };

// 将文档保存为 PDF
dataDir = dataDir + "SaveRangeOfPagesAsPDF_out.pdf";
oneFile.Save(dataDir, opts);
```

显示如何使用特定设置以 pdf 格式保存文档。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note。
Document doc = new Document(dataDir + "Aspose.one");

// 初始化 PdfSaveOptions 对象
PdfSaveOptions opts = new PdfSaveOptions
                          {
                              // 使用 Jpeg 压缩
                              ImageCompression = Saving.Pdf.PdfImageCompression.Jpeg,

                              // JPEG 压缩的质量
                              JpegQuality = 90
                          };

dataDir = dataDir + "Document.SaveWithOptions_out.pdf";
doc.Save(dataDir, opts);
```

展示如何使用 Otsu 的方法将文档保存为二进制图像。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note。
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

展示如何使用固定阈值将文档保存为二进制图像。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note。
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

### 也可以看看

* class [SaveOptions](../../../aspose.note.saving/saveoptions)
* class [Document](../../document)
* 命名空间 [Aspose.Note](../../document)
* 部件 [Aspose.Note](../../../)

---

## Save(Stream, SaveOptions) {#save_2}

使用指定的保存选项将 OneNote 文档保存到流中。

```csharp
public void Save(Stream stream, SaveOptions options)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| stream | Stream | 将保存文档的 System.IO.Stream。 |
| options | SaveOptions | 指定文档如何保存在流中的选项。 |

### 例外

| 例外 | （健康）状况 |
| --- | --- |
| [IncorrectDocumentStructureException](../../incorrectdocumentstructureexception) | 文档结构违反规范。 |
| [UnsupportedSaveFormatException](../../unsupportedsaveformatexception) | 不支持请求的保存格式。 |

### 例子

展示如何使用指定的默认字体以 pdf 格式保存文档。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

// 将文档加载到 Aspose.Note。
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// 将文档保存为 PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontName_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions() 
                      {
                          FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFont("Times New Roman")
                      });
```

演示如何使用文件中的默认字体将文档保存为 pdf 格式。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// 将文档加载到 Aspose.Note。
Document oneFile = new Document(Path.Combine(dataDir, "missing-font.one"));

// 将文档保存为 PDF
dataDir = dataDir + "SaveUsingDocumentFontsSubsystemWithDefaultFontFromFile_out.pdf";
oneFile.Save(dataDir, new PdfSaveOptions()
                          {
                              FontsSubsystem = DocumentFontsSubsystem.UsingDefaultFontFromFile(fontFile)
                          });
```

演示如何使用流中的默认字体以 pdf 格式保存文档。

```csharp
// 文档目录的路径。
string dataDir = RunExamples.GetDataDir_LoadingAndSaving();

string fontFile = Path.Combine(dataDir, "geo_1.ttf");

// 将文档加载到 Aspose.Note。
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

* class [SaveOptions](../../../aspose.note.saving/saveoptions)
* class [Document](../../document)
* 命名空间 [Aspose.Note](../../document)
* 部件 [Aspose.Note](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Note.dll -->
